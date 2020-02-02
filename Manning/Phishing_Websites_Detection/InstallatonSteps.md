# Installation Instructions for Windows 10

1. Create a folder 'project_name' and cd to the path.
2. Copy get-pip.py from <https://bootstrap.pypa.io/get-pip.py>
3. sudo python get-pip.py pip==19.3.1

```
pip install virtualenv virtualenvwrapper
```

```
virtualenv venv
```

```
cd venv\Scripts
```

## FAQ

Issue:
ImportError: cannot import name 'PackageFinder' from 'pip._internal.index'

Solution:
<https://github.com/pypa/pip/issues/7620>