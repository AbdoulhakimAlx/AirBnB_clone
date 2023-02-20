# W3C validator for Holberton School

For HTML and CSS files.

Based on 2 APIs:

- https://validator.w3.org/nu/
- http://jigsaw.w3.org/css-validator/validator

## Installation
1. Clone this repo
```sh
git clone https://github.com/holbertonschool/W3C-Validator.git
```

2. Run shell script (see example in [usage](#usage) section below)

## Usage:

Simple file:

```sh
./w3c_validator.py index.html
```

Multiple files:

```sh
./w3c_validator.py index.html header.html styles/common.css
```

All errors are printed in `STDERR`; Exit status = # of errors (0 on success)


## References

https://developer.mozilla.org/en-US/

## Troubleshooting

- Error: `bad interpreter: No such file or directory`
If you get this error you might not have Python installed correctly; or the system [PATH](https://en.wikipedia.org/wiki/PATH_(variable)) might not be updated to reflect the installed Python version.

Assuming that Python 3 is indeed installed, you can try to run it like so:
```
python3 w3c_validator.py index.html
```
- Error: `ModuleNotFoundError: No module named 'requests'`
If you get this error you do not have the module `requests` installed in your system.

You can install `requests` using pip:
```
python3 -m pip install requests
```

If you don't have `pip` installed, you can get it [here](https://pypi.org/project/pip/).
