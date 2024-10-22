# taxi-example
This repository provides a collection of examples used to support STOR 674. *This repository is for teaching (lectures) and learning --- not everything is meant to be perfect!*

## file listing

## Runtime environment
### Docker and docker stacks project
*My* preferred method for cross platform data science (and quick demos). Prerequistes:
1. Install docker (it's available as free desktop program for windows and mac; cli for linux)
2. Start docker (you will get a fairly cryptic message if you proceed the cli arguement below if you skip this step). For windows and macos this is running the docker desktop program.
3. Start a container from the docker desktop program or a terminal environment.

## Get data
```
bash get_taxi.sh
```

## Perform datascience
### Docker Stacks: `datascience-notebook`
Using the docker stacks project datascience notebook. Directions [here](https://jupyter-docker-stacks.readthedocs.io/en/latest/#example-2).
```
docker run -it --rm -p 8888:8888 -v "${PWD}":/home/jovyan/work quay.io/jupyter/datascience-notebook:2024-08-30
```
### Docker Stacks: `pytorch-notebook`
For the pytorch examples we use the [pytorch notebook](https://jupyter-docker-stacks.readthedocs.io/en/latest/using/selecting.html#jupyter-pytorch-notebook) which can be launched as before
```
docker run -it --rm -p 8888:8888 -v "${PWD}":/home/jovyan/work quay.io/jupyter/pytorch-notebook
```
### Anaconda
`#TODO: provide details on doing the same with anaconda; loosely, `
