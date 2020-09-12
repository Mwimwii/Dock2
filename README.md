<p align="center">
  <img src="media/logo.jpg" >
</p>

![License](https://img.shields.io/badge/license-MIT-lightgrey.svg)
![Python version](https://img.shields.io/badge/python-3.x-blue.svg)

This is a simple wrapper for interacting with h2cs drivers (HTTP2 ClearText)

## 🔧 Installation

Run the following to install:

```python
pip install Dock2
```

You need to download the h2cs driver into your **working directory** in order
for this to function properly

### Supported Drivers

| Driver | Author                                      | Download                                                                                  |
| ------ | ------------------------------------------- | ----------------------------------------------------------------------------------------- |
| H2CS   | [the-bumble](https://github.com/the-bumble/ | [Download](https://raw.githubusercontent.com/BishopFox/h2csmuggler/master/h2csmuggler.py) |

## Usage

```python
import Dock2

#  Upgrade function
result = Dock2.upgrade('www.example.com', 'driver.py')
print(result)

# Do anything else, pass arguments h2cs returns byte string
 result =  Dock2.cmd('-x https://edgeserver -i dirs.txt http://localhost/', 'driver')
 print(result)
```

[More information regarding utility of the driver can be found here (H2CS Author)](https://github.com/BishopFox/h2csmuggler)

# Developing Dock2

To install Dock2, along with all the tools you need to develop and run tests,
run the following in your virtualenv:

```bash
$ pip install -e .[dev]
```
