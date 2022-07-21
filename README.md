# flask-frontend-template

Minimal example demonstrating flask's templating functionality and how to define basic endpoint.

Do note that this is _NOT_ an example of a production-ready server.
It is meant as a gentle introduction to the basic concepts involved with creating an front-end or API with flask.

## Instructions

Prerequisites:

```bash
pip install flask
```

Run:

```bash
python main.py
```

or

```bash
./main.py
```

Visit the URL printed in your Terminal.
Your web app will be running on port `1337`.

Note: in containerized environments, you will need to bind to an IP which is accessible, which can be configured through editing `main.py` or by running the following (which will take precedence over the former):

```bash
flask run --host 0.0.0.0 [--port 1337]
```

When moving to a production server (e.g. `gunicorn` with `wsgi`), you will specify hosts and ports differently, and the settings in `main.py` will not be relevant since the entry-point will not be `main:__main__` but rather `main:app`
