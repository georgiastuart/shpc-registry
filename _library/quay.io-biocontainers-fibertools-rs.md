---
layout: container
name:  "quay.io/biocontainers/fibertools-rs"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/fibertools-rs/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/fibertools-rs/container.yaml"
updated_at: "2023-03-29 00:45:40.600411"
latest: "0.1.3--h71fd010_0"
container_url: "https://biocontainers.pro/tools/fibertools-rs"
aliases:
 - "ft"
versions:
 - "0.1.2--h71fd010_0"
 - "0.1.3--h71fd010_0"
description: "singularity registry hpc automated addition for fibertools-rs"
config: {"url": "https://biocontainers.pro/tools/fibertools-rs", "maintainer": "@vsoch", "description": "singularity registry hpc automated addition for fibertools-rs", "latest": {"0.1.3--h71fd010_0": "sha256:4af6107cde71afbdcbeffdb08db17e8dde249205cab0ceeec473bf93b70a5c6f"}, "tags": {"0.1.2--h71fd010_0": "sha256:a66b88ea70106270a0ab246e45aada09593ffc2c02832698cf044c0f83c2bc3b", "0.1.3--h71fd010_0": "sha256:4af6107cde71afbdcbeffdb08db17e8dde249205cab0ceeec473bf93b70a5c6f"}, "docker": "quay.io/biocontainers/fibertools-rs", "aliases": {"ft": "/usr/local/bin/ft"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/fibertools-rs.
singularity registry hpc automated addition for fibertools-rs
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/fibertools-rs
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/fibertools-rs:0.1.3--h71fd010_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/fibertools-rs/0.1.3--h71fd010_0
$ module help quay.io/biocontainers/fibertools-rs/0.1.3--h71fd010_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### fibertools-rs-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### fibertools-rs-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### fibertools-rs-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### fibertools-rs-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### fibertools-rs-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### fibertools-rs-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### ft

```bash
$ singularity exec <container> /usr/local/bin/ft
$ podman run --it --rm --entrypoint /usr/local/bin/ft   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/ft   -v ${PWD} -w ${PWD} <container> -c " $@"
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