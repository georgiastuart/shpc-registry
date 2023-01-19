---
layout: container
name:  "quay.io/biocontainers/irfinder"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/irfinder/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/irfinder/container.yaml"
updated_at: "2023-01-19 03:32:38.327216"
latest: "1.3.1--hec16e2b_2"
container_url: "https://biocontainers.pro/tools/irfinder"
aliases:
 - "IRFinder"
 - "perl5.32.1"
 - "streamzip"
versions:
 - "1.3.1--hec16e2b_2"
description: "shpc-registry automated BioContainers addition for irfinder"
config: {"url": "https://biocontainers.pro/tools/irfinder", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for irfinder", "latest": {"1.3.1--hec16e2b_2": "sha256:75da0f3da1b5d823d5d6b882376dcebd07ac2cf81a7727c1d061e2563b9005bd"}, "tags": {"1.3.1--hec16e2b_2": "sha256:75da0f3da1b5d823d5d6b882376dcebd07ac2cf81a7727c1d061e2563b9005bd"}, "docker": "quay.io/biocontainers/irfinder", "aliases": {"IRFinder": "/usr/local/bin/IRFinder", "perl5.32.1": "/usr/local/bin/perl5.32.1", "streamzip": "/usr/local/bin/streamzip"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/irfinder.
shpc-registry automated BioContainers addition for irfinder
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/irfinder
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/irfinder:1.3.1--hec16e2b_2
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/irfinder/1.3.1--hec16e2b_2
$ module help quay.io/biocontainers/irfinder/1.3.1--hec16e2b_2
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### irfinder-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### irfinder-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### irfinder-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### irfinder-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### irfinder-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### irfinder-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### IRFinder

```bash
$ singularity exec <container> /usr/local/bin/IRFinder
$ podman run --it --rm --entrypoint /usr/local/bin/IRFinder   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/IRFinder   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### perl5.32.1

```bash
$ singularity exec <container> /usr/local/bin/perl5.32.1
$ podman run --it --rm --entrypoint /usr/local/bin/perl5.32.1   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/perl5.32.1   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### streamzip

```bash
$ singularity exec <container> /usr/local/bin/streamzip
$ podman run --it --rm --entrypoint /usr/local/bin/streamzip   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/streamzip   -v ${PWD} -w ${PWD} <container> -c " $@"
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