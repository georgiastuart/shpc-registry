---
layout: container
name:  "quay.io/biocontainers/mrsfast"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/mrsfast/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/mrsfast/container.yaml"
updated_at: "2023-01-19 03:16:44.033924"
latest: "3.4.2--h7132678_2"
container_url: "https://biocontainers.pro/tools/mrsfast"
aliases:
 - "mrsfast"
versions:
 - "3.4.2--h7132678_2"
description: "shpc-registry automated BioContainers addition for mrsfast"
config: {"url": "https://biocontainers.pro/tools/mrsfast", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for mrsfast", "latest": {"3.4.2--h7132678_2": "sha256:0eef21f24fffa5eed8e296953fdaab52feae5d1501e7f067a65bbc529d949020"}, "tags": {"3.4.2--h7132678_2": "sha256:0eef21f24fffa5eed8e296953fdaab52feae5d1501e7f067a65bbc529d949020"}, "docker": "quay.io/biocontainers/mrsfast", "aliases": {"mrsfast": "/usr/local/bin/mrsfast"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/mrsfast.
shpc-registry automated BioContainers addition for mrsfast
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/mrsfast
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/mrsfast:3.4.2--h7132678_2
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/mrsfast/3.4.2--h7132678_2
$ module help quay.io/biocontainers/mrsfast/3.4.2--h7132678_2
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### mrsfast-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### mrsfast-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### mrsfast-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### mrsfast-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### mrsfast-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### mrsfast-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### mrsfast

```bash
$ singularity exec <container> /usr/local/bin/mrsfast
$ podman run --it --rm --entrypoint /usr/local/bin/mrsfast   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/mrsfast   -v ${PWD} -w ${PWD} <container> -c " $@"
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