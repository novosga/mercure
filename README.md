# Mercure

Custom NovoSGA Mercure docker image, on top of Mercure v0.11.

## Building

```sh
docker build -t novosga/mercure:v0.11 .
```

## Running

```sh
docker run --rm \
    -e SERVER_NAME=":3000" \
    -e MERCURE_PUBLISHER_JWT_KEY="!ChangeMe!" \
    -e MERCURE_EXTRA_DIRECTIVES="anonymous 1; cors_origins *" \
    --name mercure \
    novosga/mercure:v0.11
```
