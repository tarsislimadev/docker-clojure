# Docker Clojure

[![github/actions/workflow/status](https://img.shields.io/github/actions/workflow/status/brtmvdl/docker-clojure/docker-push.yml)](https://img.shields.io/github/actions/workflow/status/brtmvdl/docker-clojure/docker-push.yml) [![github/license](https://img.shields.io/github/license/brtmvdl/docker-clojure)](https://img.shields.io/github/license/brtmvdl/docker-clojure) [![github/stars](https://img.shields.io/github/stars/brtmvdl/docker-clojure?style=social)](https://img.shields.io/github/stars/brtmvdl/antify?style=social)

Para compilaçao e entrega de projetos escritos em clojure

Veja mais em [hub.docker.com/r/tmvdl/clojure](https://hub.docker.com/r/tmvdl/clojure)

## Como usar

Instalar o [Docker](https://docs.docker.com/engine/install/).

### Em ambiente de desenvolvimento

Criar um arquivo `docker-compose.yaml` na raiz do projeto com a imagem [tmvdl/clojure](https://hub.docker.com/r/tmvdl/clojure).

```yaml
version: '3'

services:
  app:
    image: tmvdl/clojure
    volumes:
      - .:/app
```

Subir o container para a construção do build

```bash
docker-compose up --build
```

### Em ambiente de produção

Executar como container do Docker

```sh
docker run tmvdl/clojure
```

## License

[MIT](./LICENSE) 
