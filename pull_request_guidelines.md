# Pull request guidelines

Due to our limited resources and in order to give everyone a chance to submit a pull request, we have put restrictions in place this year. If you want to submit a pull request, please take into account the following rules:

0. In general please only work on issues that have been triaged - those are issues with labels such as "high", "medium" or "enhancement". It means an admin looked at it and added it to the backlog.

	1. Bug fixes are always welcome. Start by reviewing the list of bugs with [high priority](https://github.com/laurent22/joplin/issues?utf8=%E2%9C%93&q=is%3Aopen+is%3Aissue+label%3Abug+label%3Ahigh) or [medium priority](https://github.com/laurent22/joplin/issues?utf8=%E2%9C%93&q=is%3Aopen+is%3Aissue+label%3Abug+label%3Amedium).

	2. Alternatively you may look at the [Good first issues](https://github.com/laurent22/joplin/issues?q=is%3Aopen+is%3Aissue+label%3A%22good+first+issue%22).

	3. Also check the backlog of possible [feature requests](https://github.com/laurent22/joplin/issues?q=is%3Aopen+is%3Aissue+label%3Aenhancement). Some of those are complex and not a good fit for a first pull request, but others are more simple so you might want to consider these.

	4. Finally you may implement a plugin in your own repository. Note that we will look at your code, so make sure your choose something not too trivial, so that you can really showcase your skills. Please announce your plugin on the forum, in the [#plugins category](https://discourse.joplinapp.org/c/development/plugins/18).

1. You may not work on issues created by yourself (or your friends). It is likely we will close such issues.

2. Each contributor **may only create one pull request at a time**. Once your pull request has been merged, you can post a second one. We have this rule in place due to our limited resources - if everyone was allowed to post multiple pull requests we will not be able to review them properly. It is also better for you because you only need to care about one PR - so spend time making sure it is as good as it can be - make sure it works well, has test units, documentation and screenshots (if relevant).

3. **All pull request must have test units**. In some cases it might be almost impossible to add such tests (for example integration tests), but for anything else we insist on having them, and we may close the pull request if we see they could have been added but weren't. If you don't know how to add test units, please ask on the forum or Discord. If really it's not possible to add tests, we'll let you know at this point. Also please check again the [Automated Tests](https://github.com/laurent22/joplin/blob/dev/readme/dev/index.md#automated-tests) documentation for more information.

4. AI-assisted contributions must follow the [AI policy](https://github.com/personalizedrefrigerator/gsoc/blob/main/ai_policy.md).

5. **No Work In Progress**. ONLY completed and working pull requests, and with test units, will be accepted. A WIP will be closed immediately.

6. Please **do not `@mention` contributors and mentors and do not ask for pull request reviews**. Sometimes it takes time before we can review your pull request or answer your questions but we'll get to it sooner or later. `@mentioning` someone just adds to the pile of notifications we get and it won't make us look at your issue faster.

7. **Do not force push**. If you make changes to your pull request, please simply add a new commit as that makes it easy for us to review your new changes. If you force push, we'll have to review everything from the beginning.

## PR Description Guidelines

A PR description should explain why the change exists and what it achieves. Its purpose is to reduce the reviewer’s cognitive load, not to narrate the diff. If someone can understand the problem and intent in under a minute, it is doing its job.

### Problem

Start by clearly describing what was broken, missing, or incorrect at a high level. Focus on user-visible behaviour or system impact. Explain the scenario in which the issue occurred and why it matters. Do not begin with implementation details — establish context first.

### Solution

Describe what changed at a high level. Explain the approach taken and why it resolves the problem. The goal is to communicate intent and reasoning, not to restate the diff. Reviewers can read the code for implementation details.

Call out any behavioural changes, side effects, or areas that may require extra attention during review. If the change is low risk, state that clearly.

### Test Plan

Explain how the change was verified. Include manual steps, automated tests, or both. The reviewer should understand how to confirm the fix.
