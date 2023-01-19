---
layout: container
name:  "quay.io/biocontainers/bioconductor-hybridmtest"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-hybridmtest/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-hybridmtest/container.yaml"
updated_at: "2023-01-19 03:28:28.329377"
latest: "1.42.0--r42hdfd78af_0"
container_url: "https://biocontainers.pro/tools/bioconductor-hybridmtest"

versions:
 - "1.38.0--r41hdfd78af_0"
 - "1.42.0--r42hdfd78af_0"
description: "shpc-registry automated BioContainers addition for bioconductor-hybridmtest"
config: {"url": "https://biocontainers.pro/tools/bioconductor-hybridmtest", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-hybridmtest", "latest": {"1.42.0--r42hdfd78af_0": "sha256:11e276d0467bb523f161f1d2c715c4b1a6162ac9ce06999db92f1c0a88d0491a"}, "tags": {"1.38.0--r41hdfd78af_0": "sha256:68566a64bbdd19cfc491fa76f2c1cedfee85d9f75380e0d0dd2477da20f98e69", "1.42.0--r42hdfd78af_0": "sha256:11e276d0467bb523f161f1d2c715c4b1a6162ac9ce06999db92f1c0a88d0491a"}, "docker": "quay.io/biocontainers/bioconductor-hybridmtest"}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-hybridmtest.
shpc-registry automated BioContainers addition for bioconductor-hybridmtest
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-hybridmtest
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-hybridmtest:1.42.0--r42hdfd78af_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-hybridmtest/1.42.0--r42hdfd78af_0
$ module help quay.io/biocontainers/bioconductor-hybridmtest/1.42.0--r42hdfd78af_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-hybridmtest-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-hybridmtest-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-hybridmtest-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-hybridmtest-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-hybridmtest-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-hybridmtest-inspect-deffile:

```bash
$ singularity inspect -d <container>
```



#### bioconductor-hybridmtest

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