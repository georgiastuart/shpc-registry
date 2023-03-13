---
layout: container
name:  "quay.io/biocontainers/ninja-nj"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/ninja-nj/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/ninja-nj/container.yaml"
updated_at: "2023-03-13 03:00:15.601248"
latest: "0.97--h9f5acd7_0"
container_url: "https://biocontainers.pro/tools/ninja-nj"
aliases:
 - "Ninja"
versions:
 - "0.97--h9f5acd7_0"
description: "singularity registry hpc automated addition for ninja-nj"
config: {"url": "https://biocontainers.pro/tools/ninja-nj", "maintainer": "@vsoch", "description": "singularity registry hpc automated addition for ninja-nj", "latest": {"0.97--h9f5acd7_0": "sha256:216fc2e2ba8905fc249e6dbd42c55dae95c05f2af38575d6de2090984196ee58"}, "tags": {"0.97--h9f5acd7_0": "sha256:216fc2e2ba8905fc249e6dbd42c55dae95c05f2af38575d6de2090984196ee58"}, "docker": "quay.io/biocontainers/ninja-nj", "aliases": {"Ninja": "/usr/local/bin/Ninja"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/ninja-nj.
singularity registry hpc automated addition for ninja-nj
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/ninja-nj
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/ninja-nj:0.97--h9f5acd7_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/ninja-nj/0.97--h9f5acd7_0
$ module help quay.io/biocontainers/ninja-nj/0.97--h9f5acd7_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### ninja-nj-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### ninja-nj-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### ninja-nj-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### ninja-nj-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### ninja-nj-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### ninja-nj-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### Ninja

```bash
$ singularity exec <container> /usr/local/bin/Ninja
$ podman run --it --rm --entrypoint /usr/local/bin/Ninja   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/Ninja   -v ${PWD} -w ${PWD} <container> -c " $@"
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