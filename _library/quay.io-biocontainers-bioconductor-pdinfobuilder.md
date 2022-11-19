---
layout: container
name:  "quay.io/biocontainers/bioconductor-pdinfobuilder"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-pdinfobuilder/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-pdinfobuilder/container.yaml"
updated_at: "2022-11-19 02:29:54.495415"
latest: "1.58.0--r41hc0cfd56_2"
container_url: "https://biocontainers.pro/tools/bioconductor-pdinfobuilder"

versions:
 - "1.58.0--r41hc0cfd56_2"
description: "shpc-registry automated BioContainers addition for bioconductor-pdinfobuilder"
config: {"url": "https://biocontainers.pro/tools/bioconductor-pdinfobuilder", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-pdinfobuilder", "latest": {"1.58.0--r41hc0cfd56_2": "sha256:6d7a33b0cd8ef54cb8635234040fdb74297bf914f5b5e4946cb93b3f9db0080f"}, "tags": {"1.58.0--r41hc0cfd56_2": "sha256:6d7a33b0cd8ef54cb8635234040fdb74297bf914f5b5e4946cb93b3f9db0080f"}, "docker": "quay.io/biocontainers/bioconductor-pdinfobuilder"}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-pdinfobuilder.
shpc-registry automated BioContainers addition for bioconductor-pdinfobuilder
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-pdinfobuilder
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-pdinfobuilder:1.58.0--r41hc0cfd56_2
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-pdinfobuilder/1.58.0--r41hc0cfd56_2
$ module help quay.io/biocontainers/bioconductor-pdinfobuilder/1.58.0--r41hc0cfd56_2
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-pdinfobuilder-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-pdinfobuilder-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-pdinfobuilder-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-pdinfobuilder-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-pdinfobuilder-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-pdinfobuilder-inspect-deffile:

```bash
$ singularity inspect -d <container>
```



#### bioconductor-pdinfobuilder

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