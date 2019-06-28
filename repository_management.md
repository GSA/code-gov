# Code.gov Repository Management

This is a living document explaining how we collaboratively manage the Code.gov platform repositories. If you’d like to suggest a change, please open an issue for discussion or submit a pull request to the document.

This document covers:

- [Issues](#issues)
  - [Labels](#labels)
  - [Milestones](#milestones)
  - [Triaging Issues](#triaging-issues)
- [Pull Requests](#pull-requests)
  - [Code Review](#code-review)
  - [Design Review](#design-review)
  - [Merging Pull Requests](#merging-pull-requests)
  - [Closing Pull Requests](#closing-pull-requests)

## Issues

A healthy issue list is one where issues are relevant and actionable. *Relevant* in the sense that they relate to the project’s current priorities. *Actionable* in the sense that it’s clear what action(s) need to be taken to resolve the issue.

### Labels

All issues should have [one or more labels] which are lower-case with sentence spacing (no hyphens).

Any issues that are irrelevant or not actionable should be closed, because they get in the way of making progress on the project. Imagine the issue list as a desk: the more clutter you have on it, the more difficult it is to use the space to get work done.

GitHub allows you to assign `labels` to Issues and Pull Requests. For Code.gov repos, we use a standard set of `labels` on all our repos. 

First, we use the label framework needed to tags issues in order for them to show on the Code.gov [Open Tasks page](https://code.gov/open-tasks?page=1&size=10). These labels are outlined in the [helpwanted.md file](./helpwanted.md). 

Our implementation of this includes:

* `[issue-type] bug` - a general bug found in the functionality of your project
* `[issue-type] enhancement` - this label works as a catch all for new features, code cleanup, and general code maintenance. Bugs should not have the enhancement label added to them.
* `[issue-type] good first issue` - some projects are complex. This label will help your new contributors know that this issue is a great way to get involved with your project.
* `[issue-type] feedback` - sometimes you just want to get a different perspective. This label will let your community know that you would like their feedback on a topic.

### Skill Level

There are three levels that we recognize:

* `[skill-level] beginner`
* `[skill-level] intermediate`
* `[skill-level] advanced`

### Effort

Effort is identified by sizes.

* `[effort] small`
* `[effort] medium`
* `[effort] large`


We also have labels to add helpful information related to the status, priority, and functional area of the issue with a few additional misc. labels. These include:

### Priority

Priority is identified by urgency level.

* `[priority] low`
* `[priority] medium`
* `[priority] high`

### Status

Status is identified by workflow progress.

* `[status] needs info` - follow-up required in order to be actionable.
* `[status] blocked`
* `[status] stale` - gives the original author or interested person the opportunity to update before closing
* `[status] changes requested`
* `[status] backlog`
* `[status] in progress` - tracking issues with work in progress
* `[status] needs testing`
* `[status] needs design feedback`

### Inactive

Inactive is identified by the reason an issue will not be worked

* `[inactive] duplicate` - item has already been identified in another issue/PR
* `[inactive] invalid`
* `[inactive] wontfix` - issues/PRs we are (likely) to not implement

### Functional area

Functional area is identified by the subject matter area needed

* `[area] UX`
* `[area] accessibility`
* `[area] docs`
* `[area] code quality`
* `[area] browser compatibility`
* `[area] security`
* `[area] visual design`

In addition to the labels above, we include a few others which are related to specific tools:

* `code.gov` - Used by our API to show on our Open Tasks page 
* `help wanted` - Used by GitHub to indicate how many issues are requesting help from contributors

#### Bulk adding of labels
A list of the labels (with colors) used on Code.gov repos can be found in [repo-labels.json](./repo-labels.json). It can be used in conjunction with a tool like [git-labelmaker](https://github.com/himynameisdave/git-labelmaker#remove-labels) or [git-label-cli](https://github.com/jasonbellamy/git-label-cli) to do a bulk addition of these labels when setting up a new repo.

### Milestones

We put issues into [milestones]() to better categorize them.

### Triaging Issues

To keep the issue list healthy, it needs to be triaged regularly. *Triage* is the practice of reviewing existing issues to make sure they’re relevant, actionable, and have all the information they need.

Anyone can help triage, although you’ll need contributor permission on the Gutenberg repository to modify an issue’s labels or edit its title.

Here are a couple places you can start:

- All issues without an assigned label
- The least recently updated issues

When reviewing issues, here are some steps you can perform:

- First search for duplicates. If the issue is duplicate, close it by commenting with “Duplicate of #<original-id>”, add any relevant new details to the existing issue, and add the `[inactive] duplicate` label.
- If the issue is missing labels, add some to better categorize it (requires proper permissions).
- If the title doesn’t communicate the issue, edit it for clarity (requires proper permissions).
- If it’s a bug report, test to confirm the report or add the `[status] needs testing` label. If there is not enough information to confirm the report, add the `[status] needs info` label and ask for the details needed.
- Remove the `[status] needs info` if the author of the issue has responded with enough details.
- Close the issue with a note if it has a `[status] stale` label but the author didn't respond in 2+ weeks.
- If there was conversation on the issue but no actionable steps identified, follow up with the participants to see what’s actionable.
- If you feel comfortable triaging the issue further, then you can also:
  - Check that the bug report is valid by debugging it to see if you can track down the technical specifics.
  - Check if the issue is missing some detail and see if you can fill in those details. For instance, if a bug report is missing visual detail, it’s helpful to reproduce the issue locally and upload a screenshot or GIF.

## Pull Requests

Code.gov follows a feature branch pull request workflow for all code and documentation changes. At a high-level, the process looks like this:

1. Check out a new feature branch locally.
2. Make your changes, testing thoroughly.
3. Commit your changes when you’re happy with them, and push the branch.
4. Open your pull request.

Along with this process, there are a few important points to mention:

- Non-trivial pull requests should be preceded by a related issue that defines the problem to solve and allows for discussion of the most appropriate solution before actually writing code.
- To make it far easier to merge your code, each pull request should only contain one conceptual change. Keeping contributions atomic keeps the pull request discussion focused on one topic and makes it possible to approve changes on a case-by-case basis.
- Separate pull requests can address different items or todos from their linked issue, there’s no need for a single pull request to cover a single issue if the issue is non-trivial.

### Code Review

Every pull request goes through a manual code review, in addition to automated tests. The objectives for the code review are best thought of as:

- Correct — Does the change do what it’s supposed to?
- Secure — Would a nefarious party find some way to exploit this change?
- Readable — Will your future self be able to understand this change months down the road?
- Elegant — Does the change fit aesthetically within the overall style and architecture?
- Altruistic — How does this change contribute to the greater whole?

*As a reviewer*, your feedback should be focused on the idea, not the person. Seek to understand, be respectful, and focus on constructive dialog.

*As a contributor*, your responsibility is to learn from suggestions and iterate your pull request should it be needed based on feedback. Seek to collaborate and produce the best possible contribution to the greater whole.

### Design Review

If your pull request impacts the design, you can ask for a designer to review. Most pull requests that have an impact on design are reviewed. However, you can request a design review on something by adding the `[status] needs design feedback` label. As a guide, this could be:

- Anything that changes something visually.
- If you just want design feedback on an idea or exploration.

### Merging Pull Requests

A pull request can generally be merged once it is:

- Deemed a worthwhile change to the codebase.
- In compliance with all relevant code review criteria.
- Covered by sufficient tests, as necessary.
- Vetted against all potential edge cases.
- Changelog entries were properly added.
- Reviewed by someone other than the original author.

The final pull request merge decision is made by the core team.

Please make sure to assign each merged pull request to its release milestone. Doing so creates the historical legacy of what code landed when, and makes it possible for all project contributors (even non-technical ones) to access this information.

### Closing Pull Requests

Sometimes, a pull request may not be mergeable, no matter how much additional effort is applied to it (e.g. out of scope). In these cases, it’s best to communicate with the contributor graciously while describing why the pull request was closed, this encourages productive future involvement.

Make sure to:

1. Thank the contributor for their time and effort.
2. Fully explain the reasoning behind the decision to close the pull request.
3. Link to as much supporting documentation as possible.

If you’d like a template to follow:

> Thanks ____ for the time you’ve spent on this pull request.
>
> I’m closing this pull request because ____. To clarify further, ____.
>
> For more details, please see ____ and ____.
