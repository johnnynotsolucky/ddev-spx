[![add-on registry](https://img.shields.io/badge/DDEV-Add--on_Registry-blue)](https://addons.ddev.com)
[![tests](https://github.com/johnnynotsolucky/ddev-spx/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/johnnynotsolucky/ddev-spx/actions/workflows/tests.yml?query=branch%3Amain)
[![last commit](https://img.shields.io/github/last-commit/johnnynotsolucky/ddev-spx)](https://github.com/johnnynotsolucky/ddev-spx/commits)
[![release](https://img.shields.io/github/v/release/johnnynotsolucky/ddev-spx)](https://github.com/johnnynotsolucky/ddev-spx/releases/latest)

# DDEV Spx

## Overview

This add-on integrates [SPX](https://github.com/NoiseByNorthwest/php-spx) into your [DDEV](https://ddev.com/) project.

## Installation

```bash
ddev add-on get johnnynotsolucky/ddev-spx
ddev restart
```

After installation, make sure to commit the `.ddev` directory to version control.

## Usage

| Command | Description |
| ------- | ----------- |
| `ddev describe` | View service status and used ports for Spx |
| `ddev logs -s spx` | Check Spx logs |

## Advanced Customization

To change the Docker image:

```bash
ddev dotenv set .ddev/.env.spx --spx-docker-image="ddev/ddev-utilities:latest"
ddev add-on get johnnynotsolucky/ddev-spx
ddev restart
```

Make sure to commit the `.ddev/.env.spx` file to version control.

All customization options (use with caution):

| Variable           | Flag                 | Default                      |
|--------------------|----------------------|------------------------------|
| `SPX_DOCKER_IMAGE` | `--spx-docker-image` | `ddev/ddev-utilities:latest` |

## Credits

**Contributed and maintained by [@johnnynotsolucky](https://github.com/johnnynotsolucky)**
