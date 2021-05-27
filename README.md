# Cookiecutter Example

Simple cookiecutter template to showcase the usage of [cruft](https://github.com/cruft/cruft).

## Features

* [Poetry]: Dependency management and packaging
* Github Actions: Ready for Continous Integration testing
## Quickstart

Get the latest version of [Cruft].
I recommend [pipx] to install it into a global isolated environment.

```sh
pipx install cruft
```

Generate a new python package

```sh
cruft create <URL>
cd <chosen project slug>
git init
git add .
git commit -m "feat: initial project structure"
```

### Autoupdate template

This cookiecutter template comes with an auto update feature if the project was created using [cruft].
A GitHub action automatically checks for updates and creates a pull request.

It is required to add a [personal access token](https://docs.github.com/en/free-pro-team@latest/github/authenticating-to-github/creating-a-personal-access-token)
as github secret to the repository (named `AUTO_UPDATE_GITHUB_TOKEN`).
While creating the access token, the following permissions have to be granted

* repo
* workflow

[Cruft]: https://github.com/cruft/cruft
[Poetry]: https://python-poetry.org/
