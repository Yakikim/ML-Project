# Jupyter Notebook Data Science Stack

[![docker pulls](https://img.shields.io/docker/pulls/jupyter/datascience-notebook.svg)](https://hub.docker.com/r/jupyter/datascience-notebook/)
[![docker stars](https://img.shields.io/docker/stars/jupyter/datascience-notebook.svg)](https://hub.docker.com/r/jupyter/datascience-notebook/)
[![image size](https://img.shields.io/docker/image-size/jupyter/datascience-notebook/latest)](https://hub.docker.com/r/jupyter/datascience-notebook/ "jupyter/datascience-notebook image size")

GitHub Actions in the <https://github.com/jupyter/docker-stacks> project builds and pushes this image to Docker Hub.

Please visit the project documentation site for help to use and contribute to this image and others.

- [Jupyter Docker Stacks on ReadTheDocs](https://jupyter-docker-stacks.readthedocs.io/en/latest/index.html)
- [Selecting an Image :: Core Stacks :: jupyter/datascience-notebook](https://jupyter-docker-stacks.readthedocs.io/en/latest/using/selecting.html#jupyter-datascience-notebook)


```
docker run -d \
  -it \
  --rm \
  -p 10000:8888 \
  --name dataScienceContainer \
  -v "$(pwd)"/target:/app \
  --mount type=bind,source="${PWD}"/work/,target=/home/jovyan/work \
  data_notebook:jun-2023 
```