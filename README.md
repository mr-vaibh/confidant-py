# Confidant-Py

Multi platform scalable environment variables manager

## Installation

```sh
pip install confidant-py
```

## Usage

```python
from confidant_py.loader import ConfidantLoader

loader = ConfidantLoader()
envs = loader.get_envs()
print(envs)
```


## **4. Publish to PyPI**
### Install necessary tools:
```sh
pip install setuptools wheel twine
```

### Build the package

```sh
python setup.py sdist bdist_wheel
```

### Upload to PyPI:

```sh
twine upload dist/*
```

### Updating the package

Bump the version in `setup.py` (e.g., 0.1.1).

```sh
python setup.py sdist bdist_wheel
twine upload dist/*
```