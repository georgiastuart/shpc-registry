---
layout: container
name:  "quay.io/biocontainers/r-r0"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/r-r0/container.yaml"
config_url: "https://raw.githubusercontent.com//singularityhub/shpc-registry/main/quay.io/biocontainers/r-r0/container.yaml"
updated_at: "2022-10-29 18:28:24.662988"
latest: "1.2_6--r41h3121a25_0"
container_url: "https://biocontainers.pro/tools/r-r0"

versions:
 - "1.2_6--r41h3121a25_0"
description: "shpc-registry automated BioContainers addition for r-r0"
config: {"url": "https://biocontainers.pro/tools/r-r0", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for r-r0", "latest": {"1.2_6--r41h3121a25_0": "sha256:11ee1f23da1384699320bfa421606c1b9017c3fbe2ca264900ae4abb8eb29e65"}, "tags": {"1.2_6--r41h3121a25_0": "sha256:11ee1f23da1384699320bfa421606c1b9017c3fbe2ca264900ae4abb8eb29e65"}, "docker": "quay.io/biocontainers/r-r0"}
---

This module is a singularity container wrapper for quay.io/biocontainers/r-r0.
shpc-registry automated BioContainers addition for r-r0
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/r-r0
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/r-r0:1.2_6--r41h3121a25_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/r-r0/1.2_6--r41h3121a25_0
$ module help quay.io/biocontainers/r-r0/1.2_6--r41h3121a25_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### r-r0-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### r-r0-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### r-r0-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### r-r0-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### r-r0-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### r-r0-inspect-deffile:

```bash
$ singularity inspect -d <container>
```



#### r-r0

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