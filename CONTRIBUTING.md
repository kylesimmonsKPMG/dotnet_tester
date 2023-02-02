# <Company Name> CONTRIBUTING.md

This document includes instructions on best practices to follow when using the <Company Name> GitHub account. These instructions are separated by subject matter. See the [Table of Contents](#table-of-contents) for different sections of best practice. Please make sure to read the relevant sections before making contributions, both for security and for efficiency purposes. 


## Table of Contents

- [Code of Conduct](#code-of-conduct)
- [Suggesting Enhancements](#suggesting-enhancements)
- [Your First Code Contribution](#your-first-code-contribution)
- [Improving The Documentation](#improving-the-documentation)
- [Identity and Access Management](#identity-and-access-management)
- [Security Tools](#Security)
- [Coding](#coding)
- [Communication](#communication)
- [Styleguides](#styleguides)
- [Commit Messages](#commit-messages)
- [Join The Project Team](#join-the-project-team)



### Suggesting Enhancements

This section guides you through submitting an enhancement suggestion for CONTRIBUTING.md, **including completely new features and minor improvements to existing functionality**. Following these guidelines will help maintainers and the community to understand your suggestion and find related suggestions.


#### Before Submitting an Enhancement

- Make sure that you are using the latest version.
- Read the [documentation]() carefully and find out if the functionality is already covered, maybe by an individual configuration.
- Perform a [search](/issues) to see if the enhancement has already been suggested. If it has, add a comment to the existing issue instead of opening a new one.
- Find out whether your idea fits with the scope and aims of the project. It's up to you to make a strong case to convince the project's developers of the merits of this feature. Keep in mind that we want features that will be useful to the majority of our users and not just a small subset. If you're just targeting a minority of users, consider writing an add-on/plugin library.


#### How Do I Submit a Good Enhancement Suggestion?

Enhancement suggestions are tracked as [GitHub issues](/issues).

- Use a **clear and descriptive title** for the issue to identify the suggestion.
- Provide a **step-by-step description of the suggested enhancement** in as many details as possible.
- **Describe the current behavior** and **explain which behavior you expected to see instead** and why. At this point you can also tell which alternatives do not work for you.
- You may want to **include screenshots and animated GIFs** which help you demonstrate the steps or point out the part which the suggestion is related to. You can use [this tool](https://www.cockos.com/licecap/) to record GIFs on macOS and Windows, and [this tool](https://github.com/colinkeenan/silentcast) or [this tool](https://github.com/GNOME/byzanz) on Linux. 
- **Explain why this enhancement would be useful** to most CONTRIBUTING.md users. You may also want to point out the other projects that solved it better and which could serve as inspiration.



### Identity and Access Management
  - **Use a CODEOWNERS file** to define individuals or teams that are responsible for code in a repository.
  - **Use the principle of least privilege** to ensure users are not granted more access than they need.
  - **Synchronize GitHub Teams and Azure Active Directory** through Enterprise Managed Users to automate user provisioning and deprovisioning inside organizations.
  - **Have multiple code owners** to ensure continuing access to the organization.

### Security
  - Enable GitHub Advanced Security to utilize its security features
  - Protect secrets from being exposed during code commits by using GitHub Secret Scanning or a third-party scanning program
  - Use Code Scanning upon each push and pull request to automatically detect security vulnerabilities and coding errors in new or modified code using CodeQL
  - Monitor dependencies for your project using GitHub Dependency Graph and Dependency Review
  - Enable Dependabot to inform you of any security vulnerabilities in your dependencies
  - Maintain Audit trails of all changes to repositories
  
### Coding
  - Perform code checks prior to committing code to the main branch
  - Branch and test your code often, and commit once.
  - Use GitHub Secrets to encrypt and prevent secrets, authentication tokens, and other credentials being stored in plaintext.
  - Make small changes often to branches, rather than infrequent, large changes.
  - Require status checks from administrators before merging branches.
  - Use both automated and manual code review.
  
### Communication
  - Use built-in features in issues and pull requests to let you easily communicate with your collaborators. 
  - Assign collaborators to specific issues to communicate responsibility.
  - Write short, detailed comments on commits and pull requests
 
