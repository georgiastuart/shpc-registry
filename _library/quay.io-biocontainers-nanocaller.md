---
layout: container
name:  "quay.io/biocontainers/nanocaller"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/nanocaller/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/nanocaller/container.yaml"
updated_at: "2023-03-13 03:38:08.013663"
latest: "3.0.0--hdfd78af_0"
container_url: "https://biocontainers.pro/tools/nanocaller"
aliases:
 - "NanoCaller"
 - "import_pb_to_tensorboard"
 - "vcfnormalizesvs"
 - "vcfnull2ref"
 - "vcfunphase"
 - "whatshap"
 - "plotBfst.R"
 - "plotHapLrt.R"
 - "plotHaplotypes.R"
 - "plotPfst.R"
 - "plotSmoothed.R"
 - "plotWCfst.R"
 - "plotXPEHH.R"
 - "plot_roc.r"
 - "abba-baba"
 - "bFst"
 - "bed2region"
 - "bgziptabix"
 - "dumpContigsFromHeader"
 - "genotypeSummary"
 - "hapLrt"
 - "iHS"
 - "meltEHH"
 - "normalize-iHS"
 - "pFst"
 - "pVst"
 - "permuteGPAT++"
 - "permuteSmooth"
 - "plotHaps"
 - "popStats"
 - "segmentFst"
versions:
 - "3.0.0--hdfd78af_0"
