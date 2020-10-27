# Introduction
Template repository for python package

Manuel steps to generate and publish the package to TestPyPI, documentation from [packaging.python](https://packaging.python.org/tutorials/packaging-projects/)

Generate distribution archives
```shell
python setup.py sdist bdist_wheel
```

Upload distribution archive to TestPyPI (a separate instance of the Python Package Index)
```shell
python -m twine upload --repository testpypi dist/*
```

# Installation
```shell
python -m pip install --index-url https://test.pypi.org/simple/ --no-deps mypkg128
```
or
```shell
pipenv install --pypi-mirror https://test.pypi.org/simple/ mypkg128
```

# Usage
```python
from mypkg128 import main
main.test()
```

# Code of Conduct

# History (changelog)
