---
layout: container
name:  "quay.io/biocontainers/bambamc"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bambamc/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bambamc/container.yaml"
updated_at: "2023-01-19 03:15:17.075174"
latest: "0.0.50--h7132678_5"
container_url: "https://biocontainers.pro/tools/bambamc"

versions:
 - "0.0.50--h7132678_5"
description: "shpc-registry automated BioContainers addition for bambamc"
config: {"url": "https://biocontainers.pro/tools/bambamc", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bambamc", "latest": {"0.0.50--h7132678_5": "sha256:1747302f343455876f6a7850483e817a8bfbb598c25c2f68faad94a3ba71662e"}, "tags": {"0.0.50--h7132678_5": "sha256:1747302f343455876f6a7850483e817a8bfbb598c25c2f68faad94a3ba71662e"}, "docker": "quay.io/biocontainers/bambamc"}
---

This module is a singularity container wrapper for quay.io/biocontainers/bambamc.
shpc-registry automated BioContainers addition for bambamc
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bambamc
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bambamc:0.0.50--h7132678_5
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bambamc/0.0.50--h7132678_5
$ module help quay.io/biocontainers/bambamc/0.0.50--h7132678_5
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bambamc-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bambamc-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bambamc-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bambamc-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bambamc-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bambamc-inspect-deffile:

```bash
$ singularity inspect -d <container>
```



#### bambamc

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