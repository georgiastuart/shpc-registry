---
layout: container
name:  "quay.io/biocontainers/bioconductor-ampaffyexample"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-ampaffyexample/container.yaml"
config_url: "https://raw.githubusercontent.com//singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-ampaffyexample/container.yaml"
updated_at: "2022-10-29 18:23:57.293367"
latest: "1.34.0--r41hdfd78af_1"
container_url: "https://biocontainers.pro/tools/bioconductor-ampaffyexample"
aliases:
 - ".bioconductor-ampaffyexample-post-link.sh"
 - ".bioconductor-ampaffyexample-pre-unlink.sh"
versions:
 - "1.34.0--r41hdfd78af_1"
description: "shpc-registry automated BioContainers addition for bioconductor-ampaffyexample"
config: {"url": "https://biocontainers.pro/tools/bioconductor-ampaffyexample", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-ampaffyexample", "latest": {"1.34.0--r41hdfd78af_1": "sha256:96c253ff8daf0ffc130c90919c6468bd4dde82da9a55e94a35f90fcce86dfc4a"}, "tags": {"1.34.0--r41hdfd78af_1": "sha256:96c253ff8daf0ffc130c90919c6468bd4dde82da9a55e94a35f90fcce86dfc4a"}, "docker": "quay.io/biocontainers/bioconductor-ampaffyexample", "aliases": {".bioconductor-ampaffyexample-post-link.sh": "/usr/local/bin/.bioconductor-ampaffyexample-post-link.sh", ".bioconductor-ampaffyexample-pre-unlink.sh": "/usr/local/bin/.bioconductor-ampaffyexample-pre-unlink.sh"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-ampaffyexample.
shpc-registry automated BioContainers addition for bioconductor-ampaffyexample
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-ampaffyexample
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-ampaffyexample:1.34.0--r41hdfd78af_1
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-ampaffyexample/1.34.0--r41hdfd78af_1
$ module help quay.io/biocontainers/bioconductor-ampaffyexample/1.34.0--r41hdfd78af_1
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-ampaffyexample-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-ampaffyexample-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-ampaffyexample-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-ampaffyexample-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-ampaffyexample-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-ampaffyexample-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### .bioconductor-ampaffyexample-post-link.sh

```bash
$ singularity exec <container> /usr/local/bin/.bioconductor-ampaffyexample-post-link.sh
$ podman run --it --rm --entrypoint /usr/local/bin/.bioconductor-ampaffyexample-post-link.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/.bioconductor-ampaffyexample-post-link.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### .bioconductor-ampaffyexample-pre-unlink.sh

```bash
$ singularity exec <container> /usr/local/bin/.bioconductor-ampaffyexample-pre-unlink.sh
$ podman run --it --rm --entrypoint /usr/local/bin/.bioconductor-ampaffyexample-pre-unlink.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/.bioconductor-ampaffyexample-pre-unlink.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
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