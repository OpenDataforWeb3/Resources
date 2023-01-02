# Welcome to the ODC contributing guide
<!-- forked from https://github.com/github/docs/blob/main/CONTRIBUTING.md-->

Thank you for investing your time in contributing to the OpenData Community!  We are using GitHub and git as a part of working in public, together.    

<!--Read our [Code of Conduct](./CODE_OF_CONDUCT.md) to keep our community approachable and respectable. -->

In this guide you will get an overview of the contribution workflow from opening an issue, creating a PR, reviewing, and merging the PR.

## New contributor guide

To get an overview of the project, read the [README](README.md). Here are some resources to help you get started with open source contributions:

- [HackMD - many of our contributors use HackMD to push content to the ODC github] (https://hackmd.io/features)
- [Set up Git](https://docs.github.com/en/get-started/quickstart/set-up-git)
- [GitHub Desktop - GUI git manager](https://desktop.github.com)
- [Visual Studio Code - IDE for editing files](https://code.visualstudio.com)
- [Collaborating with pull requests](https://docs.github.com/en/github/collaborating-with-pull-requests)
- For more information on markdown files, see [the GitHub Markdown reference](https://github.com/github/docs/blob/main/contributing/content-markup-reference.md).


## Getting started

To contribute to the ODC repository, you must be a member of the ODC discord and in good standing. ODC discord members in good standing can be ODC github organization members. This means you will have write access to repositories in the ODC organization. Just ask in the ODC general channel and we will add you as an ODC github organization member.

Find below the types of contributions we encourage.

## Create a new issue

If you want to make a change, [search if an issue already exists](https://docs.github.com/en/github/searching-for-information-on-github/searching-on-github/searching-issues-and-pull-requests#search-by-the-title-body-or-comments). If a related issue doesn't exist, you can open a new issue using a relevant [issue form](https://github.com/opendataforweb3/landscape/issues/new/choose). 

## Solve an issue

Scan through our [existing issues](https://github.com/github/docs/issues) to find one that interests you. You can narrow down the search using `labels` as filters. If you find an issue to work on, assign the issue to yourself, and open a PR with a fix.

## Make changes in the wiki

By default, the wiki allows any github user to read and write. We suggest using the wiki for research you want to share with other members. 

## Make changes in the repository online
Find a file that you want to edit and make changes through the github ODC repository web interface. Follow the branch, commit, and pull request recommendations below. 

## OR Make changes in the repository locally

1. Clone the repository. `NOTE:` If you don't want  to join the discord and be a ODC github organization member, you can still propose changes by forking the repository, making a change on the fork, and submitting the change through a PR.  
- Using GitHub Desktop:
  - [Getting started with GitHub Desktop](https://docs.github.com/en/desktop/installing-and-configuring-github-desktop/getting-started-with-github-desktop) will guide you through setting up Github Desktop.
  - Once Desktop is set up, you can use it to [clone the repo](https://docs.github.com/en/desktop/contributing-and-collaborating-using-github-desktop/cloning-and-forking-repositories-from-github-desktop)!

- OR Using the command line:
  - [Clone the repo](https://www.git-scm.com/docs/git-clone) so that you can make your changes without affecting the original project until you're ready to merge them.

2. Create a working branch and start with your changes. We suggest using a branch name similar to `<user>-<patch><#>`, e.g. sarob-patch01.
3. Make your changes.
   - [Getting started with Visual Studio Code](https://code.visualstudio.com/docs/introvideos/basics) will guide you through setting up VSC.

## Then commit your update

- Commit and push the changes once you are happy with them using an informative message. An issue is optional for a PR, but recommended.  The description field is also optional. If there is an issue, always  add the issue # into either the summary or description field as `#<number>`, e.g. the issue number is 32, so add `#32`.  
- We use repository branch protection rules that require ODC repositories only allow Pull Requests (PR), so Github Desktop will prompt you to create a PR.

## Pull Request

- Don't forget to [link the PR to issue](https://docs.github.com/en/issues/tracking-your-work-with-issues/) if one is available.
Once you submit your PR, a ODC member will review your work. We may ask questions or request additional information.
- `NOTE:` We want work in progress to be updated on the remote (origin) repository at least once day. That way we know you are still working on the changes. Just in case you go offline for awhile, someone else can pick up where you left off. If you are still working on your change, but are not ready for a review, add a comment to the PR saying something like `I am still working on this, but I am sharing as I am going offline for the day`.
- When you are ready for a review, we may ask for changes to be made before a PR can be merged using pull request comments. You can apply suggested changes directly through the UI or locally. Remember to push your local changes again!
- If you run into any merge issues, checkout this [git tutorial](https://github.com/skills/resolve-merge-conflicts) to help you resolve merge conflicts and other issues.

## Your PR is merged!

Congratulations! 

- Once your PR is merged, your contributions will be publicly visible in the repository.  
- If you are updating web content, your commit will cause the published website to be updated. You can check the publishing progress through the repository [Actions](https://github.com/OpenDataforWeb3/Landscape/actions). 
