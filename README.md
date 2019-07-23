# Docker image for MAGIC (Markov Affinity-based Graph Imputation of Cells)

Markov Affinity-based Graph Imputation of Cells (MAGIC) is an algorithm for denoising high-dimensional data most commonly applied to single-cell RNA sequencing data. MAGIC learns the manifold data, using the resultant graph to smooth the features and restore the structure of the data.
The software is available on https://github.com/KrishnaswamyLab/MAGIC


## Docker installation
To install docker follow the instructions in the links below depending on your operating system:
- CentOS: https://docs.docker.com/install/linux/docker-ce/centos/
- Debian: https://docs.docker.com/install/linux/docker-ce/debian/
- Fedora: https://docs.docker.com/install/linux/docker-ce/fedora/
- Ubuntu: https://docs.docker.com/install/linux/docker-ce/ubuntu/
- MacOS: https://docs.docker.com/docker-for-mac/install/
- Windows: https://docs.docker.com/docker-for-windows/install/


## Pulling Docker Image
Once docker is installed, the next step is to pull the [scmatch](https://hub.docker.com/r/biagii/magic) image from dockerhub using the following command:
```
docker pull biagii/magic
```


## Running image
```
docker run -it --rm --name [ANY_NAME] -v /server/path/:/docker/path biagii/magic python
```


## Help
This docker image is based on MAGIC tool developed by David van Dijk. Any doubt about how to use the parameters of the tool can be found in https://github.com/KrishnaswamyLab/MAGIC and further details in the original [paper](https://www.cell.com/cell/fulltext/S0092-8674(18)30724-4).

Any questions in Docker image contact the developer by email: biagi@usp.br
