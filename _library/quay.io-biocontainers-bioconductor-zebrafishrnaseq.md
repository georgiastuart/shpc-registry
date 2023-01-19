---
layout: container
name:  "quay.io/biocontainers/bioconductor-zebrafishrnaseq"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-zebrafishrnaseq/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-zebrafishrnaseq/container.yaml"
updated_at: "2023-01-19 03:45:24.891361"
latest: "1.17.0--r42hdfd78af_0"
container_url: "https://biocontainers.pro/tools/bioconductor-zebrafishrnaseq"
aliases:
 - "x86_64-conda-linux-gnu-gfortran.bin"
versions:
 - "1.9.0--r40_0"
 - "1.17.0--r42hdfd78af_0"
 - "1.14.0--r41hdfd78af_1"
 - "1.12.0--r41hdfd78af_0"
 - "1.10.0--r40hdfd78af_1"
description: "shpc-registry automated BioContainers addition for bioconductor-zebrafishrnaseq"
config: {"url": "https://biocontainers.pro/tools/bioconductor-zebrafishrnaseq", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-zebrafishrnaseq", "latest": {"1.17.0--r42hdfd78af_0": "sha256:7679f2ff753439a35ba3f84fc8dece993c9c34189ed804a7ec1e236e20971901"}, "tags": {"1.9.0--r40_0": "sha256:7221fb618f6399b2b2a6672da2882ef6c15a52498e4bc0a37218a03ae0c270af", "1.17.0--r42hdfd78af_0": "sha256:7679f2ff753439a35ba3f84fc8dece993c9c34189ed804a7ec1e236e20971901", "1.14.0--r41hdfd78af_1": "sha256:9a571d5f70ff4660f253eed45b6f6e5679c3272a6f13ce27960fdb026dbe38e3", "1.12.0--r41hdfd78af_0": "sha256:5ea0ecb25d1a887f385198a2c9326b89eef6bf61e2aface1c7b54504976f221e", "1.10.0--r40hdfd78af_1": "sha256:6af77b16104be663df98052d37bf6e78be5660eb2048ba5243bee6f9d197bc7e"}, "docker": "quay.io/biocontainers/bioconductor-zebrafishrnaseq", "aliases": {"x86_64-conda-linux-gnu-gfortran.bin": "/usr/local/bin/x86_64-conda-linux-gnu-gfortran.bin"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-zebrafishrnaseq.
shpc-registry automated BioContainers addition for bioconductor-zebrafishrnaseq
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-zebrafishrnaseq
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-zebrafishrnaseq:1.17.0--r42hdfd78af_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-zebrafishrnaseq/1.17.0--r42hdfd78af_0
$ module help quay.io/biocontainers/bioconductor-zebrafishrnaseq/1.17.0--r42hdfd78af_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-zebrafishrnaseq-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-zebrafishrnaseq-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-zebrafishrnaseq-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-zebrafishrnaseq-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-zebrafishrnaseq-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-zebrafishrnaseq-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### x86_64-conda-linux-gnu-gfortran.bin

```bash
$ singularity exec <container> /usr/local/bin/x86_64-conda-linux-gnu-gfortran.bin
$ podman run --it --rm --entrypoint /usr/local/bin/x86_64-conda-linux-gnu-gfortran.bin   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/x86_64-conda-linux-gnu-gfortran.bin   -v ${PWD} -w ${PWD} <container> -c " $@"
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