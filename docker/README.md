# Gitlab CI Runner for Docker

This Gitlab CI runner can be used to build docker images for any project.

To do so, it needs to access the host's docker instance and thus needs special privileges.

## Usage

    docker run -ti --rm -e CI_SERVER_URL=<URL for gitlab CI> -e REGISTRATION_TOKEN=<Gitlab CI runner token> -v /var/run/docker.sock:/var/run/docker.sock --privileged stilvoid/gitlab-ci-runner-docker
