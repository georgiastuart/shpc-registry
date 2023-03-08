---
layout: container
name:  "quay.io/biocontainers/strobealign"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/strobealign/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/strobealign/container.yaml"
updated_at: "2023-03-08 03:17:21.933932"
latest: "0.8.0--h5b5514e_0"
container_url: "https://biocontainers.pro/tools/strobealign"
aliases:
 - "strobealign"
versions:
 - "0.8.0--h5b5514e_0"
description: "singularity registry hpc automated addition for strobealign"
config: {"url": "https://biocontainers.pro/tools/strobealign", "maintainer": "@vsoch", "description": "singularity registry hpc automated addition for strobealign", "latest": {"0.8.0--h5b5514e_0": "sha256:ed5a49652c2d82798289955d567586f7accd48b2f0119a88eefef28d34cf63c5"}, "tags": {"0.8.0--h5b5514e_0": "sha256:ed5a49652c2d82798289955d567586f7accd48b2f0119a88eefef28d34cf63c5"}, "docker": "quay.io/biocontainers/strobealign", "aliases": {"strobealign": "/usr/local/bin/strobealign"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/strobealign.
singularity registry hpc automated addition for strobealign
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/strobealign
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/strobealign:0.8.0--h5b5514e_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/strobealign/0.8.0--h5b5514e_0
$ module help quay.io/biocontainers/strobealign/0.8.0--h5b5514e_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### strobealign-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### strobealign-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### strobealign-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### strobealign-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### strobealign-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### strobealign-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### strobealign

```bash
$ singularity exec <container> /usr/local/bin/strobealign
$ podman run --it --rm --entrypoint /usr/local/bin/strobealign   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/strobealign   -v ${PWD} -w ${PWD} <container> -c " $@"
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