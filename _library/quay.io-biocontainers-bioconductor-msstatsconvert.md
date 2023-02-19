---
layout: container
name:  "quay.io/biocontainers/bioconductor-msstatsconvert"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-msstatsconvert/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-msstatsconvert/container.yaml"
updated_at: "2023-02-19 02:58:55.894754"
latest: "1.8.0--r42hdfd78af_0"
container_url: "https://biocontainers.pro/tools/bioconductor-msstatsconvert"

versions:
 - "1.4.0--r41hdfd78af_0"
 - "1.8.0--r42hdfd78af_0"
description: "shpc-registry automated BioContainers addition for bioconductor-msstatsconvert"
config: {"url": "https://biocontainers.pro/tools/bioconductor-msstatsconvert", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-msstatsconvert", "latest": {"1.8.0--r42hdfd78af_0": "sha256:f70c455a0aab7282df5f2b49596d51c074e6ea5b91c2d4f59540ee33d46a67ae"}, "tags": {"1.4.0--r41hdfd78af_0": "sha256:2b8bbaee3b068a22207fdd5b6438610f51f63107425a4e5bbb93692ee50a04b2", "1.8.0--r42hdfd78af_0": "sha256:f70c455a0aab7282df5f2b49596d51c074e6ea5b91c2d4f59540ee33d46a67ae"}, "docker": "quay.io/biocontainers/bioconductor-msstatsconvert"}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-msstatsconvert.
shpc-registry automated BioContainers addition for bioconductor-msstatsconvert
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-msstatsconvert
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-msstatsconvert:1.8.0--r42hdfd78af_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-msstatsconvert/1.8.0--r42hdfd78af_0
$ module help quay.io/biocontainers/bioconductor-msstatsconvert/1.8.0--r42hdfd78af_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-msstatsconvert-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-msstatsconvert-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-msstatsconvert-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-msstatsconvert-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-msstatsconvert-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-msstatsconvert-inspect-deffile:

```bash
$ singularity inspect -d <container>
```



#### bioconductor-msstatsconvert

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