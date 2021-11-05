Qt Advanced Docking System Shiboken Bindings
============================================

### Prepare the environment

1. Use virtualenv or (pyenv+)pipenv to create an environment for Shiboken
2. [Install Shiboken](https://doc.qt.io/qtforpython/shiboken6/gettingstarted.html) in the venv

```sh
pip install --index-url=http://download.qt.io/official_releases/QtForPython/ --trusted-host download.qt.io shiboken6 pyside6 shiboken6_generator
```

pyside6 and shiboken6 can be installed from pypi.org, but shiboken_generator cannot.

### Build with QtCreator

1. Use QtCreator to open the root CMakeLists.txt file
2. Configure the project for BUILD_SHIBOKEN=True; BUILD_EXAMPLES=False; PYTHON_INTERPRETER=/path/to/venv/python
3. Click Build

### TODO

1. Call a packager to wrap the output library in a Python package.
