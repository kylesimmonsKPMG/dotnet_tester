# <Company Name> CONTRIBUTING.md

This document includes instructions on best practices to follow when using the <Company Name> GitHub account. These instructions are separated by subject matter. See the [Table of Contents](#table-of-contents) for different sections of best practice. Please make sure to read the relevant sections before making contributions, both for security and for efficiency purposes. 


## Table of Contents

- [Code of Conduct](#code-of-conduct)
- [Suggesting Enhancements](#suggesting-enhancements)
- [Improving The Documentation](#improving-the-documentation)
- [Identity and Access Management](#identity-and-access-management)
- [Security Tools](#security)
- [Coding](#coding)
- [Communication](#communication)



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
  - **Only utilize <Company Name> Actions** inside code to prevent supply chain vulnerabilities
  
### Coding
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
 
