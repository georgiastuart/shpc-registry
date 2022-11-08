---
layout: container
name:  "quay.io/biocontainers/minnow"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/minnow/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/minnow/container.yaml"
updated_at: "2022-11-08 00:04:20.879201"
latest: "beta_1.3--h7f8bfb2_2"
container_url: "https://biocontainers.pro/tools/minnow"
aliases:
 - "fixfasta"
 - "minnow"
versions:
 - "beta_1.3--h7f8bfb2_2"
description: "shpc-registry automated BioContainers addition for minnow"
config: {"url": "https://biocontainers.pro/tools/minnow", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for minnow", "latest": {"beta_1.3--h7f8bfb2_2": "sha256:35ccf4f29592aee63b5ef61429d75f7b9e4cac62660c16a38aaec4612ff51d5f"}, "tags": {"beta_1.3--h7f8bfb2_2": "sha256:35ccf4f29592aee63b5ef61429d75f7b9e4cac62660c16a38aaec4612ff51d5f"}, "docker": "quay.io/biocontainers/minnow", "aliases": {"fixfasta": "/usr/local/bin/fixfasta", "minnow": "/usr/local/bin/minnow"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/minnow.
shpc-registry automated BioContainers addition for minnow
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/minnow
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/minnow:beta_1.3--h7f8bfb2_2
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/minnow/beta_1.3--h7f8bfb2_2
$ module help quay.io/biocontainers/minnow/beta_1.3--h7f8bfb2_2
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### minnow-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### minnow-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### minnow-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### minnow-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### minnow-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### minnow-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### fixfasta

```bash
$ singularity exec <container> /usr/local/bin/fixfasta
$ podman run --it --rm --entrypoint /usr/local/bin/fixfasta   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/fixfasta   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### minnow

```bash
$ singularity exec <container> /usr/local/bin/minnow
$ podman run --it --rm --entrypoint /usr/local/bin/minnow   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/minnow   -v ${PWD} -w ${PWD} <container> -c " $@"
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