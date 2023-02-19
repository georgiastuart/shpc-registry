---
layout: container
name:  "quay.io/biocontainers/fqtk"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/fqtk/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/fqtk/container.yaml"
updated_at: "2023-02-19 03:34:08.183571"
latest: "0.2.0--h9f5acd7_0"
container_url: "https://biocontainers.pro/tools/fqtk"
aliases:
 - "fqtk"
versions:
 - "0.2.0--h9f5acd7_0"
description: "singularity registry hpc automated addition for fqtk"
config: {"url": "https://biocontainers.pro/tools/fqtk", "maintainer": "@vsoch", "description": "singularity registry hpc automated addition for fqtk", "latest": {"0.2.0--h9f5acd7_0": "sha256:14bdfc6ceba1585638ccf09033dfe68882bd0bf75ee5f807596e9d6676f5cbcd"}, "tags": {"0.2.0--h9f5acd7_0": "sha256:14bdfc6ceba1585638ccf09033dfe68882bd0bf75ee5f807596e9d6676f5cbcd"}, "docker": "quay.io/biocontainers/fqtk", "aliases": {"fqtk": "/usr/local/bin/fqtk"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/fqtk.
singularity registry hpc automated addition for fqtk
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/fqtk
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/fqtk:0.2.0--h9f5acd7_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/fqtk/0.2.0--h9f5acd7_0
$ module help quay.io/biocontainers/fqtk/0.2.0--h9f5acd7_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### fqtk-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### fqtk-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### fqtk-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### fqtk-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### fqtk-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### fqtk-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### fqtk

```bash
$ singularity exec <container> /usr/local/bin/fqtk
$ podman run --it --rm --entrypoint /usr/local/bin/fqtk   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/fqtk   -v ${PWD} -w ${PWD} <container> -c " $@"
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