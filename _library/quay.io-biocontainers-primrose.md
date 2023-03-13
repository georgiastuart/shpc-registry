---
layout: container
name:  "quay.io/biocontainers/primrose"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/primrose/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/primrose/container.yaml"
updated_at: "2023-03-13 03:39:49.092504"
latest: "1.3.0--h9ee0642_0"
container_url: "https://biocontainers.pro/tools/primrose"
aliases:
 - "primrose"
versions:
 - "1.3.0--h9ee0642_0"
description: "singularity registry hpc automated addition for primrose"
config: {"url": "https://biocontainers.pro/tools/primrose", "maintainer": "@vsoch", "description": "singularity registry hpc automated addition for primrose", "latest": {"1.3.0--h9ee0642_0": "sha256:ea2d49caee235c569a315686b73d922f09c42132985fdebd880cbd99bec9a651"}, "tags": {"1.3.0--h9ee0642_0": "sha256:ea2d49caee235c569a315686b73d922f09c42132985fdebd880cbd99bec9a651"}, "docker": "quay.io/biocontainers/primrose", "aliases": {"primrose": "/usr/local/bin/primrose"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/primrose.
singularity registry hpc automated addition for primrose
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/primrose
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/primrose:1.3.0--h9ee0642_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/primrose/1.3.0--h9ee0642_0
$ module help quay.io/biocontainers/primrose/1.3.0--h9ee0642_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### primrose-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### primrose-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### primrose-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### primrose-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### primrose-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### primrose-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### primrose

```bash
$ singularity exec <container> /usr/local/bin/primrose
$ podman run --it --rm --entrypoint /usr/local/bin/primrose   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/primrose   -v ${PWD} -w ${PWD} <container> -c " $@"
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