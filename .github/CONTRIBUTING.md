# Contributing to DotVoid

Thanks a lot for contributing to the DotVoid community project!  

In this document, you will find guidelines explaining how to contribute to DotVoid.

## Table of contents

* [Code of conduct](#code-of-conduct)
* [Issues](#issues)
  * [Before submitting an issue](#before-submitting-an-issue)
  * [Issue templates](#issue-templates)
    * [Report](#report)
    * [Support](#ask-for-support)
    * [Request](#request)
* [Code contributions](#code-contributions)
  * [Common practices](#common-practices)
  * [How to make a pull request](#how-to-make-a-pull-request)

## Code of conduct

The [code of conduct](CODE_OF_CONDUCT.md) outlines our expectations for all those who participate in our community, as well as the consequences for unacceptable behavior. Please read it, even if you don't plan on contributing.

## Issues

This section will guide you through the process of reporting a problem, suggest something, or asking for support. Please understand that we need as much information as possible in your report to be able to correctly address it. Be precise.

### Before submitting an issue

Before submitting an issue, please make some research. Check that a similar issue has not been already submited. You may find what you need. Duplicate issues are undesirable.  

If you find an **open** issue similar to your problem, comment it instead of submitting a new one.  
If you find only a **closed** issue similar to your problem, submit a new one including a link to the original issue.

### Issue templates

Issues can be about multiple things: reports, support or requests. Each issue type has its own issue template. Pick the one corresponding to your case and fill it meticulously. You will find guides for each of them below.

* [Report](https://github.com/Nunustolemybike/FreshGanache/issues/new?template=report.md)
* [Support](https://github.com/Nunustolemybike/FreshGanache/issues/new?template=support.md)
* [Request](https://github.com/Nunustolemybike/FreshGanache/issues/new?template=suggestion.md)

Each issue type has specific instructions but all issues have shared requirements:

* **Use a clear and descriptive title.** Don't explain the problem in the title, it's only there to identify it.
* **Write your issues in english with a correct grammar and spelling.**
* **Don't hesitate to use [markdown](https://guides.github.com/features/mastering-markdown/)** to improve the presentation of your issue, highlight important things and improve readability. Any line of code should be inside a code format.

#### Report

Use this template if you want to report a typo, a bad sentence, a formatting problem or incorrect information. Describe the problem and suggest a fix.

#### Ask for support

To ask for support, please use the [Support issue template](https://github.com/Nunustolemybike/FreshGanache/issues/new?template=support.md).

Here are the specific requirements for support issues:

* **Describe precisely what you are trying to achieve.** We need to understand exactly what you want to do to be able to understand the problem.
* **Provide us with the relevant markup.** Show us the what you struggle to make working.
* **Include the branch and the commit hash** to let us know where you are located on the source control. Take this opportunity to check if you're up to date on this branch.

#### Request

To suggest a new section or enhancement, please use the [request issue template](https://github.com/Nunustolemybike/FreshGanache/issues/new?template=suggestion.md).

Enhancements suggestions include completely new chapters, minor improvements, visual changes, ...

Here are the specific requirements for suggestions:

* **Explain the aim of your suggestion.** What should it be used for? What would it bring? Why would it be a good change?

## Code contributions

### Common practices

#### Git

We are using a variant of **GitFlow**. You can learn more about it [here](https://datasift.github.io/gitflow/IntroducingGitFlow.html).  
Our approach differs by the fact we are not using release branches as we will not support multiple versions at once. The `develop` branch is the place where everything done in a traditional git flow will be done.  

You can rebase on your personal feature branches. Please make sure you don't break *the golden rule of rebasing*: "Never rebase while you're on a public branch.".  
Accepted pull requests are **merged** into the `develop` branch. 

The following naming is used for branches:

* `feature/<feature_name>`: branches containing full chapters or feature. Checked out from `develop`.
* `hotfix/<feature_name>`: branches containing hotfixes. Checked out from `master`. They will be merged both in `master` and `develop`.
* `meta/<meta_name>`: branches containing meta changes. Meta is readmes, documentation, contribution guidelines, etc. 

**We use the Github process**. Each task is linked to an issue and added to a *Github Project*. Applicable labels will be added.    

A **commit** should contain only one fully completed change. Unrelated changes should be in separate commits, making them atomic.  

**Messages:**  

* Use the present tense with the imperative mood. (Example: "*Move logic from X to Y*")
* The first line must not exceed 72 characters. Add a blank line after it.
* If your commit is related to one or more issue(s), refer them on the third line (after the blank line).
* Add a clear description. Don't overdetail as the literal changes are also visible directly. The reader should understand what has changed and how it defers from the previous implementation.

### How to make a pull request

Pull requests are the way for everyone to add their code into the project.  
All pull requests, if approved, are merged into **`develop`**.

To submit a pull request, please follow these instructions:

* Fill the [pull request template](PULL_REQUEST_TEMPLATE.md).
* **Describe the benefits of your changes.**
* **Describe the possible drawbacks and/or caveats of your changes.**
* If you want to include one or more issue numbers, **don't add them to the title**: use the appropriate section from the pull request template instead.
* If your pull request contains visual changes, **include screenshots**. Ideally, include a "before-after" screenshot too.

Any pull request which doesn't comply with these rules will be ignored and closed.
