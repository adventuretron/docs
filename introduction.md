# Introduction to Adventuretron

Adventuretron is a tool for creating self-guided workshops that run as desktop apps on MacOS, Windows, & Linux.

## Work in progress

We're still early in the development of Adventuretron. There are weird APIs and messy rough edges. Please let us know what makes sense, what was easy, what was challenging, and what was ridiculously wrong.

## Get involved

- [adventuretron.org](https://adventuretron.org)
- [documentation](https://docs.adventuretron.org)
- [github org](https://github.com/adventuretron)
- [chat](https://gitter.im/adventuretron/discuss)

## Code of conduct

All participants in the production of Adventuretron projects are expected to follow the [code of conduct](https://github.com/adventuretron/discuss/tree/master/CONDUCT.md).

## Overview

### Features
- i18n support
- cross-platform desktop apps
- make workshops for any topic, not just code

### Why create Adventuretron?

After making [javascripting](https://github.com/sethvincent/javascripting) and running a few nodeschool events, I've found that folks struggle with reading all the instructions in the terminal. In part this can be due to various cross-platform issues with specific versions of node. Additionally, trying to have colorized terminal output that is accessible for everybody seems weirdly difficult.

Electron can help with this. [git-it-electron](https://github.com/jlord/git-it-electron) is a great example of how we can have clear, readable instructions in a cross-platform desktop app that still encourages people to learn using the same tools they'd regularly use doing this kind of work.

### What are you using to build this?

The main dependencies of Adventuretron are [electron](http://electron.atom.io/) & [choo](https://github.com/yoshuawuyts/choo).
