# Docker - KonaKart & Dynatrace

This repository is designed to hold my personal configurations for my environment. It is not expected to work on any other environment and has more than a few hard-coded values throughout.

This is a 'fork' of work done by [@beantoast](https://github.com/beantoast)

## Dependencies:

* [dynatrace 6.3](https://www.dynatrace.com/)
* [dynatrace_docker](https://github.com/Dynatrace/Dynatrace-Docker)
* [konakart-8.1.0.0](http://www.konakart.com/kits/8.1.0.0/KonaKart-8.1.0.0-Linux-Install-64)
* [haproxy](http://www.haproxy.org/)
* [docker](https://www.docker.com/)
* [docker-compose](https://docs.docker.com/compose/)

## Configuration

I'm sure I'm forgetting things...

* Konakart downloaded and in `/app` named `konakart-installation`.
* Dynatrace agent downloaded and in `/app` named `dynatrace-agent-6.3.0.1305-unix.jar`.

## Usage

After accounting for dependencies. I did the following.

`# docker-compose build`

Then start it up.

`# docker-compose up`
