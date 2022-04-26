# µlearn

_"micro·learn"_: the microframework for building and deploying machine learning services

## Build the Documentation

Until we release this into the wild, you'll have to build the docs locally.

First create and activate a virtual environment

```
python -m venv ~/ulearn_env
source ~/ulearn_env/bin/activate
```

Install requirements:

```
pip install -r requirements.txt -r requirements-dev.txt -r requirements-docs.txt
```

Make the documentation:

```
make -C docs clean html
```

Now you can open up `docs/_build/html/index.html` to view the docs.
