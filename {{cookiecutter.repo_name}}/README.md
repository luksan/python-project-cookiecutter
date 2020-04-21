# {{cookiecutter.project_name}}

## Setup
```sh
# Install dependencies
pipenv install --dev

# Setup pre-commit and pre-push hooks
pipenv run pre-commit install -t pre-commit
pipenv run pre-commit install -t pre-push
```

## Credits
This package was created with Cookiecutter and the
[luksan/python-project-cookiecutter](https://github.com/luksan/python-project-cookiecutter)
project template.
