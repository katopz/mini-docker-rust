# mini-docker-rust ![docker-github-action](https://github.com/kpcyrd/mini-docker-rust/actions/workflows/test-docker.yml/badge.svg)

Very small rust docker image.

This is an example project on how to build very small docker images for a rust project. The resulting image for a working hello world was about 6.01MB during my tests.

This repo is trying to keep the docker overhead to a minimum without sacrificing performance or the usability implications of using `FROM scratch`. If you want to reduce the binary size further you might be interested in [johnthagen/min-sized-rust](https://github.com/johnthagen/min-sized-rust).

## See for yourself

You don't need to install anything besides docker.

1. Build with `docker build -t mini-docker-rust .`
1. and run with `docker run -p 8080:8080 mini-docker-rust`.
1. `curl http://0.0.0.0:8080` or `open http://localhost:8080`.

## Annotated docker file

See [Dockerfile](Dockerfile).
