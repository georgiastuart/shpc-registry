---
layout: container
name:  "quay.io/biocontainers/sneep"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/sneep/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/sneep/container.yaml"
updated_at: "2023-03-13 03:34:04.495595"
latest: "0.4--py39h7cff6ad_0"
container_url: "https://biocontainers.pro/tools/sneep"
aliases:
 - "HandleInOutput"
 - "HandleInOutput.cpp"
 - "HandleInOutput.hpp"
 - "Makefile.bak"
 - "Matrix"
 - "Matrix_new.cpp"
 - "Matrix_new.hpp"
 - "callBashCommand"
 - "callBashCommand.cpp"
 - "callBashCommand.hpp"
 - "differentialBindingAffinity_multipleSNPs"
 - "differentialBindingAffinity_multipleSNPs.cpp"
 - "estimateScalePerMotif.sh"
 - "findZerosEachMotif.py"
 - "histogram.R"
 - "pvalue"
 - "pvalue_copy.cpp"
 - "pvalue_copy.hpp"
 - "randomRsIds_2.0"
 - "sampleRandomRsIDs2.cpp"
 - "sampleRandomRsIDs2.hpp"
 - "seperatePFMs.py"
 - "seperatePFMsAndCheckActivity.py"
 - "Makefile"
 - "shiftBed"
 - "annotateBed"
 - "bamToBed"
 - "bamToFastq"
 - "bed12ToBed6"
 - "bedToBam"
 - "bedToIgv"
 - "bedpeToBam"
 - "bedtools"
 - "closestBed"
 - "clusterBed"
 - "complementBed"
 - "coverageBed"
 - "expandCols"
 - "fastaFromBed"
 - "flankBed"
 - "genomeCoverageBed"
 - "getOverlap"
 - "groupBy"
 - "intersectBed"
 - "linksBed"
 - "mapBed"
 - "maskFastaFromBed"
 - "mergeBed"
versions:
 - "0.4--py39h7cff6ad_0"
