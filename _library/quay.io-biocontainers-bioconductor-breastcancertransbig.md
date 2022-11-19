---
layout: container
name:  "quay.io/biocontainers/bioconductor-breastcancertransbig"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-breastcancertransbig/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-breastcancertransbig/container.yaml"
updated_at: "2022-11-19 02:35:30.179866"
latest: "1.35.0--r42hdfd78af_0"
container_url: "https://biocontainers.pro/tools/bioconductor-breastcancertransbig"
aliases:
 - ".bioconductor-breastcancertransbig-post-link.sh"
 - ".bioconductor-breastcancertransbig-pre-unlink.sh"
versions:
 - "1.32.0--r41hdfd78af_1"
 - "1.35.0--r42hdfd78af_0"
description: "shpc-registry automated BioContainers addition for bioconductor-breastcancertransbig"
config: {"url": "https://biocontainers.pro/tools/bioconductor-breastcancertransbig", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-breastcancertransbig", "latest": {"1.35.0--r42hdfd78af_0": "sha256:475d2b94f3bf37dd82ec4ba19432892646d7514d4c772b555755ca4c8f977f14"}, "tags": {"1.32.0--r41hdfd78af_1": "sha256:661d2cd2486bfb121424de9680f415770581fa8ed6d908d9912de43e802c847c", "1.35.0--r42hdfd78af_0": "sha256:475d2b94f3bf37dd82ec4ba19432892646d7514d4c772b555755ca4c8f977f14"}, "docker": "quay.io/biocontainers/bioconductor-breastcancertransbig", "aliases": {".bioconductor-breastcancertransbig-post-link.sh": "/usr/local/bin/.bioconductor-breastcancertransbig-post-link.sh", ".bioconductor-breastcancertransbig-pre-unlink.sh": "/usr/local/bin/.bioconductor-breastcancertransbig-pre-unlink.sh"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-breastcancertransbig.
shpc-registry automated BioContainers addition for bioconductor-breastcancertransbig
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-breastcancertransbig
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-breastcancertransbig:1.35.0--r42hdfd78af_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-breastcancertransbig/1.35.0--r42hdfd78af_0
$ module help quay.io/biocontainers/bioconductor-breastcancertransbig/1.35.0--r42hdfd78af_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-breastcancertransbig-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-breastcancertransbig-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-breastcancertransbig-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-breastcancertransbig-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-breastcancertransbig-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-breastcancertransbig-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### .bioconductor-breastcancertransbig-post-link.sh

```bash
$ singularity exec <container> /usr/local/bin/.bioconductor-breastcancertransbig-post-link.sh
$ podman run --it --rm --entrypoint /usr/local/bin/.bioconductor-breastcancertransbig-post-link.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/.bioconductor-breastcancertransbig-post-link.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### .bioconductor-breastcancertransbig-pre-unlink.sh

```bash
$ singularity exec <container> /usr/local/bin/.bioconductor-breastcancertransbig-pre-unlink.sh
$ podman run --it --rm --entrypoint /usr/local/bin/.bioconductor-breastcancertransbig-pre-unlink.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/.bioconductor-breastcancertransbig-pre-unlink.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
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