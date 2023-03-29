---
layout: container
name:  "quay.io/biocontainers/strandphaser"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/strandphaser/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/strandphaser/container.yaml"
updated_at: "2023-03-29 00:39:25.279837"
latest: "1.0.0--r42hdfd78af_1"
container_url: "https://biocontainers.pro/tools/strandphaser"

versions:
 - "1.0.0--r41hdfd78af_0"
 - "1.0.0--r42hdfd78af_1"
description: "singularity registry hpc automated addition for strandphaser"
config: {"url": "https://biocontainers.pro/tools/strandphaser", "maintainer": "@vsoch", "description": "singularity registry hpc automated addition for strandphaser", "latest": {"1.0.0--r42hdfd78af_1": "sha256:eb180559c14d3019fcf53f60997a5203379463e267b73dcb70c09f4b764ae571"}, "tags": {"1.0.0--r41hdfd78af_0": "sha256:494a35b6be5692ae789f7cd36c1752e246a2eb77d2472d3cd5427de62b1b8398", "1.0.0--r42hdfd78af_1": "sha256:eb180559c14d3019fcf53f60997a5203379463e267b73dcb70c09f4b764ae571"}, "docker": "quay.io/biocontainers/strandphaser"}
---

This module is a singularity container wrapper for quay.io/biocontainers/strandphaser.
singularity registry hpc automated addition for strandphaser
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/strandphaser
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/strandphaser:1.0.0--r42hdfd78af_1
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/strandphaser/1.0.0--r42hdfd78af_1
$ module help quay.io/biocontainers/strandphaser/1.0.0--r42hdfd78af_1
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### strandphaser-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### strandphaser-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### strandphaser-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### strandphaser-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### strandphaser-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### strandphaser-inspect-deffile:

```bash
$ singularity inspect -d <container>
```



#### strandphaser

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