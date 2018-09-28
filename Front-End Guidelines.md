## Front-End Guidelines for Code.gov

*This document is a living document. We welcome your contributions. Start a conversation with a [Pull Request](https://github.com/GSA/code-gov-web/compare) or by submitting an [Issue](https://github.com/GSA/code-gov-web/issues/new)*

- These are guidelines, not rules. There will be exceptions.
- Favor CSS over JavaScript because:
  - CSS requires a less complicated build process to maintain
  - We can easily test and build upon it in the browser
- Create web components for parts of the site that are used more than once, are static and don’t emit many events because web components can:
  - fit in one file
  - run on any framework
  - display easily on our style guide, like the banner
- Only create framework-dependent components for parts of the site that are complicated and emit events
  - Leverage the framework’s strengths in organizing event handling and dynamic rendering
- Only load a polyfill if it is needed
- Favor 508 compliance and accessibility 
  - Limit bandwidth usage as much as possible by moving complex filtering to our API
  - Reduce load times to better serve low bandwidth users
  - Refactor our UI / UX to be 508 compliant
