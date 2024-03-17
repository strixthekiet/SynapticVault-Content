---
tags:
  - CompSci/dev/backend/container/Docker
---
# Dockerfile
### Description:
- https://docs.docker.com/engine/reference/builder/
- Works layer by layer, data are used in the next layer
- Start from the least likely to be changed first
- Next update uses a last update and add the differences as a layer
	- much smaller file size
### FROM
- Base image, from docker hub
- A valid Dockerfile must start with a `FROM` instruction. 
- The image can be any valid image.
	- `FROM python:3.7`
### COPY
- Copy individual file from source code to image or COPY .  .
### WORKDIR
- Equivalent to `cd`
- The `WORKDIR` instruction sets the working directory for any `RUN`, `CMD`, `ENTRYPOINT`, `COPY` and `ADD`instructions that follow it in the Dockerfile. 
- If the `WORKDIR` doesn't exist, it will be created even if it's not used in any subsequent Dockerfile instruction.
	- `WORKDIR /app`
- 
### RUN
- Run in shell
### ENV
- Environment variable
### CMD
- Last command
- Use it for starting the app