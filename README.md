# JupyterLab extension template

[![Github Actions Status](https://github.com/jupyterlab/extension-template/workflows/CI/badge.svg)](https://github.com/jupyterlab/extension-template/actions/workflows/main.yml)

A [copier](https://copier.readthedocs.io) template for creating
a JupyterLab extension. Three kinds of extension are supported:
- _frontend_: Pure frontend extension written in TypeScript.
- _server_: Extension with frontend (in TypeScript) and backend (in Python) parts.
- _theme_: Theme for JupyterLab (using CSS variables).

## Use the template to create package

1. Install copier and some plugins.

```sh
pip install "copier>=7.1.0" jinja2-time
```

2. Go into the extension directory

```sh
mkdir myextension
cd myextension
```

3. Use copier to generate a package, following the prompts to fill all required information.

```
copier https://github.com/jupyterlab/extension-template .
```

If you'd like to generate a package for a older release, use the `--vcs-ref` option and give a tag or commit from this repository.

```sh
copier --vcs-ref v4.0.0 https://github.com/jupyterlab/extension-template
```

> If you are looking for a template compatible with JupyterLab version prior to 4.0.0, look at 
> the [cookiecutter template](https://github.com/jupyterlab/extension-cookiecutter-ts).

## A simple example

Your new extension includes a very simple example of a working extension. Use this example as a guide to build your own extension. Have a look at the [extension examples](https://github.com/jupyterlab/extension-examples) repository for more information on various JupyterLab features.
