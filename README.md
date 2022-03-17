# AWS-SERVICE-UTILS

## What is this?

This package is a ever growing collection of aws functionalities written in typescript available to you in form of utils

## Installation

```sh
$ npm i aws-service-utils
```

## Usage

```js
const { secretsManager } = require('aws-service-utils').services;

async function setConfig() {
    const secret = (await secretsManager.getSecret({
        secretName: 'secretName',
        region: 'ap-south-1'
    }));
    console.log(secret);
}

setConfig();
```