FROM jupyter/r-notebook:latest

USER root

RUN apt-get update && apt-get install -y gcc
RUN jupyter nbextension enable --py --sys-prefix widgetsnbextension

WORKDIR /home/jovyan

USER jovyan