description: "singularity registry hpc automated addition for nanocaller"
config: {"url": "https://biocontainers.pro/tools/nanocaller", "maintainer": "@vsoch", "description": "singularity registry hpc automated addition for nanocaller", "latest": {"3.0.0--hdfd78af_0": "sha256:1343b132b0b56dfdccd447fe7e0f5635738b901da734c504eea51ab16c5d6291"}, "tags": {"3.0.0--hdfd78af_0": "sha256:1343b132b0b56dfdccd447fe7e0f5635738b901da734c504eea51ab16c5d6291"}, "docker": "quay.io/biocontainers/nanocaller", "aliases": {"NanoCaller": "/usr/local/bin/NanoCaller", "import_pb_to_tensorboard": "/usr/local/bin/import_pb_to_tensorboard", "vcfnormalizesvs": "/usr/local/bin/vcfnormalizesvs", "vcfnull2ref": "/usr/local/bin/vcfnull2ref", "vcfunphase": "/usr/local/bin/vcfunphase", "whatshap": "/usr/local/bin/whatshap", "plotBfst.R": "/usr/local/bin/plotBfst.R", "plotHapLrt.R": "/usr/local/bin/plotHapLrt.R", "plotHaplotypes.R": "/usr/local/bin/plotHaplotypes.R", "plotPfst.R": "/usr/local/bin/plotPfst.R", "plotSmoothed.R": "/usr/local/bin/plotSmoothed.R", "plotWCfst.R": "/usr/local/bin/plotWCfst.R", "plotXPEHH.R": "/usr/local/bin/plotXPEHH.R", "plot_roc.r": "/usr/local/bin/plot_roc.r", "abba-baba": "/usr/local/bin/abba-baba", "bFst": "/usr/local/bin/bFst", "bed2region": "/usr/local/bin/bed2region", "bgziptabix": "/usr/local/bin/bgziptabix", "dumpContigsFromHeader": "/usr/local/bin/dumpContigsFromHeader", "genotypeSummary": "/usr/local/bin/genotypeSummary", "hapLrt": "/usr/local/bin/hapLrt", "iHS": "/usr/local/bin/iHS", "meltEHH": "/usr/local/bin/meltEHH", "normalize-iHS": "/usr/local/bin/normalize-iHS", "pFst": "/usr/local/bin/pFst", "pVst": "/usr/local/bin/pVst", "permuteGPAT++": "/usr/local/bin/permuteGPAT++", "permuteSmooth": "/usr/local/bin/permuteSmooth", "plotHaps": "/usr/local/bin/plotHaps", "popStats": "/usr/local/bin/popStats", "segmentFst": "/usr/local/bin/segmentFst"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/nanocaller.
singularity registry hpc automated addition for nanocaller
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/nanocaller
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/nanocaller:3.0.0--hdfd78af_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/nanocaller/3.0.0--hdfd78af_0
$ module help quay.io/biocontainers/nanocaller/3.0.0--hdfd78af_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### nanocaller-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### nanocaller-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### nanocaller-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### nanocaller-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### nanocaller-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### nanocaller-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### NanoCaller

```bash
$ singularity exec <container> /usr/local/bin/NanoCaller
$ podman run --it --rm --entrypoint /usr/local/bin/NanoCaller   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/NanoCaller   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### import_pb_to_tensorboard

```bash
$ singularity exec <container> /usr/local/bin/import_pb_to_tensorboard
$ podman run --it --rm --entrypoint /usr/local/bin/import_pb_to_tensorboard   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/import_pb_to_tensorboard   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### vcfnormalizesvs

```bash
$ singularity exec <container> /usr/local/bin/vcfnormalizesvs
$ podman run --it --rm --entrypoint /usr/local/bin/vcfnormalizesvs   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/vcfnormalizesvs   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### vcfnull2ref

```bash
$ singularity exec <container> /usr/local/bin/vcfnull2ref
$ podman run --it --rm --entrypoint /usr/local/bin/vcfnull2ref   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/vcfnull2ref   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### vcfunphase

```bash
$ singularity exec <container> /usr/local/bin/vcfunphase
$ podman run --it --rm --entrypoint /usr/local/bin/vcfunphase   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/vcfunphase   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### whatshap

```bash
$ singularity exec <container> /usr/local/bin/whatshap
$ podman run --it --rm --entrypoint /usr/local/bin/whatshap   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/whatshap   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### plotBfst.R

```bash
$ singularity exec <container> /usr/local/bin/plotBfst.R
$ podman run --it --rm --entrypoint /usr/local/bin/plotBfst.R   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/plotBfst.R   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### plotHapLrt.R

```bash
$ singularity exec <container> /usr/local/bin/plotHapLrt.R
$ podman run --it --rm --entrypoint /usr/local/bin/plotHapLrt.R   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/plotHapLrt.R   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### plotHaplotypes.R

```bash
$ singularity exec <container> /usr/local/bin/plotHaplotypes.R
$ podman run --it --rm --entrypoint /usr/local/bin/plotHaplotypes.R   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/plotHaplotypes.R   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### plotPfst.R

```bash
$ singularity exec <container> /usr/local/bin/plotPfst.R
$ podman run --it --rm --entrypoint /usr/local/bin/plotPfst.R   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/plotPfst.R   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### plotSmoothed.R

```bash
$ singularity exec <container> /usr/local/bin/plotSmoothed.R
$ podman run --it --rm --entrypoint /usr/local/bin/plotSmoothed.R   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/plotSmoothed.R   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### plotWCfst.R

```bash
$ singularity exec <container> /usr/local/bin/plotWCfst.R
$ podman run --it --rm --entrypoint /usr/local/bin/plotWCfst.R   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/plotWCfst.R   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### plotXPEHH.R

```bash
$ singularity exec <container> /usr/local/bin/plotXPEHH.R
$ podman run --it --rm --entrypoint /usr/local/bin/plotXPEHH.R   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/plotXPEHH.R   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### plot_roc.r

```bash
$ singularity exec <container> /usr/local/bin/plot_roc.r
$ podman run --it --rm --entrypoint /usr/local/bin/plot_roc.r   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/plot_roc.r   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### abba-baba

```bash
$ singularity exec <container> /usr/local/bin/abba-baba
$ podman run --it --rm --entrypoint /usr/local/bin/abba-baba   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/abba-baba   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### bFst

```bash
$ singularity exec <container> /usr/local/bin/bFst
$ podman run --it --rm --entrypoint /usr/local/bin/bFst   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/bFst   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### bed2region

```bash
$ singularity exec <container> /usr/local/bin/bed2region
$ podman run --it --rm --entrypoint /usr/local/bin/bed2region   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/bed2region   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### bgziptabix

```bash
$ singularity exec <container> /usr/local/bin/bgziptabix
$ podman run --it --rm --entrypoint /usr/local/bin/bgziptabix   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/bgziptabix   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### dumpContigsFromHeader

```bash
$ singularity exec <container> /usr/local/bin/dumpContigsFromHeader
$ podman run --it --rm --entrypoint /usr/local/bin/dumpContigsFromHeader   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/dumpContigsFromHeader   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### genotypeSummary

```bash
$ singularity exec <container> /usr/local/bin/genotypeSummary
$ podman run --it --rm --entrypoint /usr/local/bin/genotypeSummary   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/genotypeSummary   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### hapLrt

```bash
$ singularity exec <container> /usr/local/bin/hapLrt
$ podman run --it --rm --entrypoint /usr/local/bin/hapLrt   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/hapLrt   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### iHS

```bash
$ singularity exec <container> /usr/local/bin/iHS
$ podman run --it --rm --entrypoint /usr/local/bin/iHS   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/iHS   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### meltEHH

```bash
$ singularity exec <container> /usr/local/bin/meltEHH
$ podman run --it --rm --entrypoint /usr/local/bin/meltEHH   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/meltEHH   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### normalize-iHS

```bash
$ singularity exec <container> /usr/local/bin/normalize-iHS
$ podman run --it --rm --entrypoint /usr/local/bin/normalize-iHS   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/normalize-iHS   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### pFst

```bash
$ singularity exec <container> /usr/local/bin/pFst
$ podman run --it --rm --entrypoint /usr/local/bin/pFst   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/pFst   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### pVst

```bash
$ singularity exec <container> /usr/local/bin/pVst
$ podman run --it --rm --entrypoint /usr/local/bin/pVst   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/pVst   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### permuteGPAT++

```bash
$ singularity exec <container> /usr/local/bin/permuteGPAT++
$ podman run --it --rm --entrypoint /usr/local/bin/permuteGPAT++   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/permuteGPAT++   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### permuteSmooth

```bash
$ singularity exec <container> /usr/local/bin/permuteSmooth
$ podman run --it --rm --entrypoint /usr/local/bin/permuteSmooth   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/permuteSmooth   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### plotHaps

```bash
$ singularity exec <container> /usr/local/bin/plotHaps
$ podman run --it --rm --entrypoint /usr/local/bin/plotHaps   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/plotHaps   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### popStats

```bash
$ singularity exec <container> /usr/local/bin/popStats
$ podman run --it --rm --entrypoint /usr/local/bin/popStats   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/popStats   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### segmentFst

```bash
$ singularity exec <container> /usr/local/bin/segmentFst
$ podman run --it --rm --entrypoint /usr/local/bin/segmentFst   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/segmentFst   -v ${PWD} -w ${PWD} <container> -c " $@"
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