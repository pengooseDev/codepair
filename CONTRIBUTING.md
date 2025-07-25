## How to contribute

CodePair is Apache 2.0 licensed and accepts contributions via GitHub pull requests. This document outlines some of the conventions on commit message formatting, contact points for developers, and other resources to help get contributions into Yorkie.

### Contacts

If you have any questions along the way, please don’t hesitate to ask us

- Discord: [Yorkie Discord](https://discord.com/invite/MVEAwz9sBy).

### Getting started

- Fork the repository on GitHub
- Read the README.md for build instructions

## Contribution flow

This is a rough outline of what a contributor's workflow looks like:

1. Create a topic branch from where to base the contribution (usually main).
2. Make commits of logical units.
   - Make sure all tests pass, and add any new tests as appropriate.
   - Make sure commit messages are in the proper format (see below).
3. Push changes in a topic branch to the forked repository.
4. Submit a pull request to the original repository.
5. Address any review comments from CodeRabbit and maintainers.
6. After receiving LGTM from maintainers, the PR will be merged.

Thanks for contributing!

### Format of the commit message

We follow a rough convention for commit messages that is designed to answer two questions: what changed and why. The subject line should feature the what and the body of the commit should describe the why.

```
Remove the synced seq when detaching the document

To collect garbage like CRDT tombstones left on the document, all
the changes should be applied to other replicas before GC. For this
, if the document is no longer used by this client, it should be
detached.
```

The first line is the subject and should be no longer than 70 characters, the second line is always blank, and other lines should be wrapped at 80 characters. This allows the message to be easier to read on GitHub as well as in various git tools.

## Code Review

We use GitHub's pull request review feature to review code. We also use CodeRabbit to automate code review for reducing the effort of maintainers. CodeRabbit will automatically review your pull request and provide feedback on code quality, test coverage, and more.
We require that all code is reviewed by at least one maintainer before being merged. We may ask for changes to be made to the code before it is merged.

## Contributor License Agreement

We require that all contributors sign our Contributor License Agreement ("CLA") before we can accept the contribution.

### Signing the CLA

Open a pull request ("PR") to any of our open source projects to sign the CLA. A bot will comment on the PR asking you to sign the CLA if you haven't already.

Follow the steps given by the bot to sign the CLA. This will require you to log in with GitHub. We will only use this information for CLA tracking. You only have to sign the CLA once. Once you've signed the CLA, future contributions to the project will not require you to sign again.

### Why Require a CLA?

Agreeing to a CLA explicitly states that you are entitled to provide a contribution, that you cannot withdraw permission to use your contribution at a later date, and that Yorkie Team has permission to use your contribution.

This removes any ambiguities or uncertainties caused by not having a CLA and allows users and customers to confidently adopt our projects. At the same time, the CLA ensures that all contributions to our open source projects are licensed under the project's respective open source license, such as Apache-2.0 License.

Requiring a CLA is a common and well-accepted practice in open source. Major open source projects require CLAs such as Apache Software Foundation projects, Facebook projects, Google projects, Python, Django, and more. Each of these projects remains licensed under permissive OSS licenses such as MIT, Apache, BSD, and more.
