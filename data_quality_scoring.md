# Code.gov Data Quality Scoring

As part of our efforts to make Code.gov as useful as possible to our users, we have implemented rules to score the quality of the data being indexed into Code.gov. This score is not a judgement or critique of the data itself, but an effort on our part to quantify the data we have determined our users look for and need while using our site and API.

## Score Determination

We determine the quality score of a repository by using a series of rules and passing the repository through a rules engine. We also assign a __point value__ to each field that symbolizes the value that field has for Code.gov.

The rules can vary from field to field. As an example, we evaluate the existance of data in all fields before we add their weight to the overall score, but in the case of the __description__ field we also evaluate that the content of the field is not the same as the name of the project and we make a "naive" evaluation on the amount of content that the field has (word count). Other fields are evaluated depending on the data that is expected and desired in them.

### Field Points

We give point values between 0 and 10. These values are the maximum score that data in the field can obtain. There are fields where data is evaluated and may be awared less than the values in the following table.  Also, fields like tags may be awarded partial value based on number of items

|Field Name|Max Field Points|
|-|-|
|name|10|
|version|1|
|organization|5|
|description|10|
|permissions.licenses.URL|1|
|permissions.licenses.name|7|
|permissions.usageType|10|
|permissions.exemptionText|5|
|tags|10|
|contact.email|10|
|contact.name|5|
|contact.URL|5|
|contact.phone|5|
|status|5|
|vcs|5|
|repositoryURL|10|
|homepageURL|7|
|downloadURL|3|
|disclaimerURL|3|
|disclaimerText|3|
|languages|10|
|laborHours|10|
|relatedCode.name|1|
|relatedCode.URL             |1|
|relatedCode.isGovernmentRepo|1|
|reusedCode.name|1|
|reusedCode.URL|1|
|partners.name|1|
|partners.email|1|
|date.created|5|
|date.lastModified|5|
|date.metadataLastUpdated|2|

### Field Rules

We are using the [simple-rules-engine](https://www.npmjs.com/package/simple-rules-engine) package to evaluate the rules we've created for each field. Our current rules can be seen [here](https://github.com/GSA/code-gov-harvester/blob/master/libs/rules/index.js).

### Score Normalization

Score normalization is performed where the final score is between 0 and 10.  To arrive at this value, all point values of each field in the above table are tallied and divided by maximum possible point and then multipled by 10.
