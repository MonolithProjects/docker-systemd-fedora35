# Fedora 35 Ansible Test Image

[![GitHub Actions](https://github.com/MonolithProjects/docker-systemd-fedora35/workflows/Dockerfile%20test/badge.svg?branch=master)](https://github.com/MonolithProjects/docker-systemd-fedora35/actions)
[![DockerHub-pulls](https://img.shields.io/docker/pulls/monolithprojects/systemd-fedora35)](https://hub.docker.com/repository/docker/monolithprojects/systemd-fedora35)
[![DockerHub-pulls](https://img.shields.io/docker/pulls/monolithprojects/systemd-fedora35)](https://hub.docker.com/repository/docker/monolithprojects/systemd-fedora35)
[![DockerHub](https://img.shields.io/docker/image-size/monolithprojects/systemd-fedora35?sort=date)](https://hub.docker.com/repository/docker/monolithprojects/systemd-fedora35)

Docker image with Fedora 35 and enabled systemd. Image is updated with the latest software updates on the 1st day in the month. Image contains also `ansible` user (UID/GID 1000) with NOPASSWD:ALL sudo rights.  

**Note:** This docker image is ment to be used for Molecule Ansible tests and development purpose. I do not recomend to use it in production.

## Tags

- `latest`  
- `<monthly build timestamp>` for the list of the tags see the [Docker Hub](https://hub.docker.com/repository/docker/monolithprojects/systemd-fedora35/tags?page=1)

## How-to

  1. Pull image with command `docker pull monolithprojects/systemd-fedora35:latest`  
  2. Run the container from the image: `docker run --detach --privileged --volume=/sys/fs/cgroup:/sys/fs/cgroup:ro monolithprojects/systemd-fedora35:latest`  

## License

MIT
