# PostgreSQL with Containerbuddy

[postgres:9.4.4][postgres] wrapped for use with [Containerbuddy][containerbuddy].

## Usage

* `docker pull j0hnsmith/containerbuddy-postgres:latest`
* run [Consul][consul] somewhere
* set `ENV_NAME` and `CONSUL_HOST` env vars
* run `docker-compose up -d`
* visit the Consul http interface (default port 8500) and you'll see a service `postgres_{ENV_NAME}`

See [docker-compose.yml][compose file].

[postgres]: https://hub.docker.com/_/postgres/
[containerbuddy]: https://github.com/joyent/containerbuddy
[compose file]: docker-compose.yml
[consul]: https://www.consul.io/
