---
layout: container
name:  "quay.io/biocontainers/bioconductor-golubesets"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-golubesets/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-golubesets/container.yaml"
updated_at: "2022-11-19 02:00:22.634053"
latest: "1.40.0--r42hdfd78af_0"
container_url: "https://biocontainers.pro/tools/bioconductor-golubesets"
aliases:
 - ".bioconductor-golubesets-post-link.sh"
 - ".bioconductor-golubesets-pre-unlink.sh"
versions:
 - "1.36.0--r41hdfd78af_1"
 - "1.40.0--r42hdfd78af_0"
description: "shpc-registry automated BioContainers addition for bioconductor-golubesets"
config: {"url": "https://biocontainers.pro/tools/bioconductor-golubesets", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-golubesets", "latest": {"1.40.0--r42hdfd78af_0": "sha256:b2212201e9de85c861644709894fbf26ad8ed385e7a8330aee8d9c3c10e97d7d"}, "tags": {"1.36.0--r41hdfd78af_1": "sha256:52f1d40300d436c9a97a41f0b0ab804f262d75053bdd663ee52c4613c81ab12e", "1.40.0--r42hdfd78af_0": "sha256:b2212201e9de85c861644709894fbf26ad8ed385e7a8330aee8d9c3c10e97d7d"}, "docker": "quay.io/biocontainers/bioconductor-golubesets", "aliases": {".bioconductor-golubesets-post-link.sh": "/usr/local/bin/.bioconductor-golubesets-post-link.sh", ".bioconductor-golubesets-pre-unlink.sh": "/usr/local/bin/.bioconductor-golubesets-pre-unlink.sh"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-golubesets.
shpc-registry automated BioContainers addition for bioconductor-golubesets
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-golubesets
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-golubesets:1.40.0--r42hdfd78af_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-golubesets/1.40.0--r42hdfd78af_0
$ module help quay.io/biocontainers/bioconductor-golubesets/1.40.0--r42hdfd78af_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-golubesets-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-golubesets-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-golubesets-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-golubesets-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-golubesets-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-golubesets-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### .bioconductor-golubesets-post-link.sh

```bash
$ singularity exec <container> /usr/local/bin/.bioconductor-golubesets-post-link.sh
$ podman run --it --rm --entrypoint /usr/local/bin/.bioconductor-golubesets-post-link.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/.bioconductor-golubesets-post-link.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### .bioconductor-golubesets-pre-unlink.sh

```bash
$ singularity exec <container> /usr/local/bin/.bioconductor-golubesets-pre-unlink.sh
$ podman run --it --rm --entrypoint /usr/local/bin/.bioconductor-golubesets-pre-unlink.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/.bioconductor-golubesets-pre-unlink.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
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