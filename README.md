# GuidesforRepos

GuidesforRepos is a simple, but helpful guide for writting issues' and PRs' titles in an efficient way. Following that guide cleans up your very long list of issues and PRs by making it simpler for maintainers to identify the type of the issue or PR at a glance and invovle, moderate and help faster.

:information_source: GitHub does not render icons in titles just by writing the icon's code in `:`, as it does with comments. You have to mark the icon manually, copy it and then paste it in the title. 

#### Issues

When creating an issue, provide in title a simple and brief resume of the problem. In addintion, include a  github image, followed by a label, before the title's text as it is shown below (more than one may be added):

Image                  | Labels         | Type
---------------------- | -------------- | ----
:fast_forward:         | [Prog]         | In progress
:rocket:               | [Speed]        | Enhancement
:heart:                | [Prop]         | Propose a new feature
:older_man:            | [Dprc]         | Something used is deprecated
:warning:              | [Warn]         | Something may break in the future, needs to be changed
:yin_yang:             | [Semi]         | Something breaks in some systems (not in all of them)
:exclamation:          | [Bug]          | Bug
:question:             | [WhatIf]       | Not sure if bug
:imp:                  | [BadOldFriend] | Old issue appeared again
:hand:                 | [Help]         | Help needed from other contributors of this project
:call_me_hand:         | [Call]         | Help needed from contributors of another project that creates the problem
:martial_arts_uniform: | [BigBro]       | Repo's owner attention is required (use it with caution)



#### PRs

As with issues, when you first create a PR, you have to provide a corresponding icon, followed by a label, before the title's text, following the rules below.

Image               | Labels    | Type
------------------- | --------- | ----
:hammer_and_wrench: | [WIP]     | Work still in progress
:call_me_hand:      | [Help]    | Help needed for this PR
:label:             | [Approve] | Submitted for approval (must not be in "work-in-progress" state)



### For maintainers and moderators

#### Merging

When you comment your commit before merging a new PR, you should provide a label before your message of preference under these rules:

Label          | Type
-------------- | ----
[Fix]          | PR fixes something
[Feat]         | Enhancement
[FeatAdd]      | New feature added
[Update]       | Updated a deprecated package or method

and in addition, depending on the influence of the PR

[M] or [Maj]   | Major patch/Breaks backwards compatibility 
[S] or [Small] | Small patch

It's a good practice to provide the influence of the PR first. If the PR consists of multiple types, provide each type in the row and separate each corresponding message with `|`

Example: `[S][Fix][Update] #643|PackageName to v6.4.3`