---
layout: container
name:  "quay.io/biocontainers/bioconductor-qtlizer"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-qtlizer/container.yaml"
config_url: "https://raw.githubusercontent.com//singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-qtlizer/container.yaml"
updated_at: "2022-10-29 17:58:40.144399"
latest: "1.8.0--r41hdfd78af_0"
container_url: "https://biocontainers.pro/tools/bioconductor-qtlizer"

versions:
 - "1.8.0--r41hdfd78af_0"
description: "shpc-registry automated BioContainers addition for bioconductor-qtlizer"
config: {"url": "https://biocontainers.pro/tools/bioconductor-qtlizer", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-qtlizer", "latest": {"1.8.0--r41hdfd78af_0": "sha256:a893b9d21599406216f06313fd1a3a33c4c7ad1d493c39f03632cbb57d031b14"}, "tags": {"1.8.0--r41hdfd78af_0": "sha256:a893b9d21599406216f06313fd1a3a33c4c7ad1d493c39f03632cbb57d031b14"}, "docker": "quay.io/biocontainers/bioconductor-qtlizer"}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-qtlizer.
shpc-registry automated BioContainers addition for bioconductor-qtlizer
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-qtlizer
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-qtlizer:1.8.0--r41hdfd78af_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-qtlizer/1.8.0--r41hdfd78af_0
$ module help quay.io/biocontainers/bioconductor-qtlizer/1.8.0--r41hdfd78af_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-qtlizer-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-qtlizer-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-qtlizer-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-qtlizer-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-qtlizer-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-qtlizer-inspect-deffile:

```bash
$ singularity inspect -d <container>
```



#### bioconductor-qtlizer

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