# **Company Name** CONTRIBUTING.md

This document includes instructions on best practices and recommendations to follow when using the **Company Name** GitHub account. These instructions are separated by subject matter. For the repository owner, contribution guidelines explain how people should make contributions to the repository. For contributors, the guidelines help verify that they're submitting well-formed pull requests and opening useful issues. For both, contribution guidelines save time and hassle caused by improperly created pull requests or issues that have to be rejected and re-submitted. See the [Table of Contents](#table-of-contents) for different sections of best practice. Please make sure to read the relevant sections before making contributions, both for security and for efficiency purposes. 


## Table of Contents
- [Commit Guide](#commit)
- [Pull Request Guide](#pull-request)
- [Branching Guide](#branching)
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

### Commit
A commit is a discrete change to one or more files that you have write permissions to. These changes are recorded in the local repository. **Company Name** policy is that commits should be made only after testing the code. Make small changes and commit the code often to a branch. Include short, detailed descriptions in the "Update" box of the changes made, and give the update title a distinctive name. This will launch a pull request to the code owner or administrator, who will decide whether or not to approve the change.

<img width="878" alt="image" src="https://user-images.githubusercontent.com/123562599/216442741-3b9ff3e3-2bf2-4b6d-b4a6-2cf827fd3bf0.png">

### Pull Request
A pull request is a request to merge one or more commits into a different branch, "pulling" from a local repository into the remote repository. When a commit is made, the user is redirected to a page to generate a pull request for the changes. The title and description from the commit should carry over into the pull request. 

<img width="673" alt="PullRequest" src="https://user-images.githubusercontent.com/123562599/216445549-53850274-15cc-4d9a-920f-6543b6a59dd6.png">

**Company Name** has enabled "required reviews", which need a specific number of "Approve" reviews from people with write or admin permissions in the repository before they can be merged. For those with elevated permissions in the organization, pull requests can be seen in the "Pull requests" Tab. Code scanning using CodeQL should be done at this phase as well, and passed or failed checks are visible in this menu. 

<img width="611" alt="PullRequestMerge" src="https://user-images.githubusercontent.com/123562599/216447456-d5b0ff94-1e26-4bd1-8b89-2ad35180d0eb.png">

The administrator whose reviews are needed can: 
 - Comment: leaving general feedback without specific approval
 - Approve: Submit feedback and approve merging these changes
 - Request Changes: Submit feedback that must be addressed before merging
Pull Requests can be closed at any time, but if the branch is not deleted, can be reopened.

Further information about approving Pull Requests can be found [here](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/reviewing-changes-in-pull-requests/approving-a-pull-request-with-required-reviews).

![image](https://user-images.githubusercontent.com/123562599/216451795-62dc666b-c449-4eac-ac27-a4edf65dc7bc.png)

After a Pull Request has been merged into a branch, it is best practice to delete the branch the pull request came from, as it is now redundant.

<img width="615" alt="PullRequestMergeSuccess" src="https://user-images.githubusercontent.com/123562599/216457373-83bd5bfd-a8a5-4b5b-8677-c9a09e41b263.png">


### Branching
The main branch should be protected by Branch Protection Rules, found in the "Settings" tab, as advised by the repository's Security Manager.
Defunct Branches should be deleted after they have been merged into the main branch. 

More information on Branch Protection Rules can be found [here](https://docs.github.com/en/repositories/configuring-branches-and-merges-in-your-repository/defining-the-mergeability-of-pull-requests/managing-a-branch-protection-rule).








## General Best Practices

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
 
