---
layout: container
name:  "quay.io/biocontainers/pangolin-data"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/pangolin-data/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/pangolin-data/container.yaml"
updated_at: "2023-03-29 00:18:17.439501"
latest: "1.18.1.1--pyh7cba7a3_0"
container_url: "https://biocontainers.pro/tools/pangolin-data"
aliases:
 - "pangolin_data"
 - "2to3-3.10"
 - "idle3.10"
 - "pydoc3.10"
 - "python3.10"
 - "python3.10-config"
 - "python3.1"
versions:
 - "1.9--pyh5e36f6f_0"
 - "1.18.1.1--pyh7cba7a3_0"
 - "1.17--pyh7cba7a3_0"
 - "1.16--pyh7cba7a3_0"
 - "1.15.1--pyh7cba7a3_0"
 - "1.14--pyh5e36f6f_0"
description: "singularity registry hpc automated addition for pangolin-data"
config: {"url": "https://biocontainers.pro/tools/pangolin-data", "maintainer": "@vsoch", "description": "singularity registry hpc automated addition for pangolin-data", "latest": {"1.18.1.1--pyh7cba7a3_0": "sha256:b7ab5e8340e5a5129444aec7f5919e0a53fe276934b32cecb88769a142984e0a"}, "tags": {"1.9--pyh5e36f6f_0": "sha256:986d54d7de55e4764ee8a9eb195a46beb883fb9638879d559c815c9bd11d0f5c", "1.18.1.1--pyh7cba7a3_0": "sha256:b7ab5e8340e5a5129444aec7f5919e0a53fe276934b32cecb88769a142984e0a", "1.17--pyh7cba7a3_0": "sha256:bf3a497e0fbc90031a42813fe2a796b2975483b7232522f01238588dd7b07665", "1.16--pyh7cba7a3_0": "sha256:7cc3372b6595aa1437a34cbf0308557bba43827d8edeb3de6ef07c05fc0ddf20", "1.15.1--pyh7cba7a3_0": "sha256:52a9a687c37618bb0a8f07aae02dd2d53cf498e150c781ee571366f9ffab7295", "1.14--pyh5e36f6f_0": "sha256:9f01d930782ff756a372cd84553cf8444e329ef4a4dbfc2c5c690ef124b803ed"}, "docker": "quay.io/biocontainers/pangolin-data", "aliases": {"pangolin_data": "/usr/local/bin/pangolin_data", "2to3-3.10": "/usr/local/bin/2to3-3.10", "idle3.10": "/usr/local/bin/idle3.10", "pydoc3.10": "/usr/local/bin/pydoc3.10", "python3.10": "/usr/local/bin/python3.10", "python3.10-config": "/usr/local/bin/python3.10-config", "python3.1": "/usr/local/bin/python3.1"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/pangolin-data.
singularity registry hpc automated addition for pangolin-data
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/pangolin-data
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/pangolin-data:1.18.1.1--pyh7cba7a3_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/pangolin-data/1.18.1.1--pyh7cba7a3_0
$ module help quay.io/biocontainers/pangolin-data/1.18.1.1--pyh7cba7a3_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### pangolin-data-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### pangolin-data-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### pangolin-data-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### pangolin-data-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### pangolin-data-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### pangolin-data-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### pangolin_data

```bash
$ singularity exec <container> /usr/local/bin/pangolin_data
$ podman run --it --rm --entrypoint /usr/local/bin/pangolin_data   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/pangolin_data   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### 2to3-3.10

```bash
$ singularity exec <container> /usr/local/bin/2to3-3.10
$ podman run --it --rm --entrypoint /usr/local/bin/2to3-3.10   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/2to3-3.10   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### idle3.10

```bash
$ singularity exec <container> /usr/local/bin/idle3.10
$ podman run --it --rm --entrypoint /usr/local/bin/idle3.10   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/idle3.10   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### pydoc3.10

```bash
$ singularity exec <container> /usr/local/bin/pydoc3.10
$ podman run --it --rm --entrypoint /usr/local/bin/pydoc3.10   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/pydoc3.10   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### python3.10

```bash
$ singularity exec <container> /usr/local/bin/python3.10
$ podman run --it --rm --entrypoint /usr/local/bin/python3.10   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/python3.10   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### python3.10-config

```bash
$ singularity exec <container> /usr/local/bin/python3.10-config
$ podman run --it --rm --entrypoint /usr/local/bin/python3.10-config   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/python3.10-config   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### python3.1

```bash
$ singularity exec <container> /usr/local/bin/python3.1
$ podman run --it --rm --entrypoint /usr/local/bin/python3.1   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/python3.1   -v ${PWD} -w ${PWD} <container> -c " $@"
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