# Static page docker setup

**This comes from the static page template repository and should be updated when used in a project**

## Local setup

If one is not using itk-devs wrapper script. One simple needs the following steps to run it without.

```shell
docker network create frontend
docker compose up -d
```

To access the application, use the command below which will return host and port number.

```shell
docker compose port nginx 8080
```

## Nginx configuration

The default configuration for the "vhost" is located in the `.docker/templates/default.conf.template` file. Edit this
file to update the nginx setup.
