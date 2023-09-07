{% set is_open_source = cookiecutter.open_source_license != 'Not open source' -%}
# {{ cookiecutter.project_name }}

{% if is_open_source %}
[![pypi](https://img.shields.io/pypi/v/{{ cookiecutter.project_slug }}.svg)](https://pypi.org/project/{{ cookiecutter.project_slug }}/)
[![python](https://img.shields.io/pypi/pyversions/{{ cookiecutter.project_slug }}.svg)](https://pypi.org/project/{{ cookiecutter.project_slug }}/)
[![Build Status](https://github.com/{{ cookiecutter.github_username }}/{{ cookiecutter.project_slug }}/actions/workflows/dev.yml/badge.svg)](https://github.com/{{ cookiecutter.github_username }}/{{ cookiecutter.project_slug }}/actions/workflows/dev.yml)
[![codecov](https://codecov.io/gh/{{ cookiecutter.github_username }}/{{ cookiecutter.project_slug }}/branch/main/graphs/badge.svg)](https://codecov.io/github/{{ cookiecutter.github_username }}/{{ cookiecutter.project_slug }})

{% else %}
{% endif %}

{{ cookiecutter.project_short_description }}

{% if is_open_source %}
* Documentation: <https://{{ cookiecutter.github_username }}.github.io/{{ cookiecutter.project_slug }}>
* GitHub: <https://github.com/{{ cookiecutter.github_username }}/{{ cookiecutter.project_slug }}>
* PyPI: <https://pypi.org/project/{{ cookiecutter.project_slug }}/>
* Free software: {{ cookiecutter.open_source_license }}
{% endif %}

## Features

* TODO

## Credits

This package was generated using [Cookiecutter](https://github.com/audreyr/cookiecutter) with the [danibene/cookiecutter-pypackage](https://github.com/danibene/cookiecutter-pypackage) project template. It has its origins in the following templates:

- [audreyfeldroy/cookiecutter-pypackage](https://github.com/audreyfeldroy/cookiecutter-pypackage): The original project.

- [waynerv/cookiecutter-pypackage](https://github.com/waynerv/cookiecutter-pypackage)

- [zillionare/python-project-wizard](https://github.com/zillionare/python-project-wizard)

- [luiscberrocal/cookiecutter-pypackage](https://github.com/luiscberrocal/cookiecutter-pypackage)

- [danibene/cookiecutter-pypackage](https://github.com/danibene/cookiecutter-pypackage): The latest iteration of the template, incorporating the changes from the previous forks.
