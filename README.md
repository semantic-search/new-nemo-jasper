## RUN IMAGE FROM GHCR

```sh
docker run -it --env-file .env --gpus all ghcr.io/semantic-search/jasper:latest

```


To build the docker image locally, run:

```git
    git clone --recurse-submodules https://github.com/semantic-search/new-nemo-jasper.git
```

```
docker build -t jasper .
```

```
docker run -it  --env-file .env --gpus all jasper
```
