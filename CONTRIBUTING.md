## How to Contribute

The Rook project in under [Apache 2.0 license](LICENSE). We accept contributions via
GitHub pull requests. This document outlines some of the conventions related to
development workflow, commit message formatting, contact points and other
resources to make it easier to get your contribution accepted.

## Certificate of Origin

By contributing to this project you agree to the Developer Certificate of
Origin (DCO). This document was created by the Linux Kernel community and is a
simple statement that you, as a contributor, have the legal right to make the
contribution. See the [DCO](DCO) file for details.

## Getting Started

- Fork the repository on GitHub
- Read the [README](README.md) for build and test instructions
- Play with the project, submit bugs, submit patches!

## Contribution Flow

This is a rough outline of what a contributor's workflow looks like:

- Create a branch from where you want to base your work (usually master).
- Make your changes and arrange them in readable commits.
- Make sure your commit messages are in the proper format (see below).
- Push your changes to the branch in your fork of the repository.
- Make sure all tests pass, and add any new tests as appropriate.
- Submit a pull request to the original repository.

## Coding Style

Rook projects are written in golang and follows the style guidelines dictated by
the go fmt as well as go vet tools.

## Commit Messages

We follow a rough convention for commit messages that is designed to answer two
questions: what changed and why. The subject line should feature the what and
the body of the commit should describe the why.

```
cephmgr: update MON to use rocksdb

this enables us to remove leveldb from the codebase.
```

The format can be described more formally as follows:

```
<subsystem>: <what changed>
<BLANK LINE>
<why this change was made>
<BLANK LINE>
<footer>
```

The first line is the subject and should be no longer than 70 characters, the
second line is always blank, and other lines should be wrapped at 80 characters.
This allows the message to be easier to read on GitHub as well as in various
git tools.