description: "singularity registry hpc automated addition for sneep"
config: {"url": "https://biocontainers.pro/tools/sneep", "maintainer": "@vsoch", "description": "singularity registry hpc automated addition for sneep", "latest": {"0.4--py39h7cff6ad_0": "sha256:9015c0118ebc43589ca1368f31842e997b1f9abd79acbc2fc7516fabae0ea765"}, "tags": {"0.4--py39h7cff6ad_0": "sha256:9015c0118ebc43589ca1368f31842e997b1f9abd79acbc2fc7516fabae0ea765"}, "docker": "quay.io/biocontainers/sneep", "aliases": {"HandleInOutput": "/usr/local/bin/HandleInOutput", "HandleInOutput.cpp": "/usr/local/bin/HandleInOutput.cpp", "HandleInOutput.hpp": "/usr/local/bin/HandleInOutput.hpp", "Makefile.bak": "/usr/local/bin/Makefile.bak", "Matrix": "/usr/local/bin/Matrix", "Matrix_new.cpp": "/usr/local/bin/Matrix_new.cpp", "Matrix_new.hpp": "/usr/local/bin/Matrix_new.hpp", "callBashCommand": "/usr/local/bin/callBashCommand", "callBashCommand.cpp": "/usr/local/bin/callBashCommand.cpp", "callBashCommand.hpp": "/usr/local/bin/callBashCommand.hpp", "differentialBindingAffinity_multipleSNPs": "/usr/local/bin/differentialBindingAffinity_multipleSNPs", "differentialBindingAffinity_multipleSNPs.cpp": "/usr/local/bin/differentialBindingAffinity_multipleSNPs.cpp", "estimateScalePerMotif.sh": "/usr/local/bin/estimateScalePerMotif.sh", "findZerosEachMotif.py": "/usr/local/bin/findZerosEachMotif.py", "histogram.R": "/usr/local/bin/histogram.R", "pvalue": "/usr/local/bin/pvalue", "pvalue_copy.cpp": "/usr/local/bin/pvalue_copy.cpp", "pvalue_copy.hpp": "/usr/local/bin/pvalue_copy.hpp", "randomRsIds_2.0": "/usr/local/bin/randomRsIds_2.0", "sampleRandomRsIDs2.cpp": "/usr/local/bin/sampleRandomRsIDs2.cpp", "sampleRandomRsIDs2.hpp": "/usr/local/bin/sampleRandomRsIDs2.hpp", "seperatePFMs.py": "/usr/local/bin/seperatePFMs.py", "seperatePFMsAndCheckActivity.py": "/usr/local/bin/seperatePFMsAndCheckActivity.py", "Makefile": "/usr/local/bin/Makefile", "shiftBed": "/usr/local/bin/shiftBed", "annotateBed": "/usr/local/bin/annotateBed", "bamToBed": "/usr/local/bin/bamToBed", "bamToFastq": "/usr/local/bin/bamToFastq", "bed12ToBed6": "/usr/local/bin/bed12ToBed6", "bedToBam": "/usr/local/bin/bedToBam", "bedToIgv": "/usr/local/bin/bedToIgv", "bedpeToBam": "/usr/local/bin/bedpeToBam", "bedtools": "/usr/local/bin/bedtools", "closestBed": "/usr/local/bin/closestBed", "clusterBed": "/usr/local/bin/clusterBed", "complementBed": "/usr/local/bin/complementBed", "coverageBed": "/usr/local/bin/coverageBed", "expandCols": "/usr/local/bin/expandCols", "fastaFromBed": "/usr/local/bin/fastaFromBed", "flankBed": "/usr/local/bin/flankBed", "genomeCoverageBed": "/usr/local/bin/genomeCoverageBed", "getOverlap": "/usr/local/bin/getOverlap", "groupBy": "/usr/local/bin/groupBy", "intersectBed": "/usr/local/bin/intersectBed", "linksBed": "/usr/local/bin/linksBed", "mapBed": "/usr/local/bin/mapBed", "maskFastaFromBed": "/usr/local/bin/maskFastaFromBed", "mergeBed": "/usr/local/bin/mergeBed"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/sneep.
singularity registry hpc automated addition for sneep
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/sneep
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/sneep:0.4--py39h7cff6ad_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/sneep/0.4--py39h7cff6ad_0
$ module help quay.io/biocontainers/sneep/0.4--py39h7cff6ad_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### sneep-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### sneep-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### sneep-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### sneep-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### sneep-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### sneep-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### HandleInOutput

```bash
$ singularity exec <container> /usr/local/bin/HandleInOutput
$ podman run --it --rm --entrypoint /usr/local/bin/HandleInOutput   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/HandleInOutput   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### HandleInOutput.cpp

```bash
$ singularity exec <container> /usr/local/bin/HandleInOutput.cpp
$ podman run --it --rm --entrypoint /usr/local/bin/HandleInOutput.cpp   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/HandleInOutput.cpp   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### HandleInOutput.hpp

```bash
$ singularity exec <container> /usr/local/bin/HandleInOutput.hpp
$ podman run --it --rm --entrypoint /usr/local/bin/HandleInOutput.hpp   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/HandleInOutput.hpp   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### Makefile.bak

```bash
$ singularity exec <container> /usr/local/bin/Makefile.bak
$ podman run --it --rm --entrypoint /usr/local/bin/Makefile.bak   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/Makefile.bak   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### Matrix

```bash
$ singularity exec <container> /usr/local/bin/Matrix
$ podman run --it --rm --entrypoint /usr/local/bin/Matrix   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/Matrix   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### Matrix_new.cpp

```bash
$ singularity exec <container> /usr/local/bin/Matrix_new.cpp
$ podman run --it --rm --entrypoint /usr/local/bin/Matrix_new.cpp   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/Matrix_new.cpp   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### Matrix_new.hpp

```bash
$ singularity exec <container> /usr/local/bin/Matrix_new.hpp
$ podman run --it --rm --entrypoint /usr/local/bin/Matrix_new.hpp   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/Matrix_new.hpp   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### callBashCommand

```bash
$ singularity exec <container> /usr/local/bin/callBashCommand
$ podman run --it --rm --entrypoint /usr/local/bin/callBashCommand   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/callBashCommand   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### callBashCommand.cpp

```bash
$ singularity exec <container> /usr/local/bin/callBashCommand.cpp
$ podman run --it --rm --entrypoint /usr/local/bin/callBashCommand.cpp   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/callBashCommand.cpp   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### callBashCommand.hpp

```bash
$ singularity exec <container> /usr/local/bin/callBashCommand.hpp
$ podman run --it --rm --entrypoint /usr/local/bin/callBashCommand.hpp   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/callBashCommand.hpp   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### differentialBindingAffinity_multipleSNPs

```bash
$ singularity exec <container> /usr/local/bin/differentialBindingAffinity_multipleSNPs
$ podman run --it --rm --entrypoint /usr/local/bin/differentialBindingAffinity_multipleSNPs   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/differentialBindingAffinity_multipleSNPs   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### differentialBindingAffinity_multipleSNPs.cpp

```bash
$ singularity exec <container> /usr/local/bin/differentialBindingAffinity_multipleSNPs.cpp
$ podman run --it --rm --entrypoint /usr/local/bin/differentialBindingAffinity_multipleSNPs.cpp   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/differentialBindingAffinity_multipleSNPs.cpp   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### estimateScalePerMotif.sh

```bash
$ singularity exec <container> /usr/local/bin/estimateScalePerMotif.sh
$ podman run --it --rm --entrypoint /usr/local/bin/estimateScalePerMotif.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/estimateScalePerMotif.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### findZerosEachMotif.py

```bash
$ singularity exec <container> /usr/local/bin/findZerosEachMotif.py
$ podman run --it --rm --entrypoint /usr/local/bin/findZerosEachMotif.py   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/findZerosEachMotif.py   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### histogram.R

```bash
$ singularity exec <container> /usr/local/bin/histogram.R
$ podman run --it --rm --entrypoint /usr/local/bin/histogram.R   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/histogram.R   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### pvalue

```bash
$ singularity exec <container> /usr/local/bin/pvalue
$ podman run --it --rm --entrypoint /usr/local/bin/pvalue   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/pvalue   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### pvalue_copy.cpp

```bash
$ singularity exec <container> /usr/local/bin/pvalue_copy.cpp
$ podman run --it --rm --entrypoint /usr/local/bin/pvalue_copy.cpp   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/pvalue_copy.cpp   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### pvalue_copy.hpp

```bash
$ singularity exec <container> /usr/local/bin/pvalue_copy.hpp
$ podman run --it --rm --entrypoint /usr/local/bin/pvalue_copy.hpp   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/pvalue_copy.hpp   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### randomRsIds_2.0

```bash
$ singularity exec <container> /usr/local/bin/randomRsIds_2.0
$ podman run --it --rm --entrypoint /usr/local/bin/randomRsIds_2.0   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/randomRsIds_2.0   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### sampleRandomRsIDs2.cpp

```bash
$ singularity exec <container> /usr/local/bin/sampleRandomRsIDs2.cpp
$ podman run --it --rm --entrypoint /usr/local/bin/sampleRandomRsIDs2.cpp   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/sampleRandomRsIDs2.cpp   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### sampleRandomRsIDs2.hpp

```bash
$ singularity exec <container> /usr/local/bin/sampleRandomRsIDs2.hpp
$ podman run --it --rm --entrypoint /usr/local/bin/sampleRandomRsIDs2.hpp   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/sampleRandomRsIDs2.hpp   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### seperatePFMs.py

```bash
$ singularity exec <container> /usr/local/bin/seperatePFMs.py
$ podman run --it --rm --entrypoint /usr/local/bin/seperatePFMs.py   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/seperatePFMs.py   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### seperatePFMsAndCheckActivity.py

```bash
$ singularity exec <container> /usr/local/bin/seperatePFMsAndCheckActivity.py
$ podman run --it --rm --entrypoint /usr/local/bin/seperatePFMsAndCheckActivity.py   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/seperatePFMsAndCheckActivity.py   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### Makefile

```bash
$ singularity exec <container> /usr/local/bin/Makefile
$ podman run --it --rm --entrypoint /usr/local/bin/Makefile   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/Makefile   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### shiftBed

```bash
$ singularity exec <container> /usr/local/bin/shiftBed
$ podman run --it --rm --entrypoint /usr/local/bin/shiftBed   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/shiftBed   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### annotateBed

```bash
$ singularity exec <container> /usr/local/bin/annotateBed
$ podman run --it --rm --entrypoint /usr/local/bin/annotateBed   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/annotateBed   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### bamToBed

```bash
$ singularity exec <container> /usr/local/bin/bamToBed
$ podman run --it --rm --entrypoint /usr/local/bin/bamToBed   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/bamToBed   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### bamToFastq

```bash
$ singularity exec <container> /usr/local/bin/bamToFastq
$ podman run --it --rm --entrypoint /usr/local/bin/bamToFastq   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/bamToFastq   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### bed12ToBed6

```bash
$ singularity exec <container> /usr/local/bin/bed12ToBed6
$ podman run --it --rm --entrypoint /usr/local/bin/bed12ToBed6   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/bed12ToBed6   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### bedToBam

```bash
$ singularity exec <container> /usr/local/bin/bedToBam
$ podman run --it --rm --entrypoint /usr/local/bin/bedToBam   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/bedToBam   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### bedToIgv

```bash
$ singularity exec <container> /usr/local/bin/bedToIgv
$ podman run --it --rm --entrypoint /usr/local/bin/bedToIgv   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/bedToIgv   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### bedpeToBam

```bash
$ singularity exec <container> /usr/local/bin/bedpeToBam
$ podman run --it --rm --entrypoint /usr/local/bin/bedpeToBam   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/bedpeToBam   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### bedtools

```bash
$ singularity exec <container> /usr/local/bin/bedtools
$ podman run --it --rm --entrypoint /usr/local/bin/bedtools   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/bedtools   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### closestBed

```bash
$ singularity exec <container> /usr/local/bin/closestBed
$ podman run --it --rm --entrypoint /usr/local/bin/closestBed   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/closestBed   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### clusterBed

```bash
$ singularity exec <container> /usr/local/bin/clusterBed
$ podman run --it --rm --entrypoint /usr/local/bin/clusterBed   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/clusterBed   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### complementBed

```bash
$ singularity exec <container> /usr/local/bin/complementBed
$ podman run --it --rm --entrypoint /usr/local/bin/complementBed   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/complementBed   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### coverageBed

```bash
$ singularity exec <container> /usr/local/bin/coverageBed
$ podman run --it --rm --entrypoint /usr/local/bin/coverageBed   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/coverageBed   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### expandCols

```bash
$ singularity exec <container> /usr/local/bin/expandCols
$ podman run --it --rm --entrypoint /usr/local/bin/expandCols   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/expandCols   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### fastaFromBed

```bash
$ singularity exec <container> /usr/local/bin/fastaFromBed
$ podman run --it --rm --entrypoint /usr/local/bin/fastaFromBed   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/fastaFromBed   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### flankBed

```bash
$ singularity exec <container> /usr/local/bin/flankBed
$ podman run --it --rm --entrypoint /usr/local/bin/flankBed   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/flankBed   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### genomeCoverageBed

```bash
$ singularity exec <container> /usr/local/bin/genomeCoverageBed
$ podman run --it --rm --entrypoint /usr/local/bin/genomeCoverageBed   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/genomeCoverageBed   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### getOverlap

```bash
$ singularity exec <container> /usr/local/bin/getOverlap
$ podman run --it --rm --entrypoint /usr/local/bin/getOverlap   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/getOverlap   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### groupBy

```bash
$ singularity exec <container> /usr/local/bin/groupBy
$ podman run --it --rm --entrypoint /usr/local/bin/groupBy   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/groupBy   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### intersectBed

```bash
$ singularity exec <container> /usr/local/bin/intersectBed
$ podman run --it --rm --entrypoint /usr/local/bin/intersectBed   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/intersectBed   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### linksBed

```bash
$ singularity exec <container> /usr/local/bin/linksBed
$ podman run --it --rm --entrypoint /usr/local/bin/linksBed   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/linksBed   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### mapBed

```bash
$ singularity exec <container> /usr/local/bin/mapBed
$ podman run --it --rm --entrypoint /usr/local/bin/mapBed   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/mapBed   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### maskFastaFromBed

```bash
$ singularity exec <container> /usr/local/bin/maskFastaFromBed
$ podman run --it --rm --entrypoint /usr/local/bin/maskFastaFromBed   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/maskFastaFromBed   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### mergeBed

```bash
$ singularity exec <container> /usr/local/bin/mergeBed
$ podman run --it --rm --entrypoint /usr/local/bin/mergeBed   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/mergeBed   -v ${PWD} -w ${PWD} <container> -c " $@"
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