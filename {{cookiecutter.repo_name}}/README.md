# {{cookiecutter.project_name}}

## Setup
```sh
# Install dependencies
pipenv install --dev

# Install development tools, if not already installed
pipx install flake8
pipx inject flake8 flake8-bugbear
pipx install black
pipx install isort
pipx install mypy
pipx install pre-commit

# Setup pre-commit and pre-push hooks
pre-commit install -t pre-commit
pre-commit install -t pre-push
```

## Credits
This package was created with Cookiecutter and the
[luksan/python-project-cookiecutter](https://github.com/luksan/python-project-cookiecutter)
project template.
