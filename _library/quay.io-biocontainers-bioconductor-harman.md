---
layout: container
name:  "quay.io/biocontainers/bioconductor-harman"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-harman/container.yaml"
config_url: "https://raw.githubusercontent.com//singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-harman/container.yaml"
updated_at: "2022-10-29 18:25:22.616198"
latest: "1.8.0--r351hfc679d8_0"
container_url: "https://biocontainers.pro/tools/bioconductor-harman"

versions:
 - "1.8.0--r351hfc679d8_0"
description: "shpc-registry automated BioContainers addition for bioconductor-harman"
config: {"url": "https://biocontainers.pro/tools/bioconductor-harman", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-harman", "latest": {"1.8.0--r351hfc679d8_0": "sha256:f991fcbfe53b063c3c8c6ed799e43aa5eb6483a15aea768d7c2c2a9e0bab394a"}, "tags": {"1.8.0--r351hfc679d8_0": "sha256:f991fcbfe53b063c3c8c6ed799e43aa5eb6483a15aea768d7c2c2a9e0bab394a"}, "docker": "quay.io/biocontainers/bioconductor-harman"}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-harman.
shpc-registry automated BioContainers addition for bioconductor-harman
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-harman
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-harman:1.8.0--r351hfc679d8_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-harman/1.8.0--r351hfc679d8_0
$ module help quay.io/biocontainers/bioconductor-harman/1.8.0--r351hfc679d8_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-harman-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-harman-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-harman-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-harman-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-harman-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-harman-inspect-deffile:

```bash
$ singularity inspect -d <container>
```



#### bioconductor-harman

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