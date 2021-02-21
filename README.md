# jupyter

Мое персональное

Документация по [Jupyter Docker Stacks on ReadTheDocs](http://jupyter-docker-stacks.readthedocs.io/en/latest/index.html)

Docker image: `docker pull jtprog/jupyter:latest`

docker-compose:
```yaml
version: "3"

services:
  mynotes:
    image: jtprog/jupyter
    ports:
      - "127.0.0.1:8888:8888"
    volumes:
      - ./data:/home/jtprogru/work:rw
    restart: always
```
