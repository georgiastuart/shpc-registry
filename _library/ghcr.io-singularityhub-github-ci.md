---
layout: container
name:  "ghcr.io/singularityhub/github-ci"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/ghcr.io/singularityhub/github-ci/container.yaml"
config_url: "https://raw.githubusercontent.com//singularityhub/shpc-registry/main/ghcr.io/singularityhub/github-ci/container.yaml"
updated_at: "2022-10-01 03:20:00.835407"
latest: "latest"
container_url: "https://github.com/singularityhub/github-ci/pkgs/container/github-ci"

versions:
 - "latest"
description: "An example SIF on GitHub packages to pull with oras"
config: {"oras": "ghcr.io/singularityhub/github-ci", "url": "https://github.com/singularityhub/github-ci/pkgs/container/github-ci", "maintainer": "@vsoch", "description": "An example SIF on GitHub packages to pull with oras", "latest": {"latest": "sha256:5d6742ff0b10c1196202765dafb43275259bcbdbd3868c19ba1d19476c088867"}, "tags": {"latest": "sha256:5d6742ff0b10c1196202765dafb43275259bcbdbd3868c19ba1d19476c088867"}}
---

This module is a singularity container wrapper for ghcr.io/singularityhub/github-ci.
An example SIF on GitHub packages to pull with oras
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install ghcr.io/singularityhub/github-ci
```

Or a specific version:

```bash
$ shpc install ghcr.io/singularityhub/github-ci:latest
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load ghcr.io/singularityhub/github-ci/latest
$ module help ghcr.io/singularityhub/github-ci/latest
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### github-ci-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### github-ci-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### github-ci-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### github-ci-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### github-ci-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### github-ci-inspect-deffile:

```bash
$ singularity inspect -d <container>
```



#### github-ci

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```


In the above, the `<container>` directive will reference an actual container provided
by the module, for the version you have chosen to load. An environment file in the
module folder will also be bound. Note that although a container
might provide custom commands, every container exposes unique exec, shell, run, and
inspect aliases. For anycommands above, you can export:

 - SINGULARITY_OPTS: to define custom options for singularity (e.g., --debug)
 - SINGULARITY_COMMAND_OPTS: to define custom options for the command (e.g., -b)
 - PODMAN_OPTS: to define custom options for podman or docker
 - PODMAN_COMMAND_OPTS: to define custom options for the command

<br>
  
### Install

You can install shpc locally (for yourself or your user base) as follows:

```bash
$ git clone https://github.com/singularityhub/singularity-hpc
$ cd singularity-hpc
$ pip install -e .
```

Have any questions, or want to request a new module or version? [ask for help!](https://github.com/singularityhub/singularity-hpc/issues)