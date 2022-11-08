---
layout: container
name:  "quay.io/biocontainers/fastool"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/fastool/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/fastool/container.yaml"
updated_at: "2022-11-08 00:15:22.553417"
latest: "0.1.4--h7132678_6"
container_url: "https://biocontainers.pro/tools/fastool"
aliases:
 - "fastool"
versions:
 - "0.1.4--h7132678_6"
description: "shpc-registry automated BioContainers addition for fastool"
config: {"url": "https://biocontainers.pro/tools/fastool", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for fastool", "latest": {"0.1.4--h7132678_6": "sha256:1ae1a12b41850b8be6edfe37c7445f1c525023d1bcbd189b495d490b3f9bfc27"}, "tags": {"0.1.4--h7132678_6": "sha256:1ae1a12b41850b8be6edfe37c7445f1c525023d1bcbd189b495d490b3f9bfc27"}, "docker": "quay.io/biocontainers/fastool", "aliases": {"fastool": "/usr/local/bin/fastool"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/fastool.
shpc-registry automated BioContainers addition for fastool
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/fastool
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/fastool:0.1.4--h7132678_6
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/fastool/0.1.4--h7132678_6
$ module help quay.io/biocontainers/fastool/0.1.4--h7132678_6
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### fastool-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### fastool-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### fastool-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### fastool-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### fastool-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### fastool-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### fastool

```bash
$ singularity exec <container> /usr/local/bin/fastool
$ podman run --it --rm --entrypoint /usr/local/bin/fastool   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/fastool   -v ${PWD} -w ${PWD} <container> -c " $@"
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