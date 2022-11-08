---
layout: container
name:  "quay.io/biocontainers/bioconductor-ewce"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-ewce/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-ewce/container.yaml"
updated_at: "2022-11-08 00:19:59.265695"
latest: "1.2.0--r41hdfd78af_0"
container_url: "https://biocontainers.pro/tools/bioconductor-ewce"
aliases:
 - ".bioconductor-ewcedata-post-link.sh"
 - ".bioconductor-ewcedata-pre-unlink.sh"
versions:
 - "1.2.0--r41hdfd78af_0"
description: "shpc-registry automated BioContainers addition for bioconductor-ewce"
config: {"url": "https://biocontainers.pro/tools/bioconductor-ewce", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-ewce", "latest": {"1.2.0--r41hdfd78af_0": "sha256:745deb9a0cd62484210da4357840222560dc1ed22574e5c80ac79fa21065ec7a"}, "tags": {"1.2.0--r41hdfd78af_0": "sha256:745deb9a0cd62484210da4357840222560dc1ed22574e5c80ac79fa21065ec7a"}, "docker": "quay.io/biocontainers/bioconductor-ewce", "aliases": {".bioconductor-ewcedata-post-link.sh": "/usr/local/bin/.bioconductor-ewcedata-post-link.sh", ".bioconductor-ewcedata-pre-unlink.sh": "/usr/local/bin/.bioconductor-ewcedata-pre-unlink.sh"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-ewce.
shpc-registry automated BioContainers addition for bioconductor-ewce
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-ewce
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-ewce:1.2.0--r41hdfd78af_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-ewce/1.2.0--r41hdfd78af_0
$ module help quay.io/biocontainers/bioconductor-ewce/1.2.0--r41hdfd78af_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-ewce-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-ewce-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-ewce-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-ewce-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-ewce-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-ewce-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### .bioconductor-ewcedata-post-link.sh

```bash
$ singularity exec <container> /usr/local/bin/.bioconductor-ewcedata-post-link.sh
$ podman run --it --rm --entrypoint /usr/local/bin/.bioconductor-ewcedata-post-link.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/.bioconductor-ewcedata-post-link.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### .bioconductor-ewcedata-pre-unlink.sh

```bash
$ singularity exec <container> /usr/local/bin/.bioconductor-ewcedata-pre-unlink.sh
$ podman run --it --rm --entrypoint /usr/local/bin/.bioconductor-ewcedata-pre-unlink.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/.bioconductor-ewcedata-pre-unlink.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
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