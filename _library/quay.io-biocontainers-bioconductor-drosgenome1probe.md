---
layout: container
name:  "quay.io/biocontainers/bioconductor-drosgenome1probe"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-drosgenome1probe/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-drosgenome1probe/container.yaml"
updated_at: "2022-11-08 00:05:19.527264"
latest: "2.18.0--r41hdfd78af_9"
container_url: "https://biocontainers.pro/tools/bioconductor-drosgenome1probe"
aliases:
 - ".bioconductor-drosgenome1probe-post-link.sh"
 - ".bioconductor-drosgenome1probe-pre-unlink.sh"
versions:
 - "2.18.0--r41hdfd78af_9"
description: "shpc-registry automated BioContainers addition for bioconductor-drosgenome1probe"
config: {"url": "https://biocontainers.pro/tools/bioconductor-drosgenome1probe", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-drosgenome1probe", "latest": {"2.18.0--r41hdfd78af_9": "sha256:bd1b6315588f6b5f3e1f35650da5c24e394e836de69437a6ded2b52c02832c5e"}, "tags": {"2.18.0--r41hdfd78af_9": "sha256:bd1b6315588f6b5f3e1f35650da5c24e394e836de69437a6ded2b52c02832c5e"}, "docker": "quay.io/biocontainers/bioconductor-drosgenome1probe", "aliases": {".bioconductor-drosgenome1probe-post-link.sh": "/usr/local/bin/.bioconductor-drosgenome1probe-post-link.sh", ".bioconductor-drosgenome1probe-pre-unlink.sh": "/usr/local/bin/.bioconductor-drosgenome1probe-pre-unlink.sh"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-drosgenome1probe.
shpc-registry automated BioContainers addition for bioconductor-drosgenome1probe
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-drosgenome1probe
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-drosgenome1probe:2.18.0--r41hdfd78af_9
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-drosgenome1probe/2.18.0--r41hdfd78af_9
$ module help quay.io/biocontainers/bioconductor-drosgenome1probe/2.18.0--r41hdfd78af_9
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-drosgenome1probe-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-drosgenome1probe-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-drosgenome1probe-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-drosgenome1probe-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-drosgenome1probe-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-drosgenome1probe-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### .bioconductor-drosgenome1probe-post-link.sh

```bash
$ singularity exec <container> /usr/local/bin/.bioconductor-drosgenome1probe-post-link.sh
$ podman run --it --rm --entrypoint /usr/local/bin/.bioconductor-drosgenome1probe-post-link.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/.bioconductor-drosgenome1probe-post-link.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### .bioconductor-drosgenome1probe-pre-unlink.sh

```bash
$ singularity exec <container> /usr/local/bin/.bioconductor-drosgenome1probe-pre-unlink.sh
$ podman run --it --rm --entrypoint /usr/local/bin/.bioconductor-drosgenome1probe-pre-unlink.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/.bioconductor-drosgenome1probe-pre-unlink.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
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