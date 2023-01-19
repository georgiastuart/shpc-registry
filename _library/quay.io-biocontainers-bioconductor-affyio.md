---
layout: container
name:  "quay.io/biocontainers/bioconductor-affyio"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-affyio/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-affyio/container.yaml"
updated_at: "2023-01-19 03:22:04.460446"
latest: "1.68.0--r42hc0cfd56_0"
container_url: "https://biocontainers.pro/tools/bioconductor-affyio"

versions:
 - "1.64.0--r41hc0cfd56_2"
 - "1.68.0--r42hc0cfd56_0"
description: "shpc-registry automated BioContainers addition for bioconductor-affyio"
config: {"url": "https://biocontainers.pro/tools/bioconductor-affyio", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-affyio", "latest": {"1.68.0--r42hc0cfd56_0": "sha256:4fc4b4083c4c7e8146676cbcf60f0173b5d36169334e0f9f5596f53a97a836c1"}, "tags": {"1.64.0--r41hc0cfd56_2": "sha256:07e979c261f9a7e21f73aa7b06bc50fd78e60be422df35c880a650bac85087d7", "1.68.0--r42hc0cfd56_0": "sha256:4fc4b4083c4c7e8146676cbcf60f0173b5d36169334e0f9f5596f53a97a836c1"}, "docker": "quay.io/biocontainers/bioconductor-affyio"}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-affyio.
shpc-registry automated BioContainers addition for bioconductor-affyio
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-affyio
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-affyio:1.68.0--r42hc0cfd56_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-affyio/1.68.0--r42hc0cfd56_0
$ module help quay.io/biocontainers/bioconductor-affyio/1.68.0--r42hc0cfd56_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-affyio-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-affyio-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-affyio-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-affyio-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-affyio-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-affyio-inspect-deffile:

```bash
$ singularity inspect -d <container>
```



#### bioconductor-affyio

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