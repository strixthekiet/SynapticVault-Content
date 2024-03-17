---
tags:
  - CompSci/dev/backend/container/Docker/CLI
---
# docker run
### Description:
- Start container
- Can be from docker hub directly, when images are not downloaded
- Doesnt reuse image
### Synopis:
- `docker run [OPTIONS] IMAGE [COMMAND] [ARG...]`
### Options:
- `--name`
	- Assign a name to it
- `--detach`
	- Run container in background, no printing log
	- Print container ID
- `--publish`
	- Publish a container's port(s) to the host
	- Port forwarding