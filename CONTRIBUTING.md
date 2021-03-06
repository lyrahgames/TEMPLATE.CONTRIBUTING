# Contributing

First off, thanks for taking the time to contribute!

The following is a set of guidelines for contributing to the project and its packages, which are hosted on [GitHub](https://github.com/lyrahgames/pxart).
These are mostly guidelines, not rules.
Use your best judgment, and feel free to propose changes to this document in a pull request.

## Table of Contents
<!-- MarkdownTOC -->

- Code of Conduct
- What should I know before I get started?
- How can I contribute?
    - Asking Questions, Reporting Bugs, and Suggesting Enhancements
    - Code Contribution and Pull Requests
- Development Environment
- Styleguides
    - Git
    - C++
    - Build System
    - Documentation
- Additional Notes

<!-- /MarkdownTOC -->


## Code of Conduct
This project and everyone participating in it is governed by the [Code of Conduct](CODE_OF_CONDUCT.md).
By participating, you are expected to uphold this code.
Please report to lyrahgames@mailbox.org if unacceptable behavior is encountered.

## What should I know before I get started?
This is an open-source project developed to learn, to have fun, and maybe even to provide useful utilities.
No one is forced to work on this project.
Hence, it may take its time to reply to messages or newly created issues.
Furthermore, take into account that it may be possible that your issue is not answered or resolved easily.
Please, do not hesitate to contribute because in fear of doing mistakes.
Everyone can make mistakes and that is no problem.
We will learn from them and are able to make it better the next time.

## How can I contribute?
### Asking Questions, Reporting Bugs, and Suggesting Enhancements
You don't need to be a developer to make a significant impact - just a GitHub account.
If even that is not possible, report to lyrahgames@mailbox.org and we will try to find another way.
Please, [open an issue on GitHub](https://github.com/lyrahgames/pxart/issues) and ask your question, report the bug you may have found, or suggest the enhancement that you would like to see in a future update.
Try to make sure, there is not already an issue with the same topic, and to adhere to the following issue guidelines.

**Issue Guidelines:**
- Do not send a new question by replying to an existing message. Instead, create a new issue with a new, descriptive subject.
- Choose a descriptive subject for your post. Examples of bad subjects: "Quick question", "Problem", "Help me", "SOS!!!". Examples of good subjects: "Error compiling foo.cpp with Clang 3.7", "Unable to use feature `X` to achieve result `Y`".
- If reporting a problem, specify all the relevant package and environment information. This includes the package version, operating system name and version, C++ compiler name and version, command lines used, and the exact diagnostics observed. Generally, the more details you provide, the less the person trying to help you will have to guess and assume.

### Code Contribution and Pull Requests
You can follow [Github's Pull Request Model](https://docs.github.com/en/github/collaborating-with-issues-and-pull-requests/creating-a-pull-request-from-a-fork).
- Fork the repository and setup your development environment accordingly as described below.
- Clone the forked repo with its submodules and start hacking yourself.
- Make sure that basic tests run successfully.
- Push your new changes and make your pull request.

## Development Environment
Currently, the project is developed under Linux and only tested on other platforms.
If you need to use a Windows or MacOS environment and there is no straightforward explanation how to do it, please ask a question.

- Get all requirements that are stated on the [project's page](README.md).
- Install `clang-format` for satisfying correct formatting rules.
- [Optional] Enable automatic formatting of source files on file save in your editor by using a custom extension. This will make your life much easier.
- Enable the Git hooks directory as described in the Git style guide in the following section.
- Before cloning, create a directory with the name of the project inside your typical projects directory. We call this the developer folder.
- Now clone the forked repository. This will be the project folder.
- Inside the project folder, initialize one ore more configurations by the `bdep init -C ...` command.
- Try to compile and test by using `bdep update -a` and/or `bdep test -a`.
- Start hacking.
- If you have not enabled automatic clang-format checks, you will have to manually format your files.

## Styleguides

### Git
- Use the white-listing approach in newly created `.gitignore` files by first ignoring everything and then enabling which files are allowed to be added to the repository.
- Default hooks are given inside the `.githooks` directory of the repository to help you adhere to some guidelines.
For this project, you should enable this path as the default hooks directory by using the following command.
```
git config --local core.hooksPath .githooks
```
- As far as possible, adhere to [the seven rules of a great git commit message](https://chris.beams.io/posts/git-commit/).
- If your changes in the source code are more involved, consider creating multiple commits such that your intentions and ideas are easier to follow for everyone else when taking a look in the commit history of the repository.

### C++
To not make this document excessively long, the styleguide for C++ will not be explained thoroughly here.
In this project, a custom C++ style is used.
When creating something new or introducing changes look at the code around and try to be consistent.
If in doubt, post a question.
Formatting should be done before doing a commit with `clang-format` in the style of the project which is given by the `.clang-format` file in the root of the repository.

### Build System
The project is built by [the build2 toolchain](https://build2.org).
Tweaking the buildfiles of the project will need a certain understanding of its functioning.
Read through the documentation to get yourself accustomed to the basics.
Ask a question if there are more advanced problems.

### Documentation
Typically, only the minority of developers are native English speakers.
So it is natural language mistakes will arise regularly.
When creating documentation, use full, descriptive sentences and try not to make them overly complicated.
The same holds true for the general explanation.
Be grammatically correct to the best of your knowledge.

## Additional Notes