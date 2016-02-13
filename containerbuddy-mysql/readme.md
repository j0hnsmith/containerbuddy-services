# MySQL with Containerbuddy

[mysql:5.6][mysql] wrapped for use with [Containerbuddy][containerbuddy].

## Usage

* `docker pull j0hnsmith/containerbuddy-mysql:latest`
* run [Consul][consul] somewhere
* set `ENV_NAME` and `CONSUL_HOST` env vars
* run `docker-compose up -d`
* visit the Consul http interface (default port 8500) and you'll see a service `mysql_{ENV_NAME}`

See [docker-compose.yml][compose file].

[mysql]: https://hub.docker.com/_/mysql/
[containerbuddy]: https://github.com/joyent/containerbuddy
[compose file]: docker-compose.yml
[consul]: https://www.consul.io/
