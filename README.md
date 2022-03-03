[![Publish Docker Image](https://github.com/GentseStudentenraad/docker-example/actions/workflows/publish.yml/badge.svg)](https://github.com/GentseStudentenraad/docker-example/actions/workflows/publish.yml)

# Publish a Docker image

An example on how to publish a Docker image to Github.

### Publishing a package.

Github will automatically publish a new version of the image when a release is created. To automatically build and publish your project using this workflow, change the `IMAGE_NAME` variable in `publish.yml`.

### Using a published package.

Simply pull the image like any other using `docker pull` or a `docker-compose` file. Available tags are `latest`, `MAJOR.MINOR` and `MAJOR.MINOR.PATCH`.

```
docker pull ghcr.io/gentsestudentenraad/docker-example:latest
```

### Authentication.

To pull (and manually update) containers, you may need to be authenticated. Refer to [this](https://docs.github.com/en/packages/working-with-a-github-packages-registry/working-with-the-container-registry) manual for more info.
