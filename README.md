# CircleCI Node Image

[![Docker Pulls](https://img.shields.io/docker/pulls/parpe/circleci-node-image.svg?style=flat-square)](https://hub.docker.com/r/parpe/circleci-node-image/)
[![Docker Stars](https://img.shields.io/docker/stars/parpe/circleci-node-image.svg?style=flat-square)](https://hub.docker.com/r/parpe/circleci-node-image/)
[![Docker Automated build](https://img.shields.io/docker/automated/parpe/circleci-node-image.svg?style=flat-square)](https://hub.docker.com/r/parpe/circleci-node-image/)
[![Docker Build Status](https://img.shields.io/docker/build/parpe/circleci-node-image.svg?style=flat-square)](https://hub.docker.com/r/parpe/circleci-node-image/)

An image with node.js to run tests in the CircleCI 

## Components

- Common tools used in development and CI are installed e.g. `git`, `ssh`, `tar`, `ca-certificates`, `curl`, `wget`.
- Docker tools: latest `docker`, `docker-compose`, and `dockerize` are installed
- Bonus tools: `jq1.5`, `awscli`
- Use a `root` user by default

## Usage
`parpe/circleci-node-image:<version>`

This is the defacto image. If you are unsure about what your needs are, you probably want to use this one for common tools.

`parpe/circleci-node-image:<version>-browsers`

This image makes browser testing easier. It extends the defacto image and installs Firefox and Chrome/chromedriver and configure them to run in a chrontainzied environment

## Stable Versions

| Common  | Browser Testing |
| ------------- | ------------- |
| 8.9.4  | 8.9.4-browsers  |

## Unstable Versions

| Common  | Browser Testing |
| ------------- | ------------- |
| 8.9.4-dev  | 8.9.4-browsers-dev  |