# Opinionated template for Python projects

This template is built around the tools provided by [Astral](https://astral.sh/). Specifically, it uses `uv` (project management), `ruff` (linting and formatting) and `ty` (type checking). Their versions are pinned across local development and continuous integration via the [pre-commit](https://pre-commit.com/) configuration.

## Usage

After copying or recreating the template, the Python project can be managed by `uv`. It handles dependencies and executes tools, while automatically keeping the virtual environment in sync. Please refer to the [uv documentation](https://docs.astral.sh/uv/) for a complete overview.

### Examples

Add a dependency and run the template app.

```sh
uv add fastapi
uv run template 
```

Install pre-commit hooks and run them manually.

```sh
uvx pre-commit install
uvx pre-commit run --all-files
```

## Components

1. [Python project created by `uv init`](pyproject.toml)

2. [GitHub's `.gitignore` template](https://github.com/github/gitignore/blob/main/Python.gitignore)

3. [Pre-commit hooks for Astral tools](.pre-commit-config.yaml)

4. [Continuous integration workflow](.github/workflows/)
