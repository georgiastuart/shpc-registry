---
layout: container
name:  "quay.io/biocontainers/bioconductor-rgoslin"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-rgoslin/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-rgoslin/container.yaml"
updated_at: "2023-03-08 03:46:51.194041"
latest: "1.2.0--r42hc247a5b_0"
container_url: "https://biocontainers.pro/tools/bioconductor-rgoslin"

versions:
 - "1.2.0--r42hc247a5b_0"
description: "singularity registry hpc automated addition for bioconductor-rgoslin"
config: {"url": "https://biocontainers.pro/tools/bioconductor-rgoslin", "maintainer": "@vsoch", "description": "singularity registry hpc automated addition for bioconductor-rgoslin", "latest": {"1.2.0--r42hc247a5b_0": "sha256:0418b22c0377eaa4b875012f42d5573565b67b0be4cbf6e8ec4c18dd57b3cccb"}, "tags": {"1.2.0--r42hc247a5b_0": "sha256:0418b22c0377eaa4b875012f42d5573565b67b0be4cbf6e8ec4c18dd57b3cccb"}, "docker": "quay.io/biocontainers/bioconductor-rgoslin"}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-rgoslin.
singularity registry hpc automated addition for bioconductor-rgoslin
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-rgoslin
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-rgoslin:1.2.0--r42hc247a5b_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-rgoslin/1.2.0--r42hc247a5b_0
$ module help quay.io/biocontainers/bioconductor-rgoslin/1.2.0--r42hc247a5b_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-rgoslin-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-rgoslin-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-rgoslin-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-rgoslin-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-rgoslin-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-rgoslin-inspect-deffile:

```bash
$ singularity inspect -d <container>
```



#### bioconductor-rgoslin

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