---
layout: container
name:  "quay.io/biocontainers/perl-convert-binhex"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/perl-convert-binhex/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/perl-convert-binhex/container.yaml"
updated_at: "2022-11-08 00:03:43.812427"
latest: "1.125--pl5321hdfd78af_2"
container_url: "https://biocontainers.pro/tools/perl-convert-binhex"
aliases:
 - "binhex.pl"
 - "debinhex.pl"
 - "perl5.32.1"
 - "streamzip"
versions:
 - "1.125--pl5321hdfd78af_2"
description: "shpc-registry automated BioContainers addition for perl-convert-binhex"
config: {"url": "https://biocontainers.pro/tools/perl-convert-binhex", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for perl-convert-binhex", "latest": {"1.125--pl5321hdfd78af_2": "sha256:5e2c1bfd9d7b73eb8213f0ffb69fa5d2e9e31ba47dd5da0213492ed536588163"}, "tags": {"1.125--pl5321hdfd78af_2": "sha256:5e2c1bfd9d7b73eb8213f0ffb69fa5d2e9e31ba47dd5da0213492ed536588163"}, "docker": "quay.io/biocontainers/perl-convert-binhex", "aliases": {"binhex.pl": "/usr/local/bin/binhex.pl", "debinhex.pl": "/usr/local/bin/debinhex.pl", "perl5.32.1": "/usr/local/bin/perl5.32.1", "streamzip": "/usr/local/bin/streamzip"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/perl-convert-binhex.
shpc-registry automated BioContainers addition for perl-convert-binhex
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/perl-convert-binhex
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/perl-convert-binhex:1.125--pl5321hdfd78af_2
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/perl-convert-binhex/1.125--pl5321hdfd78af_2
$ module help quay.io/biocontainers/perl-convert-binhex/1.125--pl5321hdfd78af_2
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### perl-convert-binhex-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### perl-convert-binhex-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### perl-convert-binhex-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### perl-convert-binhex-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### perl-convert-binhex-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### perl-convert-binhex-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### binhex.pl

```bash
$ singularity exec <container> /usr/local/bin/binhex.pl
$ podman run --it --rm --entrypoint /usr/local/bin/binhex.pl   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/binhex.pl   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### debinhex.pl

```bash
$ singularity exec <container> /usr/local/bin/debinhex.pl
$ podman run --it --rm --entrypoint /usr/local/bin/debinhex.pl   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/debinhex.pl   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### perl5.32.1

```bash
$ singularity exec <container> /usr/local/bin/perl5.32.1
$ podman run --it --rm --entrypoint /usr/local/bin/perl5.32.1   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/perl5.32.1   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### streamzip

```bash
$ singularity exec <container> /usr/local/bin/streamzip
$ podman run --it --rm --entrypoint /usr/local/bin/streamzip   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/streamzip   -v ${PWD} -w ${PWD} <container> -c " $@"
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