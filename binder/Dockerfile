FROM jupyter/r-notebook:latest

USER root

ARG JUPYTERHUB_VERSION=1.1.0
RUN pip install --trusted-host pypi.python.org --no-cache jupyterhub>=$JUPYTERHUB_VERSION

RUN apt-get update && apt-get install -y gcc
RUN jupyter nbextension enable --py --sys-prefix widgetsnbextension

WORKDIR /home/jovyan

USER jovyan