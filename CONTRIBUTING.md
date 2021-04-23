# Contributing

First off, thanks for taking the time to contribute!

The following is a set of guidelines for contributing to the project and its packages, which are hosted on GitHub.
These are mostly guidelines, not rules.
Use your best judgment, and feel free to propose changes to this document in a pull request.

## Table of Contents
<!-- MarkdownTOC -->

- Code of Conduct
- Getting Started
- TL;DR
    - FAQ and Questions
    - Mailing List
    - Issues
- What should I know before I get started?
- What can you contribute to?
- How can I contribute?
    - Reporting Bugs
    - Suggesting Enhancements
    - Code Contribution and Pull Requests
- Development Environment
    - Getting Started and Setup
- Styleguides
    - Git
        - `.gitignore` Files
        - Hooks
        - Commit Messages
        - Count of Commits
    - C++
    - Build System
    - Documentation
- Additional Notes

<!-- /MarkdownTOC -->


## Code of Conduct
This project and everyone participating in it is governed by the [Code of Conduct](CODE_OF_CONDUCT.md).
By participating, you are expected to uphold this code.
Please report to lyrahgames@mailbox.org if unacceptable behavior is encountered.

## Getting Started
## TL;DR
### FAQ and Questions
### Mailing List
### Issues

## What should I know before I get started?
## What can you contribute to?

## How can I contribute?
### Reporting Bugs
### Suggesting Enhancements
### Code Contribution and Pull Requests

## Development Environment
Currently, the project is developed under Linux and only tested on other platforms.
If you need to use a Windows or MacOS environment
### Getting Started and Setup

## Styleguides

### Git
#### `.gitignore` Files
Typically, white-listing shall be used to enable files that we want to have in a project repository.

#### Hooks
Default hooks are given inside the `.githooks` directory of the project.
For this project, you should enable this as default hooks directory.

    git config --local core.hooksPath .githooks

#### Commit Messages
As far as possible, we will adhere to [the seven rules of a great git commit message](https://chris.beams.io/posts/git-commit/).
These rules can be enforced by commit message hook.

#### Count of Commits
If your changes are more involved, please create multiple commits such that for anyone else it is easier to follow.


### C++
Custom C++ Style
Formatting with clang-format. Can be enforced by git hook.
Style is given by .clang-format file in root directory of the project.

### Build System
Currently, the build2 toolchain is used to build the project.
Please, learn about it when adding information to the build system.

### Documentation
Grammatically correct.
Full sentences.
As simple as possible.
Explainable.

## Additional Notes