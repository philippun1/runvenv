## runvenv

[![PyPI](https://img.shields.io/pypi/v/runvenv)](https://pypi.org/project/runvenv/)
[![Python](https://img.shields.io/pypi/pyversions/runvenv)](https://pypi.org/project/runvenv/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

Runs a script or module in a venv and forwards *any* parameter.
This includes non positional arguments like --help, --init, --path, --check, --requirements, etc.

With no parameters given this help will be shown. To only create a venv and not run anything
you can use the --init parameter. If the venv does not exist yet, it will create it and also install
all requirements in either reqirements.txt, .requirements.txt or .requirements.venv if available.

To check if a venv is already set up use the parameter --check. Depending on the status exit code is:
    0 = up-to-date
    1 = available but not up-to-date
    2 = not available

A custom venv path or requirements file can be configured via parameters.
