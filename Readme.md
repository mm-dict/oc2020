# Readme

## Run with docker

```
$ export JEKYLL_VERSION=3.8
$ docker run --rm \
 --volume="$PWD:/srv/jekyll" \
 -it jekyll/builder:$JEKYLL_VERSION \
 jekyll serve
```

## Build as an Nginx docker image

Inside the docker directory sits a Dockerfile that you can use to build a deployable nginx image containing the output of the jekyll build command.

