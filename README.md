# jupyterlab-favorites

[![Build Status](https://travis-ci.com/jupyterlab-contrib/jupyterlab-favorites.svg?branch=master)](https://travis-ci.com/jupyterlab-contrib/jupyterlab-favorites)

Add the ability to save favorite folders to JupyterLab for quicker browsing.

## Installation

### Prerequisites

* JupyterLab 3.x

### Install from pypi
```
python -m pip install "jupyterlab-favorites==3.0.0"
```

### Install from github
```
python -m pip install "git+https://github.com/jupyterlab-contrib/jupyterlab-favorites@v3.0.0#egg=jupyterlab_favorites"
```

### Install locally from a git checkout
```
git clone https://github.com/jupyterlab-contrib/jupyterlab-favorites.git
cd jupyterlab-favorites
pip install .
```

## Development

### Prerequisites

* An active `conda` environment with JupyterLab 3.x installed

### Install locally from a git checkout
```bash
git clone https://github.com/jupyterlab-contrib/jupyterlab-favorites.git
cd jupyterlab-favorites
pip install -ve .
```
This copies the frontend code for the extension into JupyterLab.

To keep the source code synced with JupyterLab, you can run the following:
```bash
jupyter labextension develop --overwrite .
```

To rebuild the extension manually after each change::
```bash
jlpm run build
```

To automatically rebuild after each change, run in a separate terminal:
```bash
jlpm run watch
```

## Older JupyterLab versions

### JupyterLab v2 Support

NPM install
```bash
jupyter labextension install jupyterlab-favorites@2.0.0
```

### Jupyterlab v1 Support

Via NPM:
```{bash}
jupyter labextension install jupyterlab-favorites@1.0.0
```

Or use the tagged 1.0.0 release at:
https://github.com/jupyterlab-contrib/jupyterlab-favorites/tree/v1.0.0

## Testing 
Download Firefox browser if not already installed: https://www.mozilla.org/en-US/firefox/new/

Install Selenium:
```bash
conda install -c conda-forge selenium
```
Install Pytest:
```bash
conda install -c anaconda pytest
```

Change directory to this repo after cloning
```bash
cd yourfolder/jupyterlab-favorites
```
Running test script:
```bash
./run_tests.sh
```
This will open jupyter lab and run available tests. 
Note: You will need to run in a clean jupyter environment (without existing favorites files) 
