## OMB M-16-21 Federal Source Code Policy Inventory Requirement

Since the release of the [OMB M-16-21 Federal Source Code Policy (FSCP)](https://code.gov/#/policy-guide/policy/introduction), the U.S. Government (CFO Act agencies) have been focused on completing a comprehensive inventory of all custom developed software from August 2016. Additionally, the Federal agencies have to identify which of those custom developed software can be open source, or be made government wide reuse, or exempt from being release due national security in order to comply with the OMB M-16-21 FSCP. For a full list of requirements please see the [Metadata Schema 2.0.0 ](https://code.gov/#/policy-guide/docs/compliance/inventory-code)requirements.

## Code.gov Metadata Schema 2.0.0 Requirements

The [Code.gov](https://www.code.gov) program and U.S. Government would like to developed a code.json Generator/Scraper tool that would support all GIT version control systems (VCS) and legacy VCS (e.g., SVN, VSS) to capture the software inventory systematically. The main objective is to reduce the manual process, increase efficiency, reduce human error, and standardize the technical solution. To accomplish these objectives we have setup an ongoing working group from the Federal agencies and Open Source Community to support the implementation of the code.json Generator/Scraper tools.

## Generators

Feature             | [Scraper](https://github.com/llnl/scraper) | [Code-JSON Generator](https://github.com/usgs/code-json-generator) |  [Code-Inventory Generator](https://github.com/GSA/codeinventory-github) | [Code Inventory](https://github.com/GSA/codeinventory) | [Source Code Inventory](https://github.com/HHS/Source-Code-Inventory)
--------------------|-----------------------|-----------------------|-----------------------|-----------------------|-----------------------|
Language            | Python                | Node.js | Ruby | Ruby | TBD |
GitHub.com         | :white_check_mark:    | :white_check_mark: | :white_check_mark: |  :white_check_mark: | :x: |
GitLab.com         | :white_check_mark:    | :white_check_mark: | :x: | :x: | :x: |
Bitbucket.org      | :white_check_mark:    | :x: | :x: |  :x: | :x: |
Labor Hours        | :white_check_mark:    | :x: | :x: | :x: | :x: |
Lead Developer		| [IanLee1521](https://github.com/IanLee1521)	| [emartinez-usgs](https://github.com/emartinez-usgs)	| [contolini](https://github.com/contolini) | [jfredrickson5](https://github.com/jfredrickson5) | [katucker](https://github.com/katucker) |
Agency					|	DOE-LLNL		|	DOI-USGS  		|	CFPB   	|  GSA	 |  HHS |
GitHub API			| REST API v3		|	REST API v3  | GraphQL API v4 |	REST API v3  | TBD |


## Requirements and Action Items

From the working group session we have captured business needs,  system requirements, and action items for the implementation of the Code-JSON Generator/Scraper Tools.

Please see the full list here: [https://github.com/GSA/code-gov/projects/1](https://github.com/GSA/code-gov/projects/1)

## Resources
[Metadata Schema 2.0.0](https://code.gov/#/policy-guide/docs/compliance/inventory-code)

REST API v3 | [https://developer.github.com/v3/]()  
GraphQL API v4 | [https://developer.github.com/v4/]()

Alternative GIT based Platforms:  
[https://bitbucket.org](https://bitbucket.org)  
[https://about.gitlab.com](https://about.gitlab.com)
