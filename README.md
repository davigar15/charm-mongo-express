<!-- Copyright 2021 Canonical Ltd.
See LICENSE file for licensing details. -->

# mongo-express-operator

[![codecov](https://codecov.io/gh/davigar15/charm-mongo-express/branch/main/graph/badge.svg?token=QO02OEH639)](https://codecov.io/gh/davigar15/charm-mongo-express)
[![code style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black/tree/main)
[![Run-Tests](https://github.com/davigar15/charm-mongo-express/actions/workflows/ci.yaml/badge.svg)](https://github.com/davigar15/charm-mongo-express/actions/workflows/ci.yaml)

## Description

Mongo express is a web-based MongoDB admin interface written in Node.js, Express.js, and Bootstrap3.

## Usage

Build the charm:

```shell
charmcraft build
```

Deploy charm:

```shell
juju deploy ./mongo-express_ubuntu-20.04-amd64.charm --resource mongo-express=mongo-express:0.54.0
```

The web ui will be available at port 8081.

## Actions

Get the UI credentials:

```shell
juju run-action mongo-express/0 get-credentials --wait
```

## OCI Images

- [mongo-express](https://hub.docker.com/layers/mongo-express/library/mongo-express/0.54.0/images/sha256-5bf035faae450d68247fb4364dda361bde60f89de185c179a6eda14e2aa731dc?context=explore)

## Contributing

Please see the [Juju SDK docs](https://juju.is/docs/sdk) for guidelines
on enhancements to this charm following best practice guidelines, and
`CONTRIBUTING.md` for developer guidance.
