# Code.gov Data Quality Scoring

As part of our efforts to make Code.gov as useful as possible to our users, we have implemented rules to score the quality of the data being indexed into Code.gov. This score is not a judgement or critique of the data itself, but an effort on our part to quantify the data we have determined our users look for and need while using our site and API.

## Score Determination

We determine the quality score of a repository by using a series of rules and passing the repository through a rules engine. We also assign a __weight__ to each field that symbolizes the value that field has for Code.gov.

The rules can vary from field to field. As an example, we evaluate the existance of data in all fields before we add their weight to the overall score, but in the case of the __description__ field we also evaluate that the content of the field is not the same as the name of the project and we make a "naive" evaluation on the amount of content that the field has (word count). Other fields are evaluated depending on the data that is expected and desired in them.

### Field Weights

We give weight values between 0 and 1. These values are the maximum score that data in the field can obtain. There are fields where data is evaluated and may be awared less than the values in the following table. There are other fields, like the tags field that may accumulate scores depending on the amount of data submitted (Eg. each tag contributes the field value).

| Field Name                | Field Weight |
| ------------------------- | ------------ |
| name                      | 1            |
| description               | 1            |
| permissions.licenses      | 1            |
| permissions.licenses.URL  | 1            |
| permissions.licenses.name | 1            |
| permissions.usageType     | 1            |
| permissions.exemptionText | 1            |
| organization              | 1            |
| contact.email             | 1            |
| contact.name              | 1            |
| contact.URL               | 1            |
| contact.phone             | 1            |
| tags                      | 1            |
| laborHours                | 1            |
| languages:                | 0.8          |
| repositoryURL:            | 0.8          |
| homepageURL:              | 0.8          |
| downloadURL:              | 0.8          |
| vcs:                      | 0.8          |
| date.created:             | 0.6          |
| date.lastModified:        | 0.6          |
| date.metadataLastUpdated: | 0.6          |
| version:                  | 0.6          |
| status:                   | 0.6          |
| disclaimerURL:            | 0.4          |
| disclaimerText:           | 0.4          |
| relatedCode.name:         | 0.4          |
| relatedCode.URL:          | 0.4          |
| reusedCode.name:          | 0.4          |
| reusedCode.URL:           | 0.4          |
| partners.name:            | 0.4          |
| partners.email:           | 0.4          |
| target_operating_systems: | 0.2          |
| additional_information:   | 0.1          |

### Field Rules

We are using the [simple-rules-engine](https://www.npmjs.com/package/simple-rules-engine) package to evaluate the rules we've created for each field. Our current rules can be seen [here](https://github.com/GSA/code-gov-api/blob/master/services/validator/rules/index.js).

### Score Normalization

We are currently in the process of normalizing the scores of our data. After this development is completed all scores will be between 1 and 10 points. This will give our users an easier way to interprete our data quality scores.
