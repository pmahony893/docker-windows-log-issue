# docker-windows-log-issue
Repository to reproduce an issue on Docker Desktop.

To reproduce, run `docker-compose up service2`. In another terminal, monitor the output of `docker-compose logs service1 | select -Last 1`; after about 40s, the output will freeze. Killing the `service2` container will cause the `service1` output to restart (with a gap).

Note that running `docker-compose up -d service2` does not reproduce the issue, nor does simply `docker-compose up`.
