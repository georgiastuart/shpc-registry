---
layout: container
name:  "quay.io/biocontainers/bioconductor-reactomegsa.data"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-reactomegsa.data/container.yaml"
config_url: "https://raw.githubusercontent.com//singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-reactomegsa.data/container.yaml"
updated_at: "2022-10-29 17:38:46.818930"
latest: "1.8.0--r41hdfd78af_1"
container_url: "https://biocontainers.pro/tools/bioconductor-reactomegsa.data"
aliases:
 - ".bioconductor-reactomegsa.data-post-link.sh"
 - ".bioconductor-reactomegsa.data-pre-unlink.sh"
 - "geosop"
 - "geos-config"
 - "glpsol"
versions:
 - "1.8.0--r41hdfd78af_1"
description: "shpc-registry automated BioContainers addition for bioconductor-reactomegsa.data"
config: {"url": "https://biocontainers.pro/tools/bioconductor-reactomegsa.data", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-reactomegsa.data", "latest": {"1.8.0--r41hdfd78af_1": "sha256:3d47ef470ff9d95f59bcf03dfcb18b05dbd14b8909dbc61cb2036ff30a1dc28d"}, "tags": {"1.8.0--r41hdfd78af_1": "sha256:3d47ef470ff9d95f59bcf03dfcb18b05dbd14b8909dbc61cb2036ff30a1dc28d"}, "docker": "quay.io/biocontainers/bioconductor-reactomegsa.data", "aliases": {".bioconductor-reactomegsa.data-post-link.sh": "/usr/local/bin/.bioconductor-reactomegsa.data-post-link.sh", ".bioconductor-reactomegsa.data-pre-unlink.sh": "/usr/local/bin/.bioconductor-reactomegsa.data-pre-unlink.sh", "geosop": "/usr/local/bin/geosop", "geos-config": "/usr/local/bin/geos-config", "glpsol": "/usr/local/bin/glpsol"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-reactomegsa.data.
shpc-registry automated BioContainers addition for bioconductor-reactomegsa.data
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-reactomegsa.data
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-reactomegsa.data:1.8.0--r41hdfd78af_1
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-reactomegsa.data/1.8.0--r41hdfd78af_1
$ module help quay.io/biocontainers/bioconductor-reactomegsa.data/1.8.0--r41hdfd78af_1
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-reactomegsa.data-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-reactomegsa.data-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-reactomegsa.data-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-reactomegsa.data-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-reactomegsa.data-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-reactomegsa.data-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### .bioconductor-reactomegsa.data-post-link.sh

```bash
$ singularity exec <container> /usr/local/bin/.bioconductor-reactomegsa.data-post-link.sh
$ podman run --it --rm --entrypoint /usr/local/bin/.bioconductor-reactomegsa.data-post-link.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/.bioconductor-reactomegsa.data-post-link.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### .bioconductor-reactomegsa.data-pre-unlink.sh

```bash
$ singularity exec <container> /usr/local/bin/.bioconductor-reactomegsa.data-pre-unlink.sh
$ podman run --it --rm --entrypoint /usr/local/bin/.bioconductor-reactomegsa.data-pre-unlink.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/.bioconductor-reactomegsa.data-pre-unlink.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### geosop

```bash
$ singularity exec <container> /usr/local/bin/geosop
$ podman run --it --rm --entrypoint /usr/local/bin/geosop   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/geosop   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### geos-config

```bash
$ singularity exec <container> /usr/local/bin/geos-config
$ podman run --it --rm --entrypoint /usr/local/bin/geos-config   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/geos-config   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### glpsol

```bash
$ singularity exec <container> /usr/local/bin/glpsol
$ podman run --it --rm --entrypoint /usr/local/bin/glpsol   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/glpsol   -v ${PWD} -w ${PWD} <container> -c " $@"
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