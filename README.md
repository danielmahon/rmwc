[![CircleCI](https://circleci.com/gh/jamesmfriedman/rmwc/tree/master.svg?style=shield)](https://circleci.com/gh/jamesmfriedman/rmwc/tree/master)
[![npm](https://img.shields.io/npm/v/rmwc.svg)]()
[![npm](https://img.shields.io/npm/l/rmwc.svg)]()
[![Join the chat at https://gitter.im/react-material-web-components/Lobby](https://badges.gitter.im/react-material-web-components/Lobby.svg)](https://gitter.im/react-material-web-components/Lobby?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)

# RMWC - React Material Web Components

A React (15 / 16) wrapper for Material Design (Web) Components v0.32.0
[https://jamesmfriedman.github.io/rmwc/](https://jamesmfriedman.github.io/rmwc/)

## Recent updates

RMWC is moving towards a direct implementation with MDC's Foundation classes. This means direct code reuse from the material-components-web implementation which will result in better performance, reliability, less bugs, and easier releases for RMWC. These will be rolled out a few at a time every release and will contain minimal breaking changes.

MDC has been upgraded to 0.34.0

The biggest changes in this release are related to Selects. MDC has switched to using standard CSS select elements. This shouldn't break anything in RMWC unless you were using any custom UI to render your List Items. Also, the light and dark variants of primary and secondary theme colors have been removed.

Other than that, there has been some additional housekeeping to improve the developer experience including publishing the unminified ES6 code, exposing the built in FlowTypes, and more testing around server side rendering.

View the changelog for detailed updates: [https://github.com/jamesmfriedman/rmwc/blob/master/CHANGELOG.md](https://github.com/jamesmfriedman/rmwc/blob/master/CHANGELOG.md)

## Goals

* To create the thinnest, lightest, and spec compliant wrapper around Google
  Material Design Components for the Web
  [https://material.io/components/web/](https://material.io/components/web/)
* To utilize the Foundation javascript classes and expose their api for
  consumption
* To be as unobtrusive and sensible as possible.

## Installation

Required steps

* `npm i rmwc --save` or `yarn add rmwc`
* [material-components-web](https://github.com/material-components/material-components-web) should be installed automatically as a peer dependency. Include `node_modules/material-components-web/dist/material-components-web.min.css` in your project via your method of choice (using a link tag, a css-loader, etc.).

Optional steps

* If you would like to use the default **Roboto font**:
  * add `<link href="https://fonts.googleapis.com/css?family=Roboto:300,400,500" rel="stylesheet" />`
  * add the class `mdc-typography` to the body `<body className="mdc-typography">...</body>`
* If you would like to use the **material-icons** font:
  * add `<link href="https://fonts.googleapis.com/icon?family=Material+Icons" rel="stylesheet">`
* Add global settings by using the optional `<RMWCProvider />` component at the root of your project. See the 'Provider' section for more info.

Additional information is available in the [Installation Guide](https://jamesmfriedman.github.io/rmwc/installation)

## Usage

Read the docs on how to [Usage](https://jamesmfriedman.github.io/rmwc/usage)

## Why?

Read the docs on [Methodology](https://jamesmfriedman.github.io/rmwc/methodology)

## About Breaking Changes

Read the docs on [Methodology](https://jamesmfriedman.github.io/rmwc/methodology)

## To run the tests

* On MacOS Sierra and higher, install watchman to fix a filesystem issue with
  Jest. `brew install watchman`
* `npm test`

## To run the docs / contribute

* `git clone https://github.com/jamesmfriedman/rmwc.git`
* `cd rmwc`
* `npm install`
* `npm start`
