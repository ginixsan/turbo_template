# turbo_template

[![test](https://github.com/ginixsan/turbo_template/actions/workflows/test.yml/badge.svg)](https://github.com/ginixsan/turbo_template/actions/workflows/test.yml) [![Maintainability](https://api.codeclimate.com/v1/badges/aa896ec14c570f3bb274/maintainability)](https://codeclimate.com/github/ginixsan/turbo_template/maintainability) [![codecov](https://codecov.io/gh/ginixsan/turbo_template/graph/badge.svg)](https://codecov.io/gh/ginixsan/turbo_template) [![Version](https://img.shields.io/npm/v/turbo_template.svg?colorB=green)](https://www.npmjs.com/package/turbo_template) [![Downloads](https://img.jsdelivr.com/img.shields.io/npm/d18m/turbo_template.svg)](https://www.npmjs.com/package/turbo_template) ![npm bundle size](https://img.shields.io/bundlephobia/minzip/turbo_template) [![Gitpod ready-to-code](https://img.shields.io/badge/Gitpod-ready--to--code-blue?logo=gitpod)](https://gitpod.io/from-referrer/)

> [Featured packages built with this template.](./FEATURED.md)

> We are happy to announce that we have launched a new course to help you understand this template better [Craft Next Gen UI Libraries for React 18 and Next.js 14](https://www.udemy.com/course/craft-next-gen-ui-libraries-for-react-18-and-nextjs-14/?referralCode=46B8C7845ECCEA99E0EF)

## Features

This template offers following pre-configured features. Additionally, your repo will automatically be rebranded with help of workflow and post install scripts.

✅ Monorepo powered by turbo repo to build, test and deploy your library

✅ Next.js, Vite and Remix examples to demonstrate how your library can be used (Feel free to remove Remix as it is still unstable when it comes to monorepo setup and importing from folders)

✅ Examples pre-configured to use Light/Dark theme according to user preference

✅ The examples provided are ready to be deployed to Vercel

✅ Typedoc setup to automatically create documentation for your library based on tsdoc comments

✅ Code of Conduct and contributing files that you can always update

✅ Prettier and linter configured as per the modern best practices (Feel free to add your flavour)

✅ Recommended VSCode extensions - Prettier and [Kanban board](https://github.com/mayank1513/vscode-extension-trello-kanban-board) to auto-format your code and manage your project priorities right within your IDE

✅ Powerful code generators - try yarn turbo gen

✅ Test setup with Vitest - A modern and fast testing framework supporting Jest like APIs

✅ Workflows to automate running tests on every pull-request or code push events

✅ Workflow to automatically publish and create a GitHub release when you update your librari's `package.json` file.

✅ Workflow to automatically rebrand entire template based on the name of the repo you create from this template. (As soon as you create a repo from this template, setup workflow is triggered which renames turbo_template to your repo name and does lots of other fixes to set you up and running.)

✅ With all these features, this readme file contains a quick checklist for you to configure Codecov and other badges, setup your docs website on GitHub pages, etc. See [Checklist](#step-by-step-instructions-and-checklist).

#### Create a library that is

✅ Fully Treeshakable (import from turbo_template/client/component)

✅ Full TypeScript Support

✅ Unleash the full power of React18 Server components

✅ Works with all build systems/tools/frameworks for React18

✅ Doccumented with [Typedoc](https://ginixsan.github.io/turbo_template) ([Docs](https://ginixsan.github.io/turbo_template))

## Install

```bash
$ pnpm add turbo_template
```

or

```bash
$ npm install turbo_template
```

or

```bash
$ yarn add turbo_template
```




## Getting started:

Click on the `"Use this template"` button to customize it for your next JavaScript/TypeScript/React/Vue/Next.js library or project.

## What's Different?

Compared to the default scaffold from create-turbo, this template offers:

- Unit tests with `vitest`
- Build setup with `tsup` and `esbuild-react18-useclient` Supports React Server components out of the box
- **Automatic file generation**
  - just run `yarn turbo gen` and follow the prompts to auto generate your new component with test file and dependency linking
  - follow best practices automatically
- GitHub actions/workflows to auto publish your package when version changes
- GitHub action/workflow + preinstall scripts to automatically rebrand your repo on creation

## Step by Step Instructions and Checklist

- [ ] Star [this repo](https://github.com/ginixsan/turbo_template/) so that you and others can find it more easily for your next projects. It also helps me understand that people are using this repo so that I can maintain the repo and the documentation well.




- [ ] Install and setup Node.js and IDE (I prefer VSCode)
- [ ] Install the recommended VSCode extensions - [Prettier](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode), [Trello Kanban](https://marketplace.visualstudio.com/items?itemName=mayank1513.trello-kanban-task-board)
- [ ] Install dependencies using `pnpm`
  - [ ] If you don't have `pnpm` installed, run `npm i -g pnpm` to install `pnpm` -> run `pnpm setup` to set up `pnpm` for global installations
  - [ ] Run `pnpm i` to install dependencies and `preinstall` script will automatically touch up workflows and create a commit
  - [ ] Run `pnpm i -g turbo` to install `turbo` globally (Sometime due to `TypeScript` and `Plop` version conflicts code generation requires global `turbo`).
  - [ ] Run `turbo gen react-component`, and follow prompts to generate server or client components for your library
    - [ ] Use `snake-case` for your component name - it will be automatically converted to `PascalCase`
    - [ ] Your component and test files will be created in `**/src/client/` or `**/src/server/` directory depending on whether you choose `client` or `server` component
- [ ] run `node scope.js` from the root directory if you want to publish scoped pacckage.
  - [ ] We assumed that your npm user name is same as your GitHub account or organization username.
  - [ ] Please make sure `owner` is set to your <npmjs.com> username before running the above command.
- [ ] Set up `CodeCov`
  - [ ] Visit codecov and setup your repo
  - [ ] Create [repository secret](https://github.com/ginixsan/turbo_template/settings/secrets/actions) for `CODECOV_TOKEN`
- [ ] Set up `CodeClimate`
  - [ ] Visit CodeClimate and setup your repo
  - [ ] Create [repository secret](https://github.com/ginixsan/turbo_template/settings/secrets/actions) for `CC_TEST_REPORTER_ID`
  - [ ] add `*.test.*` to ignore patterns on the website
  - [ ] update code climate badge
- [ ] Add `NPM_AUTH_TOKEN` to repository secrets to automate publishing package
  - [ ] login to your [`npm` account](https://www.npmjs.com/login) and create automation token
  - [ ] Create a new repository secrets `NPM_AUTH_TOKEN`
- [ ] Update description in `lib/turbo_template/package.json`
- [ ] Update Repo Stats by visiting and setting up [repobeats](https://repobeats.axiom.co/)
- [ ] Create your library and update examples
- [ ] Update README
- [ ] Setup GitHub pages to deploy docs
  - [ ] Go to [repo settings](https://github.com/ginixsan/turbo_template/settings/pages) -> pages (On left panel); Select deploy from a branch; Then Select `main` and `/docs`
- [ ] (Optional) Set up [Deepsource](https://app.deepsource.com/login) for static code analysis
- [ ] Push your changes/Create PR and see your library being automatically tested and published
- [ ] Optionally deploy your example(s) to Vercel.
- [ ] Update sponsorship urls.
- [ ] You are most welcome to star this template, contribute, and/or sponsor the `terborepo-template` project or my other open-source work
- [ ] You can also fork the [`terborepo-template`](https://github.com/react18-tools/turbo-repo-template/fork) and add your package to `packages/shared-ui/src/examples/featured.json`
  - [ ] If approved your package will be automatically added to FEATURED.md and also published on the home page of this repo.

## What's inside?

### Utilities

This Turborepo template includes pre-configured tools:

- [TypeScript](https://www.typescriptlang.org/) for static type checking
- [ESLint](https://eslint.org/) for code linting
- [Prettier](https://prettier.io) for code formatting
- Plop based code generator for scaffolding new components
- Automatically rebrand this template to match your repo name

### Apps and Packages

This Turborepo includes the following packages/examples/lib:

- `nextjs`: a [Next.js](https://nextjs.org/) app
- `vite`: a [Vite.js](https://vitest.dev) app
- `fork-me`: a React component library shared by both `Next.js` and `Vite` examples
- `eslint-config-custom`: ESLint configurations (includes `eslint-config-next` and `eslint-config-prettier`)
- `tsconfig`: `tsconfig.json`s used throughout the monorepo

Each package/example is 100% [TypeScript](https://www.typescriptlang.org/).

### Build

To build all apps and packages, run the following command:

```
cd turbo_template
pnpm build
```

### Develop

To develop all apps and packages, run the following command:

```
cd turbo_template
pnpm dev
```

## Useful Links

Learn more about the power of Turborepo:

- [Tasks](https://turbo.build/repo/docs/core-concepts/monorepos/running-tasks)
- [Caching](https://turbo.build/repo/docs/core-concepts/caching)
- [Remote Caching](https://turbo.build/repo/docs/core-concepts/remote-caching)
- [Filtering](https://turbo.build/repo/docs/core-concepts/monorepos/filtering)
- [Configuration Options](https://turbo.build/repo/docs/reference/configuration)
- [CLI Usage](https://turbo.build/repo/docs/reference/command-line-reference)

### 🤩 Don't forger to star [this repo](https://github.com/ginixsan/turbo_template)!

Want hands-on course for getting started with Turborepo? Check out [React and Next.js with TypeScript](https://mayank-chaudhari.vercel.app/courses/react-and-next-js-with-typescript) and [The Game of Chess with Next.js, React and TypeScrypt](https://www.udemy.com/course/game-of-chess-with-nextjs-react-and-typescrypt/?referralCode=851A28F10B254A8523FE)

![Repo Stats](https://repobeats.axiom.co/api/embed/2ef1a24385037998386148afe5a98ded6006f410.svg "Repobeats analytics image")

## License

Licensed as MIT open source.

<hr />

<p align="center" style="text-align:center">with 💖 by <a href="https://mayank-chaudhari.vercel.app" target="_blank">Mayank Kumar Chaudhari</a></p>
