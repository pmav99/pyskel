## skeleton for python projects

### Quickstart

#### activate a virtualenv Python3.7

```
python3.7 -mvenv venv
source venv/bin/activate
```

#### Install dependencies and setup pre-commit

```
poetry update
poetry install
pre-commit install
```

#### Rename your package!

If your package is going to be named `foo`:

```
mv mypackage foo
sed -i .bumpversion.cfg 's/my_package/foo/g'
sed -i .pyproject.toml 's/my_package/foo/g'
```
