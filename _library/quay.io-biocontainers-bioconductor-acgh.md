---
layout: container
name:  "quay.io/biocontainers/bioconductor-acgh"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-acgh/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-acgh/container.yaml"
updated_at: "2022-11-19 02:11:29.554092"
latest: "1.76.0--r42hc247a5b_0"
container_url: "https://biocontainers.pro/tools/bioconductor-acgh"

versions:
 - "1.72.0--r41hc247a5b_2"
 - "1.76.0--r42hc247a5b_0"
description: "shpc-registry automated BioContainers addition for bioconductor-acgh"
config: {"url": "https://biocontainers.pro/tools/bioconductor-acgh", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-acgh", "latest": {"1.76.0--r42hc247a5b_0": "sha256:b60ea47b739b76ba4a4bc5c27e5362bfd840047d095dc586a65b7a3ccd5d81ac"}, "tags": {"1.72.0--r41hc247a5b_2": "sha256:54c79a871b3ecc03fd410be5b0657ede25657bc808229653fe5eee65986988a9", "1.76.0--r42hc247a5b_0": "sha256:b60ea47b739b76ba4a4bc5c27e5362bfd840047d095dc586a65b7a3ccd5d81ac"}, "docker": "quay.io/biocontainers/bioconductor-acgh"}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-acgh.
shpc-registry automated BioContainers addition for bioconductor-acgh
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-acgh
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-acgh:1.76.0--r42hc247a5b_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-acgh/1.76.0--r42hc247a5b_0
$ module help quay.io/biocontainers/bioconductor-acgh/1.76.0--r42hc247a5b_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-acgh-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-acgh-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-acgh-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-acgh-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-acgh-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-acgh-inspect-deffile:

```bash
$ singularity inspect -d <container>
```



#### bioconductor-acgh

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