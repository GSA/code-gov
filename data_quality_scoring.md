# Code.gov Data Quality Scoring

As part of our efforts to make Code.gov as useful as possible to our users, we have implemented rules to score the quality of the data being indexed into Code.gov. This score is not a judgement or critique of the data itself, but an effort on our part to quantify the data we have determined our users look for and need while using our site and API.

## Score Determination

We determine the quality score of a repository by using a series of rules and passing the repository through a rules engine. We also assign a __point value__ to each field that symbolizes the value that field has for Code.gov.

The rules can vary from field to field. As an example, we evaluate the existance of data in all fields before we add their weight to the overall score, but in the case of the __description__ field we also evaluate that the content of the field is not the same as the name of the project and we make a "naive" evaluation on the amount of content that the field has (word count). Other fields are evaluated depending on the data that is expected and desired in them.

### Field Points

We give point values between 0 and 10. These values are the maximum score that data in the field can obtain. There are fields where data is evaluated and may be awared less than the values in the following table.  Also, fields like tags may be awarded partial value based on number of items

|Field Name|Max Field Points|Notes|
|-|-|-|
|name|10||
|version|1||
|organization|5||
|description|10|0 points if descriptions and name are same, 0 points if description is less then 3 words, 3 points of description is less then 10 words, 5 points if description is less then 20 words, 8 points if description is less then 30 words, 10 (full) points if description is 30 or more words |
|permissions.licenses.URL|1|Licenses is an Array of objects and it should have atleast 1 element|
|permissions.licenses.name|7|Licenses is an Array of objects and it should have atleast 1 element|
|permissions.usageType|10|1 point if exempt*, 5 points if governmentWideReuse, 10 (full) points if openSource'|
|permissions.exemptionText|5|5 (full) points if usageType is openSource/governmentWideReuse OR exemptionText is present, 0 otherwise|
|tags|10|Tags is an Array objects, 4 points if 1 tag element, 6 points if 2 tag elements, 10 (full) points if 3 or more tag elements|
|contact.email|10||
|contact.name|5||
|contact.URL|5||
|contact.phone|5|
|status|5||
|vcs|5||
|repositoryURL|10|10 (full) points if valid URL (starts with https:// or http://)||
|homepageURL|7|must exits and be a valid URL to get full points|
|downloadURL|3|must exits and be a valid URL to get full points|
|disclaimerURL|3|must exits and be a valid URL to get full points|
|disclaimerText|3||
|languages|10|Languages is an Array of strings, must have atleast 1 element to get full points|
|laborHours|10|Full points if a positive numeric value|
|relatedCode.name|1||
|relatedCode.URL|1|must exits and be a valid URL to get full points|
|relatedCode.isGovernmentRepo|1||
|reusedCode.name|1||
|reusedCode.URL|1|must exits and be a valid URL to get full points|
|partners.name|1||
|partners.email|1||
|date.created|5||
|date.lastModified|5||
|date.metadataLastUpdated|2||

### Field Rules

We are using the [simple-rules-engine](https://www.npmjs.com/package/simple-rules-engine) package to evaluate the rules we've created for each field. Our current rules can be seen [here](https://github.com/GSA/code-gov-harvester/blob/master/libs/rules/index.js).

### Score Normalization

Score normalization is performed where the final score is between 0 and 10.  To arrive at this value, all point values of each field in the above table are tallied and divided by maximum possible point and then multipled by 10.

### Score Display

The code.gov front end uses a [corner tag](https://gsa.github.io/code-gov-style/components/corner_tags) to display the data quality score. This is implemented by the `quality-tag` component. The tag type/color is determined by the `score` value passed to the component using the following ranges:
- low/red: a score below 4 
- medium/orange: a score greater than or equal to 4 and less than 6
- high/green: a score higher than or equal to 6

*note: because all code.gov projects should have the required fields filled, it is expected that no projects will have the low/red corner tag

For more info on the code.gov corner tags see the [style guide](https://gsa.github.io/code-gov-style/components/corner_tags).

See [quality_tag.js](https://github.com/GSA/code-gov-style/blob/master/src/quality_tag.js) to view the code for this corner tag component logic.
