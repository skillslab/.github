# :blue_book: Template for READMEs

This serves as a template for new READMEs and should be used as a guideline for existing ones.

Use [markdownlint](https://marketplace.visualstudio.com/items?itemName=DavidAnson.vscode-markdownlint) to lint the README. This is part of the *Doc Writer* Visual Studio Code Profile.

Use backticks for `filenames` and `directories`, `ENVIRONMENT_VARIABLES`, `executables`, `keys` and `--command-line-arguments`.

The title must be the name of the repository and can be preceded by an [emoji](https://github.com/ikatyang/emoji-cheat-sheet/blob/master/README.md) that has something to do with the repository .

Describe what the application(s)/services(s)/content of this repository are and how they are used in relation to other applications and services.

For large README files a table of content can be added, which can be automated with the [Auto Markdown TOC extension](https://marketplace.visualstudio.com/items?itemName=huntertran.auto-markdown-toc) (adjust the depth to start from with `depthFrom:2` after the `TOC` marker):

<!-- TOC depthfrom:2 -->

- [:blue_book: Usage](#blue_book-usage)
- [:whale: or :arrow_forward: Run a release](#whale-or-arrow_forward-run-a-release)
- [:hammer_and_wrench: Prerequisites](#hammer_and_wrench-prerequisites)
- [:desktop_computer: Development](#desktop_computer-development)
    - [Getting Started](#getting-started)
    - [Building](#building)
    - [Testing](#testing)
- [:art: Assets or Sprites](#art-assets-or-sprites)
- [:handshake: Contributing](#handshake-contributing)
- [:rocket: Production](#rocket-production)
- [:mag: Links to further information](#mag-links-to-further-information)

<!-- /TOC -->

## :blue_book: Usage

Describe or link all applications/services in this repository as well as their command line options or environment variables.

## :whale: or :arrow_forward: Run a release

If running a release is the easiest way to run the application or services of the repository, this section should be the first one.

Describe where the release can be downloaded (`docker pull` or release download) and how to start it locally. This must include all required environment variables. Use the :whale: icon for docker containers and the :arrow_forward: for all other releases.

If there is a lot of configuration, provide the command to start the service with our scripts in [docker-images](https://github.com/skillslab/docker-images) first, otherwise after the [Docker](https://www.docker.com/) or [Docker Compose](https://docs.docker.com/compose/) command.

## :hammer_and_wrench: Prerequisites

You have to add clone instructions if a simple pull is not sufficient. For example if submodules have to be checked out.

Add instructions for software that has to be installed on the machine to run the code or link to another repository or other documentation which covers the setup. Often used examples are [ansible repo](https://github.com/skillslab/ansible) and [Dev Containers](https://code.visualstudio.com/docs/devcontainers/containers).

## :desktop_computer: Development

### Getting Started

Describe how to start up the development environment. Either with docker, Visual Studio Code and Dev Containers or the Unreal Engine. If there are multiple ways, mention all, but start with the most used. Also mention the differences.

### Building

In this section describe how the project can be built and describe which configurations are available.

### Testing

Explain where the tests are organized and how they can be executed.

## :art: Assets or Sprites

In this section you can mention steps related to assets. If the steps are mandatory for builds, you have to include this section.

## :handshake: Contributing

Link to a `CONTRIBUTING.md` which explains what steps are required to contribute to this repository. This file is linked when a new pull request is created.

Provide links to coding guidelines and style guides that are followed as well es linters or formatters that are used.

Explain how hooks can be setup and what they are doing. Enumerate which checks are performed for each pull request so that a contributor can run them locally and doesn't have to wait for the feedback of github actions.

Link to the logging framework that is used, mention the logging file location and whether the log files are stored in graylog. Also link to utility tools (functions, classes) used for logging.

## :rocket: Production

Describe how production releases are created and which options are available to get to branch releases.

## :mag: Links to further information

List links to further information already in the repository or in the confluence or external documentation.
