---
layout: container
name:  "quay.io/biocontainers/bioconductor-diffbind"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-diffbind/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-diffbind/container.yaml"
updated_at: "2022-11-19 02:26:40.012230"
latest: "3.4.11--r41hc247a5b_1"
container_url: "https://biocontainers.pro/tools/bioconductor-diffbind"

versions:
 - "3.4.11--r41hc247a5b_1"
description: "shpc-registry automated BioContainers addition for bioconductor-diffbind"
config: {"url": "https://biocontainers.pro/tools/bioconductor-diffbind", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-diffbind", "latest": {"3.4.11--r41hc247a5b_1": "sha256:6c4dc11db8dbe34f4bd342b1f711548c25546414b82adfac52a2e7b7d498062b"}, "tags": {"3.4.11--r41hc247a5b_1": "sha256:6c4dc11db8dbe34f4bd342b1f711548c25546414b82adfac52a2e7b7d498062b"}, "docker": "quay.io/biocontainers/bioconductor-diffbind"}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-diffbind.
shpc-registry automated BioContainers addition for bioconductor-diffbind
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-diffbind
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-diffbind:3.4.11--r41hc247a5b_1
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-diffbind/3.4.11--r41hc247a5b_1
$ module help quay.io/biocontainers/bioconductor-diffbind/3.4.11--r41hc247a5b_1
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-diffbind-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-diffbind-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-diffbind-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-diffbind-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-diffbind-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-diffbind-inspect-deffile:

```bash
$ singularity inspect -d <container>
```



#### bioconductor-diffbind

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