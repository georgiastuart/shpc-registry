---
layout: container
name:  "quay.io/biocontainers/edlib"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/edlib/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/edlib/container.yaml"
updated_at: "2022-11-08 00:25:13.474561"
latest: "1.2.3--h2d50403_1"
container_url: "https://biocontainers.pro/tools/edlib"
aliases:
 - "edlib-aligner"
versions:
 - "1.2.3--h2d50403_1"
description: "shpc-registry automated BioContainers addition for edlib"
config: {"url": "https://biocontainers.pro/tools/edlib", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for edlib", "latest": {"1.2.3--h2d50403_1": "sha256:acf2aa7794085e1864f67424a4369bdfbfad0f544cc15a132f3ac1cdb9518208"}, "tags": {"1.2.3--h2d50403_1": "sha256:acf2aa7794085e1864f67424a4369bdfbfad0f544cc15a132f3ac1cdb9518208"}, "docker": "quay.io/biocontainers/edlib", "aliases": {"edlib-aligner": "/usr/local/bin/edlib-aligner"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/edlib.
shpc-registry automated BioContainers addition for edlib
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/edlib
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/edlib:1.2.3--h2d50403_1
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/edlib/1.2.3--h2d50403_1
$ module help quay.io/biocontainers/edlib/1.2.3--h2d50403_1
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### edlib-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### edlib-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### edlib-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### edlib-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### edlib-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### edlib-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### edlib-aligner

```bash
$ singularity exec <container> /usr/local/bin/edlib-aligner
$ podman run --it --rm --entrypoint /usr/local/bin/edlib-aligner   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/edlib-aligner   -v ${PWD} -w ${PWD} <container> -c " $@"
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