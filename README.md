# AWS-SERVICE-UTILS

## What is this?

This package is a ever growing collection of aws functionalities available to you in form of utils

## Table of contents
- [Generate Desi Names](#generate-desi-names)
    - [What is Generate desi names?](#what-is-generate-desi-names)
    - [Table of contents](#table-of-contents)
    - [Installation](#installation)
    - [Usage](#usage)
        - [Typescript support](#typescript-support)

## Installation

```sh
$ npm i aws-service-utils
```

## Usage

```js
const { secretsManager } = require('aws-service-utils').services;

async function setConfig() {
    const secret = (await secretsManager.getSecret({
        secretName: 'dice',
        region: 'ap-south-1'
    }));
    console.log(secret);
}

setConfig();
```