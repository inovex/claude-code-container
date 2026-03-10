# docker-claude

Minimal Docker image for running Claude Code in a Debian-based development container.

## Build

```sh
mise run build
```

Or directly with Docker:

```sh
docker build . -t claude-container
```

## Run

Mount your current working directory into the container at `/home/dev/work`:

```sh
docker run -it -v "$PWD:/home/dev/work" ghcr.io/inovex/claude-code-container
```
