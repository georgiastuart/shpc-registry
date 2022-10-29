---
layout: container
name:  "quay.io/biocontainers/perl-module-load"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/perl-module-load/container.yaml"
config_url: "https://raw.githubusercontent.com//singularityhub/shpc-registry/main/quay.io/biocontainers/perl-module-load/container.yaml"
updated_at: "2022-10-29 17:55:56.195680"
latest: "0.34--pl5321hdfd78af_0"
container_url: "https://biocontainers.pro/tools/perl-module-load"

versions:
 - "0.34--pl5321hdfd78af_0"
description: "shpc-registry automated BioContainers addition for perl-module-load"
config: {"url": "https://biocontainers.pro/tools/perl-module-load", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for perl-module-load", "latest": {"0.34--pl5321hdfd78af_0": "sha256:ed21018fd1c3ae62e722956b5c5688c20c8bd25f62535115a13c0e2025b4f8ac"}, "tags": {"0.34--pl5321hdfd78af_0": "sha256:ed21018fd1c3ae62e722956b5c5688c20c8bd25f62535115a13c0e2025b4f8ac"}, "docker": "quay.io/biocontainers/perl-module-load"}
---

This module is a singularity container wrapper for quay.io/biocontainers/perl-module-load.
shpc-registry automated BioContainers addition for perl-module-load
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/perl-module-load
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/perl-module-load:0.34--pl5321hdfd78af_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/perl-module-load/0.34--pl5321hdfd78af_0
$ module help quay.io/biocontainers/perl-module-load/0.34--pl5321hdfd78af_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### perl-module-load-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### perl-module-load-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### perl-module-load-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### perl-module-load-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### perl-module-load-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### perl-module-load-inspect-deffile:

```bash
$ singularity inspect -d <container>
```



#### perl-module-load

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