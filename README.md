# Python Project Cookiecutter

Python [cookiecutter](https://github.com/audreyr/cookiecutter) project template derived from the
one described in this [blogpost](https://sourcery.ai/blog/python-best-practices/) by Sourcery-AI,
with changes inspired by [janw/python-cookiecutter](https://github.com/janw/python-cookiecutter),
[GillesJ/python-project-pattern](https://github.com/GillesJ/python-project-pattern), and
[tim-fi/python_project_template](https://github.com/tim-fi/python_project_template).

Notable differences to the Sourcery-AI template:
- Excludes development enviroment tools from dev-dependencies

## Features
- Testing with [pytest](https://docs.pytest.org/en/latest/)
- Formatting with [black](https://github.com/psf/black)
- Import sorting with [isort](https://github.com/timothycrosley/isort)
- Static typing with [mypy](http://mypy-lang.org/)
- Linting with [flake8](http://flake8.pycqa.org/en/latest/)
- Git hooks that run all the above with [pre-commit](https://pre-commit.com/)
- Deployment ready with [Docker](https://docker.com/)
- Continuous Integration with [GitHub Actions](https://github.com/features/actions)

## Quickstart
```sh
# Install pipx
python3 -m pip install pipx
python3 -m pipx ensurepath

# Install pipenv using pipx
pipx install pipenv

# Install all dev environment tools using pipx
pipx install flake8
pipx install black
pipx install isort
pipx install mypy
pipx install pre-commit

# Use cookiecutter to create project from this template
pipx run cookiecutter gh:luksan/python-project-cookiecutter

# Enter project directory
cd <repo_name>

# Initialise git repo
git init

# Install dependencies
pipenv install --dev

# Setup pre-commit and pre-push hooks
pre-commit install -t pre-commit
pre-commit install -t pre-push
```
