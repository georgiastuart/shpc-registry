---
layout: container
name:  "quay.io/biocontainers/proteomiqon-alignmentbasedquantstatistics"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/proteomiqon-alignmentbasedquantstatistics/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/proteomiqon-alignmentbasedquantstatistics/container.yaml"
updated_at: "2023-03-13 02:54:45.423168"
latest: "0.0.3--hdfd78af_0"
container_url: "https://biocontainers.pro/tools/proteomiqon-alignmentbasedquantstatistics"
aliases:
 - "lttng-gen-tp"
 - "proteomiqon-alignmentbasedquantstatistics"
versions:
 - "0.0.3--hdfd78af_0"
description: "singularity registry hpc automated addition for proteomiqon-alignmentbasedquantstatistics"
config: {"url": "https://biocontainers.pro/tools/proteomiqon-alignmentbasedquantstatistics", "maintainer": "@vsoch", "description": "singularity registry hpc automated addition for proteomiqon-alignmentbasedquantstatistics", "latest": {"0.0.3--hdfd78af_0": "sha256:b5aabd129f44ec177e2af0128989766785fad5405d399cd3fb89349628240fa1"}, "tags": {"0.0.3--hdfd78af_0": "sha256:b5aabd129f44ec177e2af0128989766785fad5405d399cd3fb89349628240fa1"}, "docker": "quay.io/biocontainers/proteomiqon-alignmentbasedquantstatistics", "aliases": {"lttng-gen-tp": "/usr/local/bin/lttng-gen-tp", "proteomiqon-alignmentbasedquantstatistics": "/usr/local/bin/proteomiqon-alignmentbasedquantstatistics"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/proteomiqon-alignmentbasedquantstatistics.
singularity registry hpc automated addition for proteomiqon-alignmentbasedquantstatistics
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/proteomiqon-alignmentbasedquantstatistics
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/proteomiqon-alignmentbasedquantstatistics:0.0.3--hdfd78af_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/proteomiqon-alignmentbasedquantstatistics/0.0.3--hdfd78af_0
$ module help quay.io/biocontainers/proteomiqon-alignmentbasedquantstatistics/0.0.3--hdfd78af_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### proteomiqon-alignmentbasedquantstatistics-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### proteomiqon-alignmentbasedquantstatistics-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### proteomiqon-alignmentbasedquantstatistics-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### proteomiqon-alignmentbasedquantstatistics-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### proteomiqon-alignmentbasedquantstatistics-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### proteomiqon-alignmentbasedquantstatistics-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### lttng-gen-tp

```bash
$ singularity exec <container> /usr/local/bin/lttng-gen-tp
$ podman run --it --rm --entrypoint /usr/local/bin/lttng-gen-tp   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/lttng-gen-tp   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### proteomiqon-alignmentbasedquantstatistics

```bash
$ singularity exec <container> /usr/local/bin/proteomiqon-alignmentbasedquantstatistics
$ podman run --it --rm --entrypoint /usr/local/bin/proteomiqon-alignmentbasedquantstatistics   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/proteomiqon-alignmentbasedquantstatistics   -v ${PWD} -w ${PWD} <container> -c " $@"
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