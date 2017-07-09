# Whistleblower

Follow [@RosieDaSerenata](https://twitter.com/RosieDaSerenata) to get Brazilian Chamber of Deputies' updates in your timeline.

## Setup

Install [Docker](https://www.docker.com) and [Docker Compose](https://docs.docker.com/compose/).

```console
$ git clone --recursive git@github.com:Irio/whistleblower.git
$ cd whistleblower
$ cp .env.example .env
$ docker-compose build
```

## Running

```console
$ docker-compose run worker python rosie/rosie.py run chamber_of_deputies data --years=2017,2016
$ docker-compose up
```

## Testing

```console
$ docker-compose run worker python -m unittest discover tests
```
