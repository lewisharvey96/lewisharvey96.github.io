+++
title = 'Ruffly'
date = 2024-08-13T09:12:17+01:00
+++

Ruffly is a cli tool written in Python to copy configuration for tools such as [ruff](https://pypi.org/project/ruff/) from a source .toml. I typically use a consistent set of tool configurations, think line length, across projects and always ended up copying and pasting from one repo to another. This was a pretty "rough" process, sometimes I would grab more than I wanted and sometime I'd grab configuration for a tool I didn't need. Since most of the settings were for ruff:  *"ruffly"* seemed a fitting name. This simple package just makes this manual process a litte quicker and adds default configuration if you don't have .toml in mind to copy from.

This was the first package I've published to PyPi and a great learning experience. The project uses Github actions and setuptools to build the package and publish it to PyPi.

The package can be found on PyPi [here](https://pypi.org/project/ruffly/), and the repository on GitHub [here](https://github.com/lewisharvey96/ruffly). Below is the key info from the README.

# Ruffly 🐍

### Usage

Cli tool to add common config to pyroject.toml.

Basic usage:
```commandline
cd/project/with/pyrojecttoml ruffly
```
will add default config to pyproject.toml found in working directory.

Additional arguments:

- ```--dst``` The path to the target pytroject.toml to modify
- ```--src``` The path to the source pytroject.toml to copy from (can be url)
- ```--only-existing``` Only copies config for tools that exist int the target pyproject.toml
- ```--tools``` A list of tools to copy config for
- ```--dry-run``` Only prints the changes that would be made

Current tools supported:
- ruff
- mypy
- pytest
- coverage
- poe (poethepoet)

### Installation

```commandline
pip install ruffly
```
