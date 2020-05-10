# code-gov

Welcome! This repository is a collection point for all [Code.gov](https://code.gov) repositories.

## Code.gov

[Code.gov](https://code.gov) is a program and technical platform with a website and API promoting good practices in code development, collaboration, and reuse across the U.S. Federal Government. Code.gov provides tools and guidance to help federal agencies implement the [Federal Source Code Policy (FSCP)](https://code.gov/about/overview/introduction). Code.gov aggregates an inventory of the federal government's custom code to promote reuse between federal agencies. Code.gov provides tools to help the government and the public collaborate on open source projects.

You can read the original White House FSCP [announcement](https://www.whitehouse.gov/blog/2016/08/08/peoples-code) and [Code.gov announcement](https://obamawhitehouse.archives.gov/blog/2016/11/03/peoples-code-now-codegov).

## Repositories

All of our work is open source and we encourage you to take a look and contribute to our projects by submitting a pull request, a Github issue, or commenting on existing issues and pull requests. If you are unsure as to where an issue should live, please use the [GSA/code-gov](https://github.com/GSA/code-gov) repo as a catch all.

All of our repositories follow our [Code of Conduct](CODE_OF_CONDUCT.md) and [Contributing](CONTRIBUTING.md) guidelines.

### Code.gov repositories

Code.gov consists of multiple repositories containing code and information.

<details>
  <summary>Front-end - Repositories related to the website with user-facing interactions for the platform.</summary>
    
| Project                                                                       | Description | Issues                                                                   | New Issue                                                                       |
| ----------------------------------------------------------------------------- | ------ | ------------------------------------------------------------------------ | ------------------------------------------------------------------------------- |
| [GSA/cautious](https://github.com/GSA/cautious)                   | Utility Functions in JavaScript to clean up messy data aggregated from federal agency code.json files for Code.gov.| [View all issues](https://github.com/GSA/cautious/issues)          | [Create a new issue](https://github.com/GSA/cautious/issues/new/choose) |
| [GSA/code-gov-api-client](https://github.com/GSA/code-gov-api-client)                       | Program used by the Code.gov front-end for interacting with the Code.gov API. | [View all issues](https://github.com/GSA/code-gov-api-client/issues)            | [Create a new issue](https://github.com/GSA/code-gov-api-client/issues/new/choose)            |
| [GSA/code-gov-data](https://github.com/GSA/code-gov-data)                   | Program for updating the Code.gov schema with filters used by the Code.gov front-end. | [View all issues](https://github.com/GSA/code-gov-data/issues)          | [Create a new issue](https://github.com/GSA/code-gov-data/issues/new) |
| [GSA/code-gov-font](https://github.com/GSA/code-gov-font)                   |Custom font with icons used by the Code.gov front end.| [View all issues](https://github.com/GSA/code-gov-font/issues)          | [Create a new issue](https://github.com/GSA/code-gov-font/issues/new)   |
| [GSA/code-gov-front-end](https://github.com/GSA/code-gov-front-end)                       | Our frontend project, currently deployed as a static site which renders [Code.gov](https://code.gov/), this project is backed by our API to display project repositories, search, and an agency compliance dashboard. | [View all issues](https://github.com/GSA/code-gov-front-end/issues)            | [Create a new issue](https://github.com/GSA/code-gov-front-end/issues/new/choose)            |
| [GSA/code-gov-site-map-generator](https://github.com/GSA/code-gov-site-map-generator)                   |Generates sitemap.xml for Code.gov in production environment. | [View all issues](https://github.com/GSA/code-gov-site-map-generator/issues)          | [Create a new issue](https://github.com/GSA/code-gov-site-map-generator/issues/new/choose) |
| [GSA/code-gov-style](https://github.com/GSA/code-gov-style)                   | Our effort to modularize our CSS styles. This project is also made available as a [NPM package](https://www.npmjs.com/package/@code.gov/code-gov-style) and [jekyll site](https://gsa.github.io/code-gov-style/). | [View all issues](https://github.com/GSA/code-gov-style/issues)          | [Create a new issue](https://github.com/GSA/code-gov-style/issues/new/choose)          |
</details>
<details>
  <summary>Back-end - Repositories related to the API with data harvesting and delivery for the platform.</summary>

| Project                                                                       | Description | Issues                                                                   | New Issue                                                                       |
| ----------------------------------------------------------------------------- | ------ | ------------------------------------------------------------------------ | ------------------------------------------------------------------------------- |
| [GSA/code-gov-api](https://github.com/GSA/code-gov-api)                       | Our backend API. An Express.js app backed by Elasticsearch. Its primary function is to index and make America's source code discoverable and searchable. | [View all issues](https://github.com/GSA/code-gov-api/issues)            | [Create a new issue](https://github.com/GSA/code-gov-api/issues/new/choose)            |
| [GSA/code-gov-adapters](https://github.com/GSA/code-gov-adapters)             | Our attempt to extract all data adapters into a simple reusable project. We currently use this Elasticsearch adapter. This project is also made available as a [NPM package](https://www.npmjs.com/package/@code.gov/code-gov-adapter) | [View all issues](https://github.com/GSA/code-gov-adapters/issues)       | [Create a new issue](https://github.com/GSA/code-gov-adapters/issues/new/choose)       |
| [GSA/code-gov-harvester](https://github.com/GSA/code-gov-harvester)           | Our standalone source code inventory harvester. | [View all issues](https://github.com/GSA/code-gov-harvester/issues)      | [Create a new issue](https://github.com/GSA/code-gov-harvester/issues/new/choose)      |
| [GSA/code-gov-integrations](https://github.com/GSA/code-gov-integrations)     | This project contains all of our third party integrations. Currently Github integration is the only one implemented. This project is also made available as a [NPM package](https://www.npmjs.com/package/@code.gov/code-gov-integrations) | [View all issues](https://github.com/GSA/code-gov-integrations/issues)   | [Create a new issue](https://github.com/GSA/code-gov-integrations/issues/new/choose)   |
| [GSA/code-gov-validator](https://github.com/GSA/code-gov-validator)     | Schema validation package for Code.gov. | [View all issues](https://github.com/GSA/code-gov-validator/issues)   | [Create a new issue](https://github.com/GSA/code-gov-validator/issues/new/choose)   |
</details>  

<details>
  <summary>Tools - Projects we have created in order to better aid our work on the code.gov platform. They do not affect the development or deployment of our main repositories.</summary>

| Project                                                                                       | Description                                                                                                                                                                                                      | Issues                                                                           | New Issue                                                                                   |
| --------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------- |
| [GSA/code-gov-converter](https://github.com/GSA/code-gov-converter)  | Converts publiccode.yml to code. json. | [View all issues](https://github.com/GSA/code-gov-converter/issues)              | [Create a new issue](https://github.com/GSA/code-gov-converter/issues/new)                  |
| [GSA/code-gov-github-metrics](https://github.com/GSA/code-gov-github-metrics)                 | This project compiles and calculates GitHub metrics across the different Code.gov repos so we can understand and track community contributions over time. | [View all issues](https://github.com/GSA/code-gov-github-metrics/issues)         | [Create a new issue](https://github.com/GSA/code-gov-github-metrics/issues/new)             |
| [GSA/code-gov-open-source-toolkit](https://github.com/GSA/code-gov-open-source-toolkit)       | This is a government-wide project facilitated by the Code.gov team to produce a toolkit pertaining to open sourcing software.                                                                 | [View all issues](https://github.com/GSA/code-gov-open-source-toolkit/issues)    | [Create a new issue](https://github.com/GSA/code-gov-open-source-toolkit/issues/new/choose) |
| [GSA/code-gov-repo-template](https://github.com/GSA/code-gov-repo-template)                   | A basic template to use for all code.gov repositories which includes our standard documents and contact info. Using this as a base ensures that all of our community standards are followed.                     | [View all issues](https://github.com/GSA/code-gov-repo-template/issues)          | [Create a new issue](https://github.com/GSA/code-gov-repo-template/issues/new/choose)       |
| [GSA/code-gov-verify-agency-jsons](https://github.com/GSA/code-gov-verify-agency-jsons)       | This a utility project, used in conjuction with code-gov-harvester and can help users find various statistics of repositories imported into the Code.gov platform.                                                          | [View all issues](https://github.com/GSA/code-gov-verify-agency-jsons/issues)    | [Create a new issue](https://github.com/GSA/code-gov-verify-agency-jsons/issues/new)        |


</details>
<details>
  <summary>Deprecated repositories - Repositories that were previously used by the Code.gov team but are no longer in use.</summary>

| Project                                                                                   | Description                                                                                     | Reason for deprecation                                                                                                                                                  |
| ----------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [GSA/code-gov-about-page](https://github.com/GSA/code-gov-about-page)                     | Component for the About page on [Code.gov](https://code.gov).                                   | The about page component was integrated directly into [GSA/code-gov-front-end](https://github.com/GSA/code-gov-front-end) in order to simplify the site architecture.   |
| [GSA/code-gov-admintool](https://github.com/GSA/code-gov-admintool)                       | This repository contains the source code for the frontend of the Code.gov Admin Tool.           | The Admin Tool is no longer in use.      |
| [GSA/code-gov-admin-backend](https://github.com/GSA/code-gov-admin-backend)               | This repository contains the source code for backend of the Code.gov Admin Tool.                | The Admin Tool is no longer in use.             |
| [GSA/code-gov-coding-languages](https://github.com/GSA/code-gov-coding-languages)         | Standard List of Coding Languages used by Code.gov.                                             | The project is no longer in use.   |
| [GSA/code-gov-data-quality-poc](https://github.com/GSA/code-gov-data-quality-poc)         | Code.gov data quality scoring proof of concept.                                                 | The project was a proof of concept and is no longer in use.  |
| [GSA/code-gov-developer-docs](https://github.com/GSA/code-gov-developer-docs) | Our developer docs! This repo is meant to be a simple way to start using our API. | Documentation is now hosted at https://open.gsa.gov/api/codedotgov/  |
| [GSA/code-gov-fscp-react-component](https://github.com/GSA/code-gov-fscp-react-component) | Federal Source Code Policy (FSCP) plugin for code-gov-front-end, built with Markdown and React. | The FSCP is hosted at [https://sourcecode.cio.gov/](https://sourcecode.cio.gov/) and it was therefore duplicative for it to be on [Code.gov](https://code.gov) as well. |
| [GSA/code-gov-gitsecretpatterns](https://github.com/GSA/code-gov-gitsecretpatterns)       | Repository for Code.gov git-secrets patterns and bootstrap script.                              | The project is no longer in use.  |
| [GSA/code-gov-harvester-deprecated](https://github.com/GSA/code-gov-harvester-deprecated) | The old version of the harvester that harvests and processes code.json files from agencies.     | The new harvester repo is [GSA/code-gov-harvester](https://github.com/GSA/code-gov-harvester).  |
| [GSA/code-gov-repos-parser](https://github.com/GSA/code-gov-repos-parser)                 | Parse out information from code.gov repos.                                                      | The project is no longer in use.    |
| [GSA/code-gov-stats](https://github.com/GSA/code-gov-stats)                               | A simple app to extract stats about repositories using the Github API and Cloc                  | The project is no longer in use.  |
| [GSA/code-gov-stats-jupyter-notebook](https://github.com/GSA/code-gov-stats-jupyter-notebook) | Extract some stats for Code.gov using the Github GraphQL API. | Repo no longer in use for pulling Code.gov stats.                           |
| [GSA/code-gov-web](https://github.com/GSA/code-gov-web)                                   | The old version of the [Code.gov](https://code.gov) front end                                   | The front end stack was changed from Angular to React. The new front end repo is [GSA/code-gov-front-end](https://github.com/GSA/code-gov-front-end).  |
| [GSA/compliance-dashboard-web-component](https://github.com/GSA/compliance-dashboard-web-component)                   |Reusable compliance dashboard web component| Repo no longer in use. Web component integrated into [GSA/code-gov-front-end](https://github.com/GSA/code-gov-front-end). |
| [GSA/json-schema-validator-web-component](https://github.com/GSA/json-schema-validator-web-component)     |Web Component that Displays a JSON File and Validates it based on a Schema| Web component for validating code.json schema. 
A new version will be incorporated into the front-end in the future.   |
| [GSA/json-schema-web-component](https://github.com/GSA/json-schema-web-component)     | Web Component that Displays a JSON Schema consumed by the front end| Integrated into Code.gov front-end as a React component |



</details>  

## Files you'll find in this repo

These files offer information for federal agencies of how to inventory code and place on Code.gov.

- [Federal Source Code CoP Meeting Minutes](./docs/CoPMeetingMins): This folder contains the notes from our monthly Community of Practice meetings.
- [Federal Source Code Study](./docs/FederalSourceCodeStudy): This folder contains the Federal Source Code Study (FSCS) and summary documents to be used for upcoming blog posts.
- [Metadata Schema](./docs/MetadataSchema): This folder contains the notes from our metadata schema workgroup meetings.
- [UX](./docs/UX): This folder contains Code.gov UX personas.
- [code_json_generators.md](./docs/code_json_generators.md): A comparison table of code.json generator tools.
- [data_quality_scoring.md](./docs/data_quality_scoring.md): Info on how the Code.gov data quality scores are determined.
- [front_end_guidelines.md](./docs/front_end_guidelines.md): General guidance to follow when developing on the front end.
- [help_wanted.md](./docs/help_wanted.md): Detailed info on our Open Tasks (formerly Help Wanted) and the labels projects need to use in order to display these on code.gov.
- [infrastructure.md](./docs/infrastructure.md): Description of the infrastructure, server space and memory, required to run code.gov. It breaks down the server requirements by front-end and different back-end processes.
- [labor_hour_calc.md](./docs/labor_hour_calc.md): Guidance on how agencies can calculate labor hours on open source projects.
- [metadata_examples.md](./docs/metadata_examples.md): A showcase of good examples of metadata in current agency code.json files.
- [procedures.md](./docs/procedures.md): Administrative procedures for the Code.gov team
- [repo-labels.json](./docs/repo-labels.json): A json file that can be used to add the specific GitHub issue labels code.gov uses on their projects.
- [repository_management.md](./docs/repository_management.md): This living document explains how we collaboratively manage the Code.gov platform repositories.

## Questions?

If you have questions, please feel free to contact us.

- [Open an issue](https://github.com/GSA/code-gov/issues/new)
- [LinkedIn](https://www.linkedin.com/company/code-gov/)
- [Twitter](https://twitter.com/@CodeDotGov)
- [Email](mailto:code@gsa.gov)
- Join our `#opensource-public` channel on Slack: https://chat.18f.gov/
