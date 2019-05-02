## OMB M-16-21 Federal Source Code Policy Inventory Requirement

Since the release of the [OMB M-16-21 Federal Source Code Policy (FSCP)](https://code.gov/about/overview/introduction), the U.S. Government (CFO Act agencies) have been focused on completing a comprehensive inventory of all custom developed software from August 2016. Additionally, the Federal agencies have to identify which of those custom developed software can be open source, or be made government wide reuse, or exempt from being release due national security in order to comply with the OMB M-16-21 FSCP. For a full list of requirements please see the [Metadata Schema 2.0.0 ](https://code.gov/about/compliance/inventory-code)requirements.

## Code.gov Metadata Schema 2.0.0 Requirements

The [Code.gov](https://www.code.gov) program and U.S. Government would like to developed a code.json Generator/Scraper tool that would support all GIT version control systems (VCS) and legacy VCS (e.g. SVN, VSS) to capture the software inventory systematically. The main objective is to reduce the manual process, increase efficiency, reduce human error, and standardize the technical solution. To accomplish these objectives we have setup an ongoing working group from the Federal agencies and Open Source Community to support the implementation of the code.json Generator/Scraper tools.

## Generators

Feature             | [Scraper](https://github.com/llnl/scraper) | [Code-JSON Generator](https://github.com/usgs/code-json-generator) |  [Code Inventory Generator](https://github.com/cfpb/code-inventory-generator) | [Code Inventory](https://github.com/GSA/codeinventory) | [Source Code Inventory](https://github.com/HHS/Source-Code-Inventory)
--------------------|-----------------------|-----------------------|-----------------------|-----------------------|-----------------------|
Language            | Python                | Node.js | Node.js | Ruby | TBD |
GitHub.com          | :white_check_mark:    | :white_check_mark: | :white_check_mark: |  :white_check_mark: | :x: |
GitHub Enterprise   | :white_check_mark:    | :white_check_mark: | :white_check_mark: |  :white_check_mark: | :x: |
GitLab.com          | :white_check_mark:    | :white_check_mark: | :x: | :x: | :x: |
GitLab Hosted       | :white_check_mark:    | :white_check_mark: | :x: | :x: | :x: |
Bitbucket.org       | :white_check_mark:    | :x: | :x: |  :x: | :x: |
Bitbucket Server    | :white_check_mark:    | :x: | :x: |  :x: | :x: |
Team Foundation Server (TSF)    | :white_check_mark:    | :x: | :x: |  :x: | :x: |
Labor Hours         | :white_check_mark:    | :x: | :x: | :x: | :x: |
Lead Developer		| [IanLee1521](https://github.com/IanLee1521)	| [emartinez-usgs](https://github.com/emartinez-usgs)	| [contolini](https://github.com/contolini), [Scotchester](https://github.com/Scotchester) | [jfredrickson5](https://github.com/jfredrickson5) | [katucker](https://github.com/katucker) |
Agency					|	DOE-LLNL		|	DOI-USGS  		|	CFPB   	|  GSA	 |  HHS |
GitHub API			| REST API v3		|	REST API v3  | GraphQL API v4 |	REST API v3  | TBD |


## Requirements and Action Items

From the working group session we have captured business needs,  system requirements, and action items for the implementation of the Code-JSON Generator/Scraper Tools.

Please see the full list here: [https://github.com/GSA/code-gov/projects/1](https://github.com/GSA/code-gov/projects/1)

## GSA Code Inventory Tool

The [Code Inventory](https://github.com/GSA/codeinventory) tool is a Ruby gem application that provides basic functionality in a CLI and API, and it can be extended via plug-ins (which are also gems) to support any type of repository
One plug-in we developed is to add GitHub support: [https://github.com/GSA/codeinventory-github](https://github.com/GSA/codeinventory-github)

[New Code Clerk tool](https://github.com/GSA/code-clerk)  
Designed more as an API/SDK, which can power a CLI tool (it does have a basic CLI included)
Designed to be extensible: the user can very finely customize how they want to transform their repository metadata into code.json, but it also comes with easy defaults
Node is more commonly used in web app projects these days, hence the transition to a new language.
Only supports GitHub right now, hard coded, with the intention to make it modular and support any repository
I'm looking forward to working with everyone on Slack to focus our collective efforts!

	Questions:
	How many of you only need a CLI tool?
	How many want the tool to provide an API/SDK?
	By what means should a tool be extensible, and how extensible should it be? Every agency does things differently.
	What kind of flexibility will everyone need? If you really have to use SLOC+COCOMO, consider implementing the formula in a reusable open source library, rather than relying on an external service.

## HHS Source Code Inventory Tool

The basic concept is to add some capabilities to the existing code.json generators, specifically to enable managing metadata for offline repositories (i.e., repos that can't be directly queried by the source code inventory application), and to provide a UI for adjudicating which repos to actually include in the published code.json file.

The proposed implementation uses a GitHub repository and its associated wiki and GitHub Pages website. Entries for the source code inventory are recorded in wiki pages. Client-side Javascript is served through the GitHub Pages site to support proposing entries manually, defining "libraries" of repositories such as GitHub organization accounts that can be queried for automatically proposing entries, reviewing proposed entries, and generating an updated code.json file.

Features proposed for the application and design ideas are documented in the Issues log. The repository's wiki shows a mockup of the inventory representation as individual wiki pages.

## Resources

### Code.gov Schema Documentation

[Metadata Schema 2.0.0](https://code.gov/about/compliance/inventory-code)

### Github API

[REST API v3](https://developer.github.com/v3/) 
[GraphQL API v4](https://developer.github.com/v4/)

### Alternative Hosted GIT based Platforms:  

* [https://bitbucket.org](https://bitbucket.org)  
* [https://about.gitlab.com](https://about.gitlab.com)
