---
layout: container
name:  "quay.io/biocontainers/mupbwt"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/mupbwt/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/mupbwt/container.yaml"
updated_at: "2023-03-08 03:05:28.941213"
latest: "0.1.2--hea94271_0"
container_url: "https://biocontainers.pro/tools/mupbwt"
aliases:
 - "mupbwt"
 - "htsfile"
 - "bgzip"
 - "tabix"
versions:
 - "0.1.2--hea94271_0"
description: "singularity registry hpc automated addition for mupbwt"
config: {"url": "https://biocontainers.pro/tools/mupbwt", "maintainer": "@vsoch", "description": "singularity registry hpc automated addition for mupbwt", "latest": {"0.1.2--hea94271_0": "sha256:d24e35d23ed0799552d3486c95eff7b98541f0e44fc3d07390ae897eea94297d"}, "tags": {"0.1.2--hea94271_0": "sha256:d24e35d23ed0799552d3486c95eff7b98541f0e44fc3d07390ae897eea94297d"}, "docker": "quay.io/biocontainers/mupbwt", "aliases": {"mupbwt": "/usr/local/bin/mupbwt", "htsfile": "/usr/local/bin/htsfile", "bgzip": "/usr/local/bin/bgzip", "tabix": "/usr/local/bin/tabix"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/mupbwt.
singularity registry hpc automated addition for mupbwt
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/mupbwt
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/mupbwt:0.1.2--hea94271_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/mupbwt/0.1.2--hea94271_0
$ module help quay.io/biocontainers/mupbwt/0.1.2--hea94271_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### mupbwt-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### mupbwt-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### mupbwt-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### mupbwt-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### mupbwt-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### mupbwt-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### mupbwt

```bash
$ singularity exec <container> /usr/local/bin/mupbwt
$ podman run --it --rm --entrypoint /usr/local/bin/mupbwt   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/mupbwt   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### htsfile

```bash
$ singularity exec <container> /usr/local/bin/htsfile
$ podman run --it --rm --entrypoint /usr/local/bin/htsfile   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/htsfile   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### bgzip

```bash
$ singularity exec <container> /usr/local/bin/bgzip
$ podman run --it --rm --entrypoint /usr/local/bin/bgzip   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/bgzip   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### tabix

```bash
$ singularity exec <container> /usr/local/bin/tabix
$ podman run --it --rm --entrypoint /usr/local/bin/tabix   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/tabix   -v ${PWD} -w ${PWD} <container> -c " $@"
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