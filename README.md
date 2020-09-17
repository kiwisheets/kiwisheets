# Kiwisheets

![Logo](branding/logo.png)

## Build status
| Module      | Status                                                                                                                       |
| ----------- | ---------------------------------------------------------------------------------------------------------------------------- |
| Frontend    | [![Build Status](https://github.com/kiwisheets/frontend/workflows/CI/CD/badge.svg)](https://github.com/kiwisheets/frontend)  |
| GQL Server  | [![Build Status](https://github.com/kiwisheets/gql-server/workflows/CI/CD/badge.svg)](https://github.com/kiwisheets/gql-server)   |
| File Server | [![Build Status](https://travis-ci.com/kiwisheets/file-server.svg?branch=master)](https://github.com/kiwisheets/file-server) |

## Quick start

Note: This stack is designed to run using Docker/Docker swarm mode

Clone this repository recursively to get all submodules

    git clone --recursive https://github.com/kiwisheets/kiwisheets

Make sure to add `--recursive`

For a local development configuration, navigate to `./local-config` and see `.env.example`

    cp .env.example .env

To quickly get up and running, set the following variables inside the `.env` file

`S3_ENDPOINT`,
`AWS_ACCESS_KEY_ID`,
`AWS_SECRET_ACCESS_KEY`,
`S3_REGION`

These are required for the file server to function correctly.

The local config contains a package.json for handling scripts

To start the stack:

    npm run start-dev

To shutdown the stack:

    npm run stop-dev

## Modules
### Frontend
See the README inside this module for more info
