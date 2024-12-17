# Docling Haystack converter

[![PyPI version](https://img.shields.io/pypi/v/docling-haystack)](https://pypi.org/project/docling-haystack/)
[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/docling-haystack)](https://pypi.org/project/docling-haystack/)
[![Poetry](https://img.shields.io/endpoint?url=https://python-poetry.org/badge/v0.json)](https://python-poetry.org/)
[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
[![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
[![Pydantic v2](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/pydantic/pydantic/main/docs/badge/v2.json)](https://pydantic.dev)
[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
[![License MIT](https://img.shields.io/github/license/DS4SD/docling)](https://opensource.org/licenses/MIT)

A [Docling](https://github.com/DS4SD/docling) converter integration for
[Haystack](https://github.com/deepset-ai/haystack/).

## Installation

Simply install `docling-haystack` from your package manager, e.g. pip:
```bash
pip install docling-haystack
```

## Usage

Basic usage in a Haystack pipeline looks as follows:

```python
from haystack import Pipeline
from docling_haystack.converter import DoclingConverter

idx_pipe = Pipeline()
# ...
converter = DoclingConverter()
idx_pipe.add_component("converter", converter)
# ...
```

For end-to-end usage samples check out the [examples](examples/).
