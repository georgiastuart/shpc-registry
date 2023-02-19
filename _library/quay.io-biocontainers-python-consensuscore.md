---
layout: container
name:  "quay.io/biocontainers/python-consensuscore"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/python-consensuscore/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/python-consensuscore/container.yaml"
updated_at: "2023-02-19 03:08:16.059258"
latest: "1.1.1--py27hef6f488_6"
container_url: "https://biocontainers.pro/tools/python-consensuscore"

versions:
 - "1.1.1--py27hef6f488_6"
description: "shpc-registry automated BioContainers addition for python-consensuscore"
config: {"url": "https://biocontainers.pro/tools/python-consensuscore", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for python-consensuscore", "latest": {"1.1.1--py27hef6f488_6": "sha256:3b0662865ab54ffe5a64bbf2892fee33e3c031680f3df755ee1e45afd4d3173c"}, "tags": {"1.1.1--py27hef6f488_6": "sha256:3b0662865ab54ffe5a64bbf2892fee33e3c031680f3df755ee1e45afd4d3173c"}, "docker": "quay.io/biocontainers/python-consensuscore"}
---

This module is a singularity container wrapper for quay.io/biocontainers/python-consensuscore.
shpc-registry automated BioContainers addition for python-consensuscore
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/python-consensuscore
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/python-consensuscore:1.1.1--py27hef6f488_6
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/python-consensuscore/1.1.1--py27hef6f488_6
$ module help quay.io/biocontainers/python-consensuscore/1.1.1--py27hef6f488_6
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### python-consensuscore-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### python-consensuscore-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### python-consensuscore-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### python-consensuscore-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### python-consensuscore-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### python-consensuscore-inspect-deffile:

```bash
$ singularity inspect -d <container>
```



#### python-consensuscore

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