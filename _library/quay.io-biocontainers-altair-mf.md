---
layout: container
name:  "quay.io/biocontainers/altair-mf"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/altair-mf/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/altair-mf/container.yaml"
updated_at: "2023-03-08 03:20:34.761443"
latest: "1.0.1--hd03093a_0"
container_url: "https://biocontainers.pro/tools/altair-mf"
aliases:
 - "AltaiR"
versions:
 - "1.0.1--hd03093a_0"
description: "singularity registry hpc automated addition for altair-mf"
config: {"url": "https://biocontainers.pro/tools/altair-mf", "maintainer": "@vsoch", "description": "singularity registry hpc automated addition for altair-mf", "latest": {"1.0.1--hd03093a_0": "sha256:ab0a68275b589ed0ddfea848e8940c3e3441f1f81228b7ec4047012fb25c008f"}, "tags": {"1.0.1--hd03093a_0": "sha256:ab0a68275b589ed0ddfea848e8940c3e3441f1f81228b7ec4047012fb25c008f"}, "docker": "quay.io/biocontainers/altair-mf", "aliases": {"AltaiR": "/usr/local/bin/AltaiR"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/altair-mf.
singularity registry hpc automated addition for altair-mf
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/altair-mf
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/altair-mf:1.0.1--hd03093a_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/altair-mf/1.0.1--hd03093a_0
$ module help quay.io/biocontainers/altair-mf/1.0.1--hd03093a_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### altair-mf-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### altair-mf-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### altair-mf-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### altair-mf-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### altair-mf-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### altair-mf-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### AltaiR

```bash
$ singularity exec <container> /usr/local/bin/AltaiR
$ podman run --it --rm --entrypoint /usr/local/bin/AltaiR   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/AltaiR   -v ${PWD} -w ${PWD} <container> -c " $@"
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