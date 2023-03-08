---
layout: container
name:  "quay.io/biocontainers/tidk"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/tidk/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/tidk/container.yaml"
updated_at: "2023-03-08 03:12:24.605951"
latest: "0.2.1--h87f3376_1"
container_url: "https://biocontainers.pro/tools/tidk"
aliases:
 - "tidk"
versions:
 - "0.2.1--h87f3376_1"
description: "singularity registry hpc automated addition for tidk"
config: {"url": "https://biocontainers.pro/tools/tidk", "maintainer": "@vsoch", "description": "singularity registry hpc automated addition for tidk", "latest": {"0.2.1--h87f3376_1": "sha256:920d2cf7e33c7450eb5e85f7eaa5e30d9de2c2e765445d5b7e92c55bb8f3e5fc"}, "tags": {"0.2.1--h87f3376_1": "sha256:920d2cf7e33c7450eb5e85f7eaa5e30d9de2c2e765445d5b7e92c55bb8f3e5fc"}, "docker": "quay.io/biocontainers/tidk", "aliases": {"tidk": "/usr/local/bin/tidk"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/tidk.
singularity registry hpc automated addition for tidk
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/tidk
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/tidk:0.2.1--h87f3376_1
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/tidk/0.2.1--h87f3376_1
$ module help quay.io/biocontainers/tidk/0.2.1--h87f3376_1
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### tidk-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### tidk-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### tidk-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### tidk-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### tidk-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### tidk-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### tidk

```bash
$ singularity exec <container> /usr/local/bin/tidk
$ podman run --it --rm --entrypoint /usr/local/bin/tidk   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/tidk   -v ${PWD} -w ${PWD} <container> -c " $@"
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