# [General Purpose Template](./README.md) &middot; [![GitHub license]](./LICENSE) ![Test Action]

<!-- Table of Contents -->

- [Installation](#installation)
    - [For development](#for-development)
    - [For production](#for-production)
- [Environment Variables](#environment-variables)
- [Usage](#usage)
- [License](#license)

## Installation

The first step will be to clone the repo

```shell
git clone https://github.com/nightfury214/general-purpose-template.git
```

### For development

The requirements are:

* [Python] and [Poetry]

1. Install the dependencies
   ```shell
   poetry install
   ```

### For production

Using Docker is generally recommended (but not strictly required) because it abstracts away some additional set up work.

The requirements for Docker are:

* [Docker CE]
* [Docker Compose]
    * `pip install docker-compose`
    * This is only a required step for linux. Docker comes bundled with docker-compose on Mac OS and Windows.


## Environment Variables

To run this project, you will need to add the following environment variables.

| Variable | Description        | Default |
|----------|--------------------|---------|
| DEBUG    | Toggles debug mode | False   |

## Usage

Now you are done! You can run the project using

```shell
poetry run task start
```

or test the project using

```shell
poetry run task test
```

## License

Distributed under the MIT License. See [LICENSE](./LICENSE) for more information.

<!-- Packages Links -->

[docker ce]: https://docs.docker.com/install/
[docker compose]: https://docs.docker.com/compose/install/
[poetry]: https://python-poetry.org/docs/
[python]: https://www.python.org/downloads/

<!-- Shields.io links -->

[gitHub license]: https://img.shields.io/badge/license-MIT-blue.svg
[test action]: https://github.com/nightfury214/general-purpose-template/actions/workflows/test.yaml/badge.svg
