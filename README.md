# Hackapp

## About

**Hackapp** consolidates [hackapp-client](https://github.com/evscott/hackapp-client) and [hackapp-api](https://github.com/evscott/hackapp-api) into submodule dependencies of a single repository to facilitate development using Docker-compose.

## Getting started

### Cloning the project

```
git clone --recursive git@github.com:evscott/hackapp.git
```

### Pulling submodule dependencies

```
git pull --recurse-submodules
```

## How to use

### Running Hackapp

```
docker-compose up --build
```

### Shutting down Hackapp

```
docker-compose down
```

## Cleanup

### Pruning docker volumes
```
docker volume prune
```

### Removing docker containers
```
docker rm $(docker ps -a -q)
```