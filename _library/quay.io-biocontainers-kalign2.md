---
layout: container
name:  "quay.io/biocontainers/kalign2"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/kalign2/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/kalign2/container.yaml"
updated_at: "2022-11-08 00:24:57.491377"
latest: "2.04--hec16e2b_3"
container_url: "https://biocontainers.pro/tools/kalign2"
aliases:
 - "kalign"
versions:
 - "2.04--hec16e2b_3"
description: "shpc-registry automated BioContainers addition for kalign2"
config: {"url": "https://biocontainers.pro/tools/kalign2", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for kalign2", "latest": {"2.04--hec16e2b_3": "sha256:eb4ba0de5372625a86daefae59690a7155135e25722521f4ea281f5b0af91731"}, "tags": {"2.04--hec16e2b_3": "sha256:eb4ba0de5372625a86daefae59690a7155135e25722521f4ea281f5b0af91731"}, "docker": "quay.io/biocontainers/kalign2", "aliases": {"kalign": "/usr/local/bin/kalign"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/kalign2.
shpc-registry automated BioContainers addition for kalign2
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/kalign2
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/kalign2:2.04--hec16e2b_3
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/kalign2/2.04--hec16e2b_3
$ module help quay.io/biocontainers/kalign2/2.04--hec16e2b_3
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### kalign2-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### kalign2-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### kalign2-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### kalign2-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### kalign2-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### kalign2-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### kalign

```bash
$ singularity exec <container> /usr/local/bin/kalign
$ podman run --it --rm --entrypoint /usr/local/bin/kalign   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/kalign   -v ${PWD} -w ${PWD} <container> -c " $@"
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