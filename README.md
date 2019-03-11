# Docker Fluentd forwarder for LogSense

Run you Fluentd forwader by the Docker Compose:

```$ docker-compose up -d```

Then to use your Fluentd forwarder by Docker containers you need to specify log-driver options for them:

```$ docker run --log-driver=fluentd --log-opt fluentd-address=localhost:24224 nginx```

... or to set those options in the docker deamon configuration.
