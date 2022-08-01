---
layout: container
name:  "quay.io/pawsey/openfoam-org"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/singularity-hpc/blob/main/registry/quay.io/pawsey/openfoam-org/container.yaml"
updated_at: "2022-07-11 07:58:25.719378"
container_url: "https://quay.io/repository/pawsey/openfoam-org"

versions:
 - "8"
 - "7"
 - "5.x"
 - "2.4.x"
 - "2.2.0"
description: "OpenFOAM (openfoam.org) images built on top of MPICH."
---

This module is a singularity container wrapper for quay.io/pawsey/openfoam-org.
OpenFOAM (openfoam.org) images built on top of MPICH.
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/pawsey/openfoam-org
```

Or a specific version:

```bash
$ shpc install quay.io/pawsey/openfoam-org:8
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/pawsey/openfoam-org/8
$ module help quay.io/pawsey/openfoam-org/8
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### openfoam-org-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### openfoam-org-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### openfoam-org-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### openfoam-org-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### openfoam-org-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### openfoam-org-inspect-deffile:

```bash
$ singularity inspect -d <container>
```



#### openfoam-org

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