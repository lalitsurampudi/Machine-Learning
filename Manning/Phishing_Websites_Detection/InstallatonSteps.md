# Installation Instructions for Windows 10

Create a directory for the project and cd to the directory path.
```
mkidr Phishing_Websites_Detections
cd Phishing_Websites_Detections
```
Copy get-pip.py from <https://bootstrap.pypa.io/get-pip.py>

Install pip
```
python get-pip.py pip==19.3.1
```

Install packages `virtualenv` and `virtualenvwrapper`
```
pip install virtualenv virtualenvwrapper
```
Create virtual environment 
```
virtualenv venv
```
Activate virtual environment
```
activate venv\Scripts
```
Install packages
```
pip install -r "requirements.txt"
```


## FAQ

Issue:
ImportError: cannot import name 'PackageFinder' from 'pip._internal.index'

Solution:
<https://github.com/pypa/pip/issues/7620>