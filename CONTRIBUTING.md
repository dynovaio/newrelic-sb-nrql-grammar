# How to contribute to this project

> If you are interested in contributing to the development and maintenance of
> this package, it is recommended that you use [poetry][href:poetry]
> for dependency management and [pyenv][href:pyenv] for
> python version management.

## Environment

Clone the project

```bash
git clone https://github.com/dynovaio/newrelic-sb-nrql-parser-python.git
cd newrelic-sb-nrql-parser-python
```

Install the rquited python versions

```bash
pyenv install $(cat .python-version)
```

Install the dependencies

```bash
poetry env use $(head -n 1 .python-version)
poetry install
```

## Testing and coverage

You can run the tests with poetry

```bash
poe test
poe test:coverage
```

In case you want to run the tests in all versions you can use [`tox`](https://tox.readthedocs.io/en/latest/)

## Do you want to send a PR?

Before making your first commit and submitting your pull request, run

```bash
poetry run pre-commit install
```

Then do your commits on a regular basis.

## Code of Conduct

> Please note that this project is published with a Code of Conduct for
> collaborators. By participating in this project, you agree to abide by its
> terms.

For more information, please refer to the
[Code of Conduct ↗][href:code_of_conduct].

[href:poetry]: https://python-poetry.org
[href:pyenv]: https://github.com/pyenv/pyenv
[href:code_of_conduct]: CODE_OF_CONDUCT.md
