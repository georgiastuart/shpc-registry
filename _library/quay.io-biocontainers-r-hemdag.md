---
layout: container
name:  "quay.io/biocontainers/r-hemdag"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/r-hemdag/container.yaml"
config_url: "https://raw.githubusercontent.com//singularityhub/shpc-registry/main/quay.io/biocontainers/r-hemdag/container.yaml"
updated_at: "2022-10-29 18:24:11.912055"
latest: "2.7.4--r41hecf12ef_3"
container_url: "https://biocontainers.pro/tools/r-hemdag"

versions:
 - "2.7.4--r41hecf12ef_3"
description: "shpc-registry automated BioContainers addition for r-hemdag"
config: {"url": "https://biocontainers.pro/tools/r-hemdag", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for r-hemdag", "latest": {"2.7.4--r41hecf12ef_3": "sha256:d82eb11a905e6c664a26c002bde658edbf428e53cf76c34e99fea8054ebd0708"}, "tags": {"2.7.4--r41hecf12ef_3": "sha256:d82eb11a905e6c664a26c002bde658edbf428e53cf76c34e99fea8054ebd0708"}, "docker": "quay.io/biocontainers/r-hemdag"}
---

This module is a singularity container wrapper for quay.io/biocontainers/r-hemdag.
shpc-registry automated BioContainers addition for r-hemdag
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/r-hemdag
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/r-hemdag:2.7.4--r41hecf12ef_3
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/r-hemdag/2.7.4--r41hecf12ef_3
$ module help quay.io/biocontainers/r-hemdag/2.7.4--r41hecf12ef_3
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### r-hemdag-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### r-hemdag-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### r-hemdag-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### r-hemdag-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### r-hemdag-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### r-hemdag-inspect-deffile:

```bash
$ singularity inspect -d <container>
```



#### r-hemdag

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