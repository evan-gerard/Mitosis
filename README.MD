<p align="center"><img width="400" src="https://cdn.builder.io/api/v1/image/assets%2FYJIGb4i01jvw0SRdL5Bt%2F928fd46bd9d84a3fbc5b31fd5b93a7df"></p>

<p align="center">
  Write components once, run everywhere. Compiles to:
</p>

<p align="center"><img width="500" src="https://cdn.builder.io/api/v1/image/assets%2FYJIGb4i01jvw0SRdL5Bt%2Feceb6573940b4af0a2b6d96719be45fc" /></p>

<p align="center">
  <a href="https://mitosis.builder.io/">
    <img width="800" alt="Fiddle" src="https://imgur.com/H1WTtGe.gif" />
  </a>
  <p align="center">
    Try our  <a href="https://mitosis.builder.io/"><b>interactive fiddle</b></a>
  </p>
</p>

<p align="center">
  <a href="https://github.com/prettier/prettier"><img alt="code style: prettier" src="https://img.shields.io/badge/code_style-prettier-ff69b4.svg" /></a>
  <a href="https://github.com/BuilderIO/mitosis/pulls"><img alt="PRs Welcome" src="https://img.shields.io/badge/PRs-welcome-brightgreen.svg" /></a>
  <a href="https://github.com/BuilderIO/mitosis"><img alt="License" src="https://img.shields.io/github/license/BuilderIO/mitosis" /></a>
  <a href="https://www.npmjs.com/package/@builder.io/mitosis"><img alt="Types" src="https://img.shields.io/npm/types/@builder.io/mitosis" /></a>
  <a href="https://www.npmjs.com/package/@builder.io/mitosis" rel="nofollow"><img src="https://img.shields.io/npm/v/@builder.io/mitosis.svg?sanitize=true"></a>
</p>

## Table of contents

- [Getting Started](#getting-started)
- [Docs](#docs)
- [Why use Mitosis?](#why-use-mitosis)
  - [Component libraries](#component-libraries)
  - [Modern workflows for all platforms](#modern-workflows-for-all-platforms)
  - [JS framework fatigue](#js-framework-fatigue)
  - [Design to code](#design-to-code)
- [Status](#status)
- [Contribute](#contribute)
- [Coming soon](#coming-soon)
- [Community](#community)
- [ESLint Rules](#eslint-rules)
- [Related Projects](#related-projects)

## Getting Started

The best way to learn Mitosis is to clone our [example project](./examples/basic/) and start tinkering. Otherwise, here are some helpful external resources on trying out Mitosis:

- https://blog.logrocket.com/creating-reusable-components-mitosis-builder-io/

## Overview

[![Mitosis Video](https://cdn.builder.io/api/v1/image/assets%2FYJIGb4i01jvw0SRdL5Bt%2Ffa5c422309ce4fbea9eaa133fa471877)](https://www.youtube.com/watch?v=XQIuv34-K_8 "Mitosis Video")

## Docs

Curious about how Mitosis code works under the hood, and how to use it? Learn more [in our in-depth docs](docs/).

## Why use Mitosis?

### Component libraries

Providing a UI component library across multiple frameworks is a _pain_, especially when webcomponents are not an option (e.g. for server side rendering, best performance, etc). With Mitosis, you can write once and run everywhere while maintaining full compatibilty with the target framework.

### Modern workflows for all platforms

Mitosis allows you to incrementally adopt modern and familiar workflows for many different platforms. For instance, when working with Shopify, you can server side render to liquid and hydrate with React.

### JS framework fatigue

If you have ever had to migrate a huge codebase from one framework to another, it's an absolute nightmare. Writing components at a higher level of abstraction allows you to move from one to another with ease.

### Design to code

With Mitosis, you can convert designs from [Figma](https://github.com/BuilderIO/html-to-figma) or Sketch and convert them to clean code for the framework of your choice. You can even use [Builder.io](https://github.com/builderio/builder) to visually drag/drop to build UIs and edit the code _side by side_.

<p align="center">
<img width="80%" src="https://i.imgur.com/UlWMkRx.gif" >
</p>

## What about XKCD

<img alt="XKCD comic about solving too many standards by creating new standards just making yet another standard" src="https://user-images.githubusercontent.com/844291/168342803-5599952e-a400-4918-851d-5af93dc19585.png" width="500">

Yup, we've all seen it. But if this is a concern for you, you may be looking at Mitosis wrong. Rather than just yet-another-component-syntax, Mitosis is a compiler for the frontend, analogous to [LLVM](https://en.wikipedia.org/wiki/LLVM). A toolchain that embraces that there are, and forever will be, many ways of writing components. Mitosis defines a common [intermediate representation](https://en.wikipedia.org/wiki/Intermediate_representation) that allows us to author components once then compile to many frameworks, just like LLVM lets us write code that can compile to any [instruction set architecture](https://en.wikipedia.org/wiki/Instruction_set_architecture). If you look at Mitosis this way, you may more clearly see the value.

Also similarly to LLVM, multiple syntaxes can compile to Mitotis. Our out-of-the-box syntax uses JSX, but we have explored others, such as a Vue/Svelte-like syntax. [Builder.io](https://github.com/builderio/builder) emits Mitosis IR, allowing you to turn designs to code for any supported framework. JSX and Builder.io are the currently supported frontends of the compiler, and the frameworks listed below are the backends.

## Status

| Framework     | Status       |
| ------------- | ------------ |
| React         | Beta         |
| Qwik          | Beta         |
| Vue           | Beta         |
| Liquid        | Alpha        |
| Builder.io    | Beta         |
| Solid         | Beta         |
| Figma         | Alpha        |
| Angular       | Beta         |
| Svelte        | Beta         |
| HTML/CSS/JS   | Beta         |
| Webcomponents | Beta         |
| React Native  | Beta         |
| SwiftUI       | Experimental |

## Contribute

Interested in contribute? Head over to the [developer](developer/) docs and see how you can get setup & started!

Once you're ready, checkout our [issues](https://github.com/BuilderIO/mitosis/issues?q=is%3Aopen+is%3Aissue+label%3A%22good+first+issue%22) page and grab your first issue!

## Coming soon

[V1 release](https://github.com/orgs/BuilderIO/projects/4) (help wanted!)

## Community

- [Mitosis Discord](https://discord.gg/CQZt8hzZJR)
- [@Builderio](https://twitter.com/builderio)

## ESLint rules

Checkout our [ESLint plugin](./packages/eslint-plugin/) project for useful rules when developing in Mitosis.

## Related Projects

- [Figma plugin](https://github.com/BuilderIO/figma-html): Convert Figma designs into high quality HTML, React, Vue, Svelte, Angular, Solid, etc code via Mitosis.
- [Builder](https://github.com/BuilderIO): Drag and drop page builder and CMS for React, Vue, Angular, and more.
- [Qwik](https://github.com/BuilderIO/qwik): An open-source framework designed for best possible time to interactive, by focusing on resumability of server-side-rendering of HTML, and fine-grained lazy-loading of code.
- [Partytown](https://github.com/BuilderIO/partytown): Relocate resource intensive third-party scripts off of the main thread and into a web worker. 🎉

<p align="center">
  Made with ❤️ by <a target="_blank" href="https://www.builder.io/">Builder.io</a>
</p>
