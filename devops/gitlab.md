# Gitlab

## Setup Runner

Install `gitlab-runner` https://docs.gitlab.com/runner/install/linux-repository.html

Install `docker`
```
curl -fsSL get.docker.com -o get-docker.sh
sh get-docker.sh
```

Register runner

- https://docs.gitlab.com/runner/register/
- https://docs.gitlab.com/ee/ci/docker/using_docker_build.html
- https://docs.gitlab.com/runner/commands

Register dind runner

```
sudo gitlab-runner register -n \
  --url https://gitlab.com/ \
  --registration-token TOKEN \
  --executor docker \
  --docker-image "docker:stable" \
  --docker-privileged \
  --tag-list dind \
  --name gitlab-runner-1
```
