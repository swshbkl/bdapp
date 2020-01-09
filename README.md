<!-- omit in toc -->
# 👾 bdapp

> IndieCasa Mobile App

[![Open in Gitpod](https://gitpod.io/button/open-in-gitpod.svg)](https://gitpod.io/#https://github.com/swshbkl/bdapp)

![Version](https://img.shields.io/github/v/tag/swshbkl/bdapp)
[![Github CI/CD](https://img.shields.io/github/workflow/status/swshbkl/bdapp/Build%20and%20Deploy)](https://github.com/swshbkl/bdapp/actions?query=workflow%3A%22Build+and+Deploy%22)

[![Language](https://img.shields.io/badge/language-typescript-2B4F7E.svg?longCache=true)](https://www.typescriptlang.org/docs/handbook/typescript-in-5-minutes.html/)
[![Framework](https://img.shields.io/badge/framework-expo-473BE7.svg?longCache=true)](https://docs.expo.io/versions/latest/)
[![Deployment](https://img.shields.io/badge/deployment-expo-473BE7.svg?longCache=true)](https://docs.expo.io/versions/latest/guides/configuring-ota-updates/)

[![Discord](https://img.shields.io/discord/649868467893305346)](https://discordapp.com/channels/649868467893305346/650432461490094080)
[![Email](https://img.shields.io/badge/email-buck-blue.svg?longCache=true)](mailto:buck@bucktower.net)
![Maintenance](https://img.shields.io/maintenance/yes/2019.svg?style=flat-square)

<!-- ![Screenshot](https://i.imgur.com/WSahR2w.jpg) -->

---

<!-- omit in toc -->
## Table of Contents

- [Features](#features)
- [Documentation](#documentation)
- [<s>Tests</s> Work In Progress](#stestss-work-in-progress)
  - [Running unit tests](#running-unit-tests)
  - [Running end-to-end tests](#running-end-to-end-tests)
  - [Linting](#linting)
- [Contributing (while in Pre-release)](#contributing-while-in-pre-release)
  - [Step 1](#step-1)
  - [Step 2](#step-2)
- [<s>Contributing (once released in Alpha)</s>](#scontributing-once-released-in-alphas)
  - [Step 1](#step-1-1)
  - [Step 2](#step-2-1)
  - [Step 3](#step-3)
- [Deployment](#deployment)
  - [Step 1](#step-1-2)
  - [Step 2](#step-2-2)
- [Team](#team)
- [FAQ](#faq)
- [Support](#support)
- [License](#license)

---

## Features

- Mobile app for IndieCasa

## Documentation

No documentation yet

## ~~Tests~~ *Work In Progress*

### Running unit tests

> Execute the unit tests via [Karma](https://karma-runner.github.io)

```shell
$ npm run test
```

### Running end-to-end tests

> Execute the end-to-end tests via [Protractor](http://www.protractortest.org/)

```shell
$ npm run e2e
```

### Linting

> Run linting tools as per the [Angular Style Guide](https://angular.io/guide/styleguide)

```shell
$ npm run lint
```

---

## Contributing (while in [Pre-release](https://github.com/swshbkl/bdapp/releases))

> To get started...

### Step 1

- 👯 Click this button that you can also find up top:

[![Open in Gitpod](https://gitpod.io/button/open-in-gitpod.svg)](https://gitpod.io/#https://github.com/swshbkl/bdapp)

**The `master` branch is the single-source-of-truth. No other banches at the moment, we're just tring to go as fast as possible.**

### Step 2

- **HACK AWAY!** 🔨🔨🔨
- 📦 Push to `master` often because working from one branch could lead to some massive merge conflicts
- 👀 You can see your changes hot-reloaded by Gitpod by going to the `Open Ports` tab of the terminal window and opening the Preview or Browser for `3000`

If you close your window and boot up later without finishing and pushing:

- "Start" the Gitpod instance that has been stopped and archived in your [Gitpod workspaces](https://gitpod.io/workspaces/)

## ~~Contributing (once released in Alpha)~~

> To get started...

We use [SemVer](https://semver.org/) for versioning.

**The `master` branch is the single-source-of-truth. All other branches are feature branches to be merged in.**

We use a trunk-based, "Github flow" model. [Please click through this (5 minutes)](https://guides.github.com/introduction/flow/).
For more information, see [reasons why](https://githubflow.github.io/).

### Step 1

- 👯 Create an issue in Github that outlines what you hope to accomplish.
As part of the templating for the issue, you will fill in a Github issue number that will generate one of these buttons on the issue:

![Open in Gitpod](https://gitpod.io/button/open-in-gitpod.svg)

- 🌱 Upon clicking the button in the issue, a local branch named `GH-{issue-number}` will be created automatically, based on `master` and wil be open in Gitpod

### Step 2

- **HACK AWAY!** 🔨🔨🔨
- 📦 Feel free to push to your feature branch whenever
- 👀 You can see your changes hot-reloaded by Gitpod by going to the `Open Ports` tab of the terminal window and opening the Preview or Browser for `3000`

*It's suggested, but not required to push changes before you close Gitpod.* If closed and not reopened for 30 minutes, the workspace will be stopped.

If your workspace is stopped, no fret, it has been saved and is able to be re-"Start"ed from [Gitpod Workspaces](https://gitpod.io/workspaces/)

### Step 3


- 👨‍🍳 Once your features are ready for review, the Pull Request ("PR") view on the right in Gitpod can be used to push changes to a remote repository and create a pull request.

- 🗣 Debate and critique ensues over your PR

- 🔀 Your PR is accepted and merged into `master`. The Github issue will be automatically closed once the PR has been approved and merged into `master`

## Deployment

This part is mostly just for Buck to use, but it's worth documenting

We use [SemVer](https://semver.org/) for versioning.

We value quickness and agility over circumspect and slow-moving.
Only non-production server is the one you run on Gitpod.
Since it's in the cloud, others can access it over the open ports while it's running if you need testing and PR reviews.


### Step 1

- 🏷 Decide the proper version number as per [SemVer](https://semver.org/) and edit `package.json`
    - Given a version number `MAJOR.MINOR.PATCH`, increment the:
        - `MAJOR` version when you make incompatible API changes
        - `MINOR` version when you add functionality in a backwards-compatible manner, and
        - `PATCH` version when you make backwards-compatible bug fixes.

`package.json`:

```json
{
  ...
  "version": "MAJOR.MINOR.PATCH",
  ...
}
```

### Step 2

Deployed to [`expo.io/@bucktower/indiecasa`](https://expo.io/@bucktower/indiecasa) automatically whenever a new [Release](https://github.com/swshbkl/bdapp/releases) is created off of the `master` branch.

Able to be opened up and run on an iPhone or Android using the Expo smartphone app, ~~or by downloading the actual app from the respective app stores~~ (once published).

Native apps will automatically check for and update OTA (over-the-air) on launch whenever a new change is pushed to [`expo.io/@bucktower/indiecasa`](https://expo.io/@bucktower/indiecasa).

Don't fuck up and we'll be fine 🤗

---

## Team

| [**Buck Tower**](https://bucktower.net) |
| :---: |
| [![Buck Tower](https://avatars1.githubusercontent.com/u/1170938?v=3&s=200)](https://bucktower.net)|
| [`github.com/bucktower`](https://github.com/bucktower) |

---

## FAQ

- **How do I do *specifically* so and so placeholder?**
  - No problem! Just do this.

## Support

Reach out at one of the following places!

- Join the [Discord channel](https://discordapp.com/channels/649868467893305346/649868575049252865)
- Email [`buck@bucktower.net`](mailto:buck@bucktower.net)

---

## License

- **[ISC](https://opensource.org/licenses/ISC)**
- Copyright 2019 © [Swashbuckle Studios](https://swashbuckle.dev).
