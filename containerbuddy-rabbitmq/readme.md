# RabbitMQ with Containerbuddy

[rabbitmq:3.6-management][rabbitmq] wrapped for use with [Containerbuddy][containerbuddy].

## Usage

* `docker pull j0hnsmith/containerbuddy-rabbitmq:latest`
* run [Consul][consul] somewhere
* set `ENV_NAME` and `CONSUL_HOST` env vars
* run `docker-compose up -d`
* visit the Consul http interface (default port 8500) and you'll see a service `rabbitmq_{ENV_NAME}`

See [docker-compose.yml][compose file].

[rabbitmq]: https://hub.docker.com/_/rabbitmq/
[containerbuddy]: https://github.com/joyent/containerbuddy
[compose file]: docker-compose.yml
[consul]: https://www.consul.io/
