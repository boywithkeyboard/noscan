# noscan

> **`noscan was archived for a while and was revived on February 7, 2022. We'll soon release v3 and stay with a regular update schedule!`**

[![npm](https://img.shields.io/npm/v/noscan)](https://www.npmjs.com/package/noscan)
[![npm](https://img.shields.io/npm/dt/noscan)](https://www.npmjs.com/package/noscan)
[![GitHub last commit](https://img.shields.io/github/last-commit/azurystudios/noscan)](https://github.com/azurystudios/noscan)
[![GitHub issues](https://img.shields.io/github/issues-raw/azurystudios/noscan)](https://github.com/azurystudios/noscan/issues)
[![snyk vulnerabilities](https://snyk.io/test/github/azurystudios/noscan/badge.svg)](https://snyk.io/test/github/azurystudios/noscan)

**A more flexible SDK for [unscan.co](https://unscan.co)** 🔞🔎

- fully asynchronous
- 100% coverage of the unscan API
- typescript support

🤖 [**Discord**](https://github.com/noscanjs/discord) + [**Telegram**](https://github.com/noscanjs/discord) Bot `COMING SOON`      
💻 [**CLI**](https://github.com/noscanjs/cli) `COMING SOON`

## Installation

### Install the Package

Install **noscan** using your favorite package manager.

```sh-session
npm i noscan
yarn add noscan
```

### Usage

```js
import { isNSFW } from 'noscan'

(async () => {
  console.log(await isNSFW(stream))
})()
```

## API

### File Scanning

#### Features

- [`isMalware(file)`]()
- [`isNSFW(image)`]()
- [`scanFileFromStream(stream)`]() `COMING SOON`
- [`scanFileFromLink(url)`]() `COMING SOON`
- [`scanFileFromLocation(location)`]() `COMING SOON`
- [`scanFileFromBuffer(buffer)`]() `COMING SOON`

> ℹ️ noscan will throw an error when something went wrong.

### Link Scanning

#### Features

- [`scanLink(url)`]() `COMING SOON`

> ℹ️ noscan will throw an error when something went wrong.

## CLI `COMING SOON`

### Installation

Install the [CLI](https://github.com/noscanjs/cli) globally using your favorite package manager.

```sh-session
npm i -g @noscan/cli
yarn global add @noscan/cli
```

### Usage

```sh-session
noscan --malware ./file.exe 
```

### Features

- [`--malware`]() to determine whether a file is **malware**
- [`--nsfw`]() to determine whether a image is **nsfw**
- [`--url`]() to determine whether a url is secure or not
