# python-package-template

### Documentation
Example Project Structure for a Python / PyPI Project

### Installation
Note that this supports Python 3 *ONLY*

### Basic Usage

*Warning eggs are deprecated in favor of wheels, and not supported by pip.*

This project is a sample template used to aggregate the process of 
- Laying out a python project
- Using setuptools build system to 
    - to facilitate packaging Python projects
    - Python package and module definitions
    - Distribution package metadata
    - Project installation

Outline the process to 
- Create Python Eggs - a single-file importable distribution format
- Automatically include all packages in your source tree, without listing them individually in setup.py
- Automatically generate wrapper scripts or Windows (console and GUI) .exe files for any number of “main” functions in your project. (Note: this is not a py2exe replacement; the .exe files rely on the local Python installation.)

#### Command Reference
[https://setuptools.readthedocs.io/en/latest/setuptools.html#command-reference]

For example, to produce a source distribution, simply invoke:

```bash
python3 setup.py sdist
```

Detailed instructions to distribute a setuptools project can be found at Packaging project tutorials.
[https://packaging.python.org/tutorials/packaging-projects/#generating-distribution-archives]

Before you begin, make sure you have the latest versions of setuptools and wheel:
```bash
python3 -m pip install --user --upgrade setuptools wheel
```

To build a setuptools project, run this command from the same directory where setup.py is located:
```bash
python3 setup.py sdist bdist_wheel
```

This will generate distribution archives in the dist directory.

### Credits
Patrick Shiel:
[github.com/patrickshiel](https://github.com/patrickshiel)

### License

MIT License