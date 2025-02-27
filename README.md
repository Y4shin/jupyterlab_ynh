<!--
N.B.: This README was automatically generated by https://github.com/YunoHost/apps/tree/master/tools/README-generator
It shall NOT be edited by hand.
-->

# JupyterLab for YunoHost

[![Integration level](https://dash.yunohost.org/integration/jupyterlab.svg)](https://dash.yunohost.org/appci/app/jupyterlab) ![Working status](https://ci-apps.yunohost.org/ci/badges/jupyterlab.status.svg) ![Maintenance status](https://ci-apps.yunohost.org/ci/badges/jupyterlab.maintain.svg)  
[![Install JupyterLab with YunoHost](https://install-app.yunohost.org/install-with-yunohost.svg)](https://install-app.yunohost.org/?app=jupyterlab)

*[Lire ce readme en français.](./README_fr.md)*

> *This package allows you to install JupyterLab quickly and simply on a YunoHost server.
If you don't have YunoHost, please consult [the guide](https://yunohost.org/#/install) to learn how to install it.*

## Overview

JupyterLab is the next-generation user interface for Project Jupyter offering all the familiar building blocks of the classic Jupyter Notebook (notebook, terminal, text editor, file browser, rich outputs, etc.) in a flexible and powerful user interface. JupyterLab will eventually replace the classic Jupyter Notebook.


**Shipped version:** 3.5.2~ynh1

**Demo:** https://mybinder.org/v2/gh/jupyterlab/jupyterlab-demo/master?urlpath=lab/tree/demo

## Screenshots

![Screenshot of JupyterLab](./doc/screenshots/jupyterlab.png)

## Disclaimers / important information

## Updating configuration files

Install the new version of the app with:

```bash
sudo yunohost app install https://github.com/YunoHost-Apps/jupyterlab_ynh/tree/testing  
```

Navigate to the installation path (`/opt/jupyterlab` by default), and run :

```bash
pipenv shell
```

You are now in the virtual environment of jupyterlab. You can execute these two commands:

- To generate the `jupyterhub_config.py` file:

```bash
jupyterhub --generate-config
```

- To generate the `jupyter_notebook_config.py` file:

```bash
jupyter notebook --generate-config
cp $HOME/.jupyter/jupyter_notebook_config.py ./
```

You can now update the old template files with the new one.

## Documentation and resources

* Official app website: <https://jupyter.org>
* Official admin documentation: <https://jupyterlab.readthedocs.io/en/stable/>
* Upstream app code repository: <https://github.com/jupyterhub/jupyterhub>
* YunoHost documentation for this app: <https://yunohost.org/app_jupyterlab>
* Report a bug: <https://github.com/YunoHost-Apps/jupyterlab_ynh/issues>

## Developer info

Please send your pull request to the [testing branch](https://github.com/YunoHost-Apps/jupyterlab_ynh/tree/testing).

To try the testing branch, please proceed like that.

``` bash
sudo yunohost app install https://github.com/YunoHost-Apps/jupyterlab_ynh/tree/testing --debug
or
sudo yunohost app upgrade jupyterlab -u https://github.com/YunoHost-Apps/jupyterlab_ynh/tree/testing --debug
```

**More info regarding app packaging:** <https://yunohost.org/packaging_apps>
