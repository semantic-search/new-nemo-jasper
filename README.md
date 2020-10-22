## RUN IMAGE FROM GHCR

```sh
docker run -it --env-file .env --gpus all ghcr.io/semantic-search/new-nemo-jasper:latest

```

- Make sure you have `.env` file with following parameters

```.env
KAFKA_HOSTNAME=
KAFKA_PORT=
MONGO_HOST=
MONGO_PORT=
MONGO_DB=
MONGO_USER=
MONGO_PASSWORD=
KAFKA_CLIENT_ID=
KAFKA_USERNAME=
KAFKA_PASSWORD=
DASHBOARD_URL=
CLIENT_ID=151515
```

To build the docker image locally, run:

```git
    git clone --recurse-submodules https://github.com/semantic-search/new-nemo-jasper.git
```

```
docker build -t new-nemo-jasper .
```

```
docker run -it  --env-file .env --gpus all new-nemo-jasper
```
