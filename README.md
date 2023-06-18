# Pre-commit demo
Repo for demoing pre-commit hooks.

* Pre-commit hooks configuration: [.pre-commit-config.yaml](.pre-commit-config.yaml)
* Other configuration options and dependencies: [pyproject.toml](pyproject.toml)

## Installation
### Prerequisites
- [Poetry](https://python-poetry.org/docs/#installation)

### Getting started
Run poetry install to install pre-commit and the hooks in this repo:

```bash
poetry install
```

## Usage
Create a new git repo:

```bash
git init
```

Install pre-commit hooks:

```bash
pre-commit install
```

Run pre-commit to run the hooks on all files:

```bash
pre-commit run --all-files
```

Run pre-commit on staged files only:

```bash
pre-commit run
```

(**Note**: If you have included wily in your pre-commit hooks, you'll need to configure wily before running the hooks, with `python -m wily setup`)
