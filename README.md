# Panoptes Client

This package is the Python SDK for
[Panoptes](https://github.com/zooniverse/Panoptes), the platform behind the
[Zooniverse](https://www.zooniverse.org/). This module is intended to allow
programmatic management of projects, providing high level access to the API for
common project management tasks.

[Full documentation is available at Read the
Docs](http://panoptes-python-client.readthedocs.io/).

## Installation

Install latest stable release:

```
$ pip install panoptes-client
```

Or for development or testing, you can install the development version directly
from GitHub:

```
$ pip install -U git+git://github.com/zooniverse/panoptes-python-client.git
```

Upgrade an existing installation:

```
$ pip install -U panoptes-client
```

## Usage Examples

Create a project:

```python
from panoptes_client import Panoptes, Project

Panoptes.connect(username='example', password='example')

new_project = Project()
new_project.display_name = 'My new project'
new_project.description = 'A great new project!'
new_project.primary_language = 'en'
new_project.private = True
new_project.save()
```

See the documentation for [additional
examples](http://panoptes-python-client.readthedocs.io/en/latest/user_guide.html#usage-examples).
