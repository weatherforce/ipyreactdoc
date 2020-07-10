# Quickstart

## Installation
This guide assumes that you are using a linux based system.

## System requirements
- npm
- python3 (it has been tested using python 3.7)
- pip

## Building JavaScript
This builds the react javascript.

```bash
npm install -C nbextensions_srcs && npm run dev -C nbextensions_srcs
```
You should now have a nbextensions_dists folder

### Installing Python packages
For installing the python packages an we recommend using a virtual environment
```bash
python3 -m venv ipyreactvenv
source ipyreactvenv/bin/activate
pip install -r dev_requirements.txt
pip install .
```

## Running Jupyter notebook
In the same terminal as your virtual environment run:

```bash
jupyter notebook examples/slider.ipynb
```

There are other example ipynb which can be found in the examples folder.

If you want to develop your own widget using this project, you can refer yourself to the
[custom-widget](make-a-widget.md) section.
