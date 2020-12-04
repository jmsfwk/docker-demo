# .docker directory

This directory contains files for building and configuring Docker
Compose services.

The direct sub-directories here are named matching the services defined
in the `docker-compose.yml` file.

For example, the `php` service builds it's Docker image using the
`Dockerfile` in `.docker/php`.

```yaml
services:
  # ...
  php:
    build:
      context: .docker/php
  # ...
```

What is contained in the service sub-directly will vary depending on the
type of service, and the ammount of configuration required.
