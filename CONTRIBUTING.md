# **Company Name** CONTRIBUTING.md

This document includes instructions on best practices and recommendations to follow when using the **Company Name** GitHub account. These instructions are separated by subject matter. For the repository owner, contribution guidelines explain how people should make contributions to the repository. For contributors, the guidelines help verify that they're submitting well-formed pull requests and opening useful issues. For both, contribution guidelines save time and hassle caused by improperly created pull requests or issues that have to be rejected and re-submitted. See the [Table of Contents](#table-of-contents) for different sections of best practice. Please make sure to read the relevant sections before making contributions, both for security and for efficiency purposes. 


## Table of Contents
- 
- [Identity and Access Management](#identity-and-access-management)
- [Security Tools](#security)
- [Code Alterations](#code-alterations)
- [Communication](#communication)


## New contributor guide

Here are some resources to help you get started with GitHub contributions:
- [Set up Git](https://docs.github.com/en/get-started/quickstart/set-up-git)
- [GitHub flow](https://docs.github.com/en/get-started/quickstart/github-flow)
- [Collaborating with pull requests](https://docs.github.com/en/github/collaborating-with-pull-requests)


## Getting started

### Commit Formatting
A commit is a discrete change to one or more files that you have write permissions to. These changes are recorded in the local repository. Commits should be made only after testing the code. Make small changes and commit the code often to a branch. Include short, detailed descriptions in Update box of the changes made, and give the update title a distinctive name. This will launch a pull request to the code owner or administrator, who will decide whether or not to approve the change.

<img width="878" alt="image" src="https://user-images.githubusercontent.com/123562599/216442741-3b9ff3e3-2bf2-4b6d-b4a6-2cf827fd3bf0.png">

### Pull Request Formatting 
A pull request is a request to merge one or more commits into a different branch, "pulling" from a local repository into the remote repository. When a commit is made, the user is redirected to a page to generate a pull request for the changes. The title and description from the commit should carry over into the pull request. 

<img width="673" alt="PullRequest" src="https://user-images.githubusercontent.com/123562599/216445549-53850274-15cc-4d9a-920f-6543b6a59dd6.png">

### Pull Request-Merge Formatting

Pull requests can have "required reviews", which need a specific number of "Approve" reviews from people with write or admin permissions in the repository before they can be merged. For those with elevated permissions in the organization, pull requests can be seen in the "Pull requests" Tab. Code scanning using CodeQL should be done at this phase as well, and passed or failed checks are visible in this menu. 

<img width="611" alt="PullRequestMerge" src="https://user-images.githubusercontent.com/123562599/216447456-d5b0ff94-1e26-4bd1-8b89-2ad35180d0eb.png">

The administrator whose reviews are needed can: 
 - Comment: leaving general feedback without specific approval
 - Approve: Submit feedback and approve merging these changes
 - Request Changes: Submit feedback that must be addressed before merging

Further information about approving Pull Requests can be found [here](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/reviewing-changes-in-pull-requests/approving-a-pull-request-with-required-reviews).

![image](https://user-images.githubusercontent.com/123562599/216451795-62dc666b-c449-4eac-ac27-a4edf65dc7bc.png)


### Branching














### Make Changes

#### Make changes in the UI

Click **Make a contribution** at the bottom of any docs page to make small changes such as a typo, sentence fix, or a broken link. This takes you to the `.md` file where you can make your changes and [create a pull request](#pull-request) for a review. 

 <img src="./assets/images/contribution_cta.png" width="300" height="150" /> 

#### Make changes in a codespace

For more information about using a codespace for working on GitHub documentation, see "[Working in a codespace](https://github.com/github/docs/blob/main/contributing/codespace.md)."

#### Make changes locally

1. Fork the repository.
- Using GitHub Desktop:
  - [Getting started with GitHub Desktop](https://docs.github.com/en/desktop/installing-and-configuring-github-desktop/getting-started-with-github-desktop) will guide you through setting up Desktop.
  - Once Desktop is set up, you can use it to [fork the repo](https://docs.github.com/en/desktop/contributing-and-collaborating-using-github-desktop/cloning-and-forking-repositories-from-github-desktop)

- Using the command line:
  - [Fork the repo](https://docs.github.com/en/github/getting-started-with-github/fork-a-repo#fork-an-example-repository) so that you can make your changes without affecting the original project until you're ready to merge them.

2. Install or update to **Node.js**, at the version specified in `.node-version`. For more information, see [the development guide](contributing/development.md).

3. Create a working branch and start with your changes!

### Commit your update

Commit the changes once you are happy with them. Don't forget to [self-review](/contributing/self-review.md) to speed up the review process:zap:.

### Pull Request
Define a Pull Request-

When you're finished with the changes, create a pull request, also known as a PR.
- Fill the "Ready for review" template so that we can review your PR. This template helps reviewers understand your changes as well as the purpose of your pull request. 
- Don't forget to [link PR to issue](https://docs.github.com/en/issues/tracking-your-work-with-issues/linking-a-pull-request-to-an-issue) if you are solving one.
- Enable the checkbox to [allow maintainer edits](https://docs.github.com/en/github/collaborating-with-issues-and-pull-requests/allowing-changes-to-a-pull-request-branch-created-from-a-fork) so the branch can be updated for a merge.
Once you submit your PR, a Docs team member will review your proposal. We may ask questions or request additional information.
- We may ask for changes to be made before a PR can be merged, either using [suggested changes](https://docs.github.com/en/github/collaborating-with-issues-and-pull-requests/incorporating-feedback-in-your-pull-request) or pull request comments. You can apply suggested changes directly through the UI. You can make any other changes in your fork, then commit them to your branch.
- As you update your PR and apply changes, mark each conversation as [resolved](https://docs.github.com/en/github/collaborating-with-issues-and-pull-requests/commenting-on-a-pull-request#resolving-conversations).
- If you run into any merge issues, checkout this [git tutorial](https://github.com/skills/resolve-merge-conflicts) to help you resolve merge conflicts and other issues.

## Best Practices

### Identity and Access Management
  - **Use a CODEOWNERS file** to define individuals or teams that are responsible for code in a repository.
  - **Use the principle of least privilege** to ensure users are not granted more access than they need.
  - **Synchronize GitHub Teams and Azure Active Directory** through Enterprise Managed Users to automate user provisioning and deprovisioning inside organizations.
  - **Have multiple code owners** to ensure continuing access to the organization.

### Security
  - **Enable GitHub Advanced Security** to utilize its security features
  - **Protect secrets from being exposed** during code commits by using GitHub Secret Scanning or a third-party scanning program
  - **Use Code Scanning** upon each push and pull request to automatically detect security vulnerabilities and coding errors in new or modified code using CodeQL
  - **Monitor dependencies** for your project using GitHub Dependency Graph and Dependency Review
  - **Enable Dependabot** to inform you of any security vulnerabilities in your dependencies
  - **Maintain Audit trails** of all changes to repositories
  - **Only utilize **Company Name** Actions** inside code to prevent supply chain vulnerabilities
  
### Code Alterations
  - **Perform code checks** prior to committing code to the main branch
  - **Branch and test your code often**, and commit once.
  - **Use GitHub Secrets** to encrypt and prevent secrets, authentication tokens, and other credentials being stored in plaintext.
  - **Make small changes often** to branches, rather than infrequent, large changes.
  - **Require status checks** from administrators before merging branches.
  - **Use both automated and manual code review** to prevent errors being committed to builds.
  
### Communication
  - **Use built-in communication features** in issues and pull requests to let you easily communicate with your collaborators. 
  - **Assign collaborators to specific issues** to communicate responsibility.
  - **Write short, detailed comments** on commits and pull requests
 
