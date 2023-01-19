---
layout: container
name:  "quay.io/biocontainers/bioconductor-rhdf5"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-rhdf5/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-rhdf5/container.yaml"
updated_at: "2023-01-19 03:06:14.108587"
latest: "2.42.0--r42hbe1951d_1"
container_url: "https://biocontainers.pro/tools/bioconductor-rhdf5"

versions:
 - "2.38.1--r41hbe1951d_0"
 - "2.42.0--r42hbe1951d_1"
description: "shpc-registry automated BioContainers addition for bioconductor-rhdf5"
config: {"url": "https://biocontainers.pro/tools/bioconductor-rhdf5", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-rhdf5", "latest": {"2.42.0--r42hbe1951d_1": "sha256:15616a2f0ced1287438c795d4c937c35581f1de9f8284617795eeacb34f3b097"}, "tags": {"2.38.1--r41hbe1951d_0": "sha256:b816b7e7580680f2b339ecd4b6ed11927ea778f04f83e43f973e5807751ff549", "2.42.0--r42hbe1951d_1": "sha256:15616a2f0ced1287438c795d4c937c35581f1de9f8284617795eeacb34f3b097"}, "docker": "quay.io/biocontainers/bioconductor-rhdf5"}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-rhdf5.
shpc-registry automated BioContainers addition for bioconductor-rhdf5
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-rhdf5
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-rhdf5:2.42.0--r42hbe1951d_1
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-rhdf5/2.42.0--r42hbe1951d_1
$ module help quay.io/biocontainers/bioconductor-rhdf5/2.42.0--r42hbe1951d_1
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-rhdf5-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-rhdf5-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-rhdf5-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-rhdf5-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-rhdf5-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-rhdf5-inspect-deffile:

```bash
$ singularity inspect -d <container>
```



#### bioconductor-rhdf5

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