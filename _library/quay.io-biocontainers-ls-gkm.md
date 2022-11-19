---
layout: container
name:  "quay.io/biocontainers/ls-gkm"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/ls-gkm/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/ls-gkm/container.yaml"
updated_at: "2022-11-19 02:41:39.637193"
latest: "0.0.1--h2d50403_1"
container_url: "https://biocontainers.pro/tools/ls-gkm"
aliases:
 - "gkmpredict"
 - "gkmtrain"
versions:
 - "0.0.1--h2d50403_1"
description: "shpc-registry automated BioContainers addition for ls-gkm"
config: {"url": "https://biocontainers.pro/tools/ls-gkm", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for ls-gkm", "latest": {"0.0.1--h2d50403_1": "sha256:044a0a5f9de3c2ca0756f8a88b51474320d55c13b5d84695a629a235dcf7e6f7"}, "tags": {"0.0.1--h2d50403_1": "sha256:044a0a5f9de3c2ca0756f8a88b51474320d55c13b5d84695a629a235dcf7e6f7"}, "docker": "quay.io/biocontainers/ls-gkm", "aliases": {"gkmpredict": "/usr/local/bin/gkmpredict", "gkmtrain": "/usr/local/bin/gkmtrain"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/ls-gkm.
shpc-registry automated BioContainers addition for ls-gkm
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/ls-gkm
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/ls-gkm:0.0.1--h2d50403_1
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/ls-gkm/0.0.1--h2d50403_1
$ module help quay.io/biocontainers/ls-gkm/0.0.1--h2d50403_1
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### ls-gkm-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### ls-gkm-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### ls-gkm-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### ls-gkm-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### ls-gkm-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### ls-gkm-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### gkmpredict

```bash
$ singularity exec <container> /usr/local/bin/gkmpredict
$ podman run --it --rm --entrypoint /usr/local/bin/gkmpredict   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/gkmpredict   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### gkmtrain

```bash
$ singularity exec <container> /usr/local/bin/gkmtrain
$ podman run --it --rm --entrypoint /usr/local/bin/gkmtrain   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/gkmtrain   -v ${PWD} -w ${PWD} <container> -c " $@"
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