# uv-flask-example

An example Flask project using uv.

## Getting started

Run the server:

```console
$ uv run flask --app hello run
 * Serving Flask app 'hello'
 * Debug mode: off
WARNING: This is a development server. Do not use it in a production deployment. Use a production WSGI server instead.
 * Running on http://127.0.0.1:5000
Press CTRL+C to quit
```

Then check out the [hello world page](http://127.0.0.1:5000) in your browser.

## Creating a new Flask project

First, create a new project with uv:

```console
$ uv init uv-flask-example
$ cd uv-flask-example
```

Add a dependency on flask:

```console
$ uv add flask
```

Then, edit `hello.py` to match Flask's [minimal application
example](https://flask.palletsprojects.com/en/3.0.x/quickstart/#a-minimal-application).

```python
from flask import Flask

app = Flask(__name__)

@app.route("/")
def hello_world():
    return "<p>Hello, World!</p>"
```
