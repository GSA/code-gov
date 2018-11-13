# code-gov

Welcome! This is an informative repository for all Code.gov repositories.

## What is Code.gov

[Code.gov](https://code.gov) is a website and program promoting good practices in code development, collaboration, and reuse across the U.S. Federal Government. [Code.gov](https://code.gov) will provide tools and guidance to help federal agencies implement the [Federal Source Code Policy](https://code.gov/#/policy-guide/policy/introduction). It will include an inventory of the federal government's custom code to promote reuse between federal agencies. Also, [Code.gov](https://code.gov) will provide tools to help the government and the public collaborate on open source projects.

To learn more about the project, check out this [blog post](https://www.whitehouse.gov/blog/2016/08/08/peoples-code).

All of [Code.gov's](https://code.gov) repositories are open source, we invite your contributions be it in the form of code, design, issues, or ideas.

## Repositories

As a product, [Code.gov](https://code.gov) is a collection of repositories that enable the aggregation of source code inventory files. All of our work is open source and we encorage you to take a look and, if you wish, contribute to our projects by submitting a pull request, a Github Issue, or commenting on existing issues and pull requests.

All of our repositories follow our [Code of Conduct](CODE_OF_CONDUCT.md) and [Contributing](CONTRIBUTING.md) guidelines.

### Main repositories

1. [GSA/code-gov-web](https://github.com/GSA/code-gov-web): Our frontend project. Currently deployed as a static site, this project is backed by our API to display project repositories, search, and an agency compliance dashboard.
2. [GSA/code-gov-api](https://github.com/GSA/code-gov-api): Our backend API. An Express.js app backed by Elasticsearch. Its primary function is to index and make America's source code discoverable and searchable.
3. [GSA/code-gov-harvester](https://github.com/GSA/code-gov-harvester): Our standalone source code inventory harvester.
4. [GSA/code-gov-developer-docs](https://github.com/GSA/code-gov-developer-docs): Our developer docs! This repo is meant to be a simple way to start using our API. It can also provide API tokens. The live site can be seen [here](https://developers.code.gov).
5. [GSA/code-gov-style](https://github.com/GSA/code-gov-style): Our effort to modularize our CSS styles. This project is also made available as a [NPM package](https://www.npmjs.com/package/@code.gov/code-gov-style).
6. [GSA/code-gov-adapters](https://github.com/GSA/code-gov-adapters): Our attempt to extract all data adapters into a simple reusable project. Currently only an Elasticsearch adapter has been implemented but more are on our roadmap. This project is also made available as a [NPM package](https://www.npmjs.com/package/@code.gov/code-gov-adapter)
7. [GSA/code-gov-validator](https://github.com/GSA/code-gov-validator): Project that validates the structure of code.json files and returns all errors, warnings, and enhancements. This project is also made available as a [NPM package](https://www.npmjs.com/package/@code.gov/code-gov-validator)
8. [GSA/code-gov-integrations](https://github.com/GSA/code-gov-integrations): This project contains all of our third party integrations. Currently Github integration is the only one implemented but more are on our roadmap. This project is also made available as a [NPM package](https://www.npmjs.com/package/@code.gov/code-gov-integrations)

### Miscellaneous Repositories

These repos are marked as miscellaneous because they do not affect the development or deployment of our main repos.

1. [GSA/code-gov-stats](https://github.com/GSA/code-gov-stats)
2. [GSA/code-gov-stats-jupyter-notebook](https://github.com/GSA/code-gov-stats-jupyter-notebook)

## Communications

As an open source project we love feedback. If you want to get a hold of us you can use one of the following ways:

1. Twitter: [@CodeDotGov](https://twitter.com/CodeDotGov)
2. Email: [code@gsa.gov](mailto://code@gsa.gov)
3. LinkedIn: [code-gov](https://www.linkedin.com/company/code-gov/)

## Contribute

You can contribute to any of our open source projects by submitting a pull request, an issue, or giving general feedback.
We handle all these via Github Issues in their respective project, but if you are unsure as to where an issue should live
please use the [GSA/code-gov](https://github.com/GSA/code-gov) repo as a catch all.

| Project                                                                       | Issues                                                                   | New Issue                                                                       |
| ----------------------------------------------------------------------------- | ------------------------------------------------------------------------ | ------------------------------------------------------------------------------- |
| [GSA/code-gov](https://github.com/GSA/code-gov)                               | [View all issues](https://github.com/GSA/code-gov/issues)                | [Create a new issue](https://github.com/GSA/code-gov/issues/new)                |
| [GSA/code-gov-web](https://github.com/GSA/code-gov-web)                       | [View all issues](https://github.com/GSA/code-gov-web/issues)            | [Create a new issue](https://github.com/GSA/code-gov-web/issues/new)            |
| [GSA/code-gov-api](https://github.com/GSA/code-gov-api)                       | [View all issues](https://github.com/GSA/code-gov-api/issues)            | [Create a new issue](https://github.com/GSA/code-gov-api/issues/new)            |
| [GSA/code-gov-api-client](https://github.com/GSA/code-gov-api-client)                       | [View all issues](https://github.com/GSA/code-gov-api-client/issues)            | [Create a new issue](https://github.com/GSA/code-gov-api-client/issues/new)            |
| [GSA/code-gov-font](https://github.com/GSA/code-gov-font)                   | [View all issues](https://github.com/GSA/code-gov-font/issues)          | [Create a new issue](https://github.com/GSA/code-gov-font/issues/new)   
| [GSA/code-gov-harvester](https://github.com/GSA/code-gov-harvester)           | [View all issues](https://github.com/GSA/code-gov-harvester/issues)      | [Create a new issue](https://github.com/GSA/code-gov-harvester/issues/new)      |
| [GSA/code-gov-developer-docs](https://github.com/GSA/code-gov-developer-docs) | [View all issues](https://github.com/GSA/code-gov-developer-docs/issues) | [Create a new issue](https://github.com/GSA/code-gov-developer-docs/issues/new) |
| [GSA/code-gov-style](https://github.com/GSA/code-gov-style)                   | [View all issues](https://github.com/GSA/code-gov-style/issues)          | [Create a new issue](https://github.com/GSA/code-gov-style/issues/new)          |
| [GSA/code-gov-adapters](https://github.com/GSA/code-gov-adapters)             | [View all issues](https://github.com/GSA/code-gov-adapters/issues)       | [Create a new issue](https://github.com/GSA/code-gov-adapters/issues/new)       |
| [GSA/code-gov-validator](https://github.com/GSA/code-gov-validator)           | [View all issues](https://github.com/GSA/code-gov-validator/issues)      | [Create a new issue](https://github.com/GSA/code-gov-validator/issues/new)      |
| [GSA/code-gov-integrations](https://github.com/GSA/code-gov-integrations)     | [View all issues](https://github.com/GSA/code-gov-integrations/issues)   | [Create a new issue](https://github.com/GSA/code-gov-integrations/issues/new)   |
| [GSA/json-schema-web-component](https://github.com/GSA/json-schema-web-component)     | [View all issues](https://github.com/GSA/json-schema-web-component/issues)   | [Create a new issue](https://github.com/GSA/json-schema-web-component/issues/new)   |
| [GSA/json-schema-validator-web-component](https://github.com/GSA/json-schema-validator-web-component)     | [View all issues](https://github.com/GSA/json-schema-validator-web-component/issues)   | [Create a new issue](https://github.com/GSA/json-schema-validator-web-component/issues/new)   |

## Thanks!
