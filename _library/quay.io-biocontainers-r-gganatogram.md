---
layout: container
name:  "quay.io/biocontainers/r-gganatogram"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/r-gganatogram/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/r-gganatogram/container.yaml"
updated_at: "2023-02-19 03:19:34.489968"
latest: "0.0.1--r42hdfd78af_1"
container_url: "https://biocontainers.pro/tools/r-gganatogram"

versions:
 - "0.0.1--r41hdfd78af_0"
 - "0.0.1--r42hdfd78af_1"
description: "shpc-registry automated BioContainers addition for r-gganatogram"
config: {"url": "https://biocontainers.pro/tools/r-gganatogram", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for r-gganatogram", "latest": {"0.0.1--r42hdfd78af_1": "sha256:c8f55d1b28b626ddc69318ebc183265a4dee149e4f4eeba0af552293004371e7"}, "tags": {"0.0.1--r41hdfd78af_0": "sha256:1ba3f62bc5c3bc1e0aeb8b24951efa4314a5126c5bb094bb88b17ff0871f491e", "0.0.1--r42hdfd78af_1": "sha256:c8f55d1b28b626ddc69318ebc183265a4dee149e4f4eeba0af552293004371e7"}, "docker": "quay.io/biocontainers/r-gganatogram"}
---

This module is a singularity container wrapper for quay.io/biocontainers/r-gganatogram.
shpc-registry automated BioContainers addition for r-gganatogram
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/r-gganatogram
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/r-gganatogram:0.0.1--r42hdfd78af_1
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/r-gganatogram/0.0.1--r42hdfd78af_1
$ module help quay.io/biocontainers/r-gganatogram/0.0.1--r42hdfd78af_1
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### r-gganatogram-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### r-gganatogram-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### r-gganatogram-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### r-gganatogram-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### r-gganatogram-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### r-gganatogram-inspect-deffile:

```bash
$ singularity inspect -d <container>
```



#### r-gganatogram

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