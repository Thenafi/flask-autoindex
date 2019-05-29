[![Build Status](https://travis-ci.org/general03/flask-autoindex.svg?branch=master)](https://travis-ci.org/general03/flask-autoindex)
[![Maintainability](https://api.codeclimate.com/v1/badges/869c538c7fe4f09a5e72/maintainability)](https://codeclimate.com/github/general03/flask-autoindex/maintainability)
[![Test Coverage](https://api.codeclimate.com/v1/badges/869c538c7fe4f09a5e72/test_coverage)](https://codeclimate.com/github/general03/flask-autoindex/test_coverage)

A mod_autoindex for Flask

## Requirements

* Flask
* Python 3

## Usage

```
import os.path
from flask import Flask
from flask_autoindex import AutoIndex

app = Flask(__name__)
AutoIndex(app, browse_root=os.path.curdir)

if __name__ == '__main__':
    app.run()
```

## Test

`python setup.py test`