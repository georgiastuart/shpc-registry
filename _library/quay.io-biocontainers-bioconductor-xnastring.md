---
layout: container
name:  "quay.io/biocontainers/bioconductor-xnastring"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-xnastring/container.yaml"
config_url: "https://raw.githubusercontent.com//singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-xnastring/container.yaml"
updated_at: "2022-10-29 18:12:17.802949"
latest: "1.2.2--r41hc247a5b_1"
container_url: "https://biocontainers.pro/tools/bioconductor-xnastring"
aliases:
 - "pandoc-server"
 - "pandoc"
versions:
 - "1.2.2--r41hc247a5b_1"
description: "shpc-registry automated BioContainers addition for bioconductor-xnastring"
config: {"url": "https://biocontainers.pro/tools/bioconductor-xnastring", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-xnastring", "latest": {"1.2.2--r41hc247a5b_1": "sha256:633ae0af9fa9d79491acf5640b9cc2fb0463c49c58acb99818b3f5a4f205f42e"}, "tags": {"1.2.2--r41hc247a5b_1": "sha256:633ae0af9fa9d79491acf5640b9cc2fb0463c49c58acb99818b3f5a4f205f42e"}, "docker": "quay.io/biocontainers/bioconductor-xnastring", "aliases": {"pandoc-server": "/usr/local/bin/pandoc-server", "pandoc": "/usr/local/bin/pandoc"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-xnastring.
shpc-registry automated BioContainers addition for bioconductor-xnastring
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-xnastring
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-xnastring:1.2.2--r41hc247a5b_1
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-xnastring/1.2.2--r41hc247a5b_1
$ module help quay.io/biocontainers/bioconductor-xnastring/1.2.2--r41hc247a5b_1
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-xnastring-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-xnastring-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-xnastring-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-xnastring-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-xnastring-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-xnastring-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### pandoc-server

```bash
$ singularity exec <container> /usr/local/bin/pandoc-server
$ podman run --it --rm --entrypoint /usr/local/bin/pandoc-server   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/pandoc-server   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### pandoc

```bash
$ singularity exec <container> /usr/local/bin/pandoc
$ podman run --it --rm --entrypoint /usr/local/bin/pandoc   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/pandoc   -v ${PWD} -w ${PWD} <container> -c " $@"
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