# RetroPath2-cwl -- RetroPath2.0 IBISBA Node

[![Build Status](https://travis-ci.org/ibisba/RetroPath2-cwl.svg?branch=master)](https://travis-ci.org/ibisba/RetroPath2-cwl)
[![](https://images.microbadger.com/badges/version/ibisba/retropath2.svg)](https://hub.docker.com/r/ibisba/retropath2 "ibisba/retropath2")
[![](https://images.microbadger.com/badges/image/ibisba/retropath2.svg)](https://microbadger.com/images/ibisba/retropath2 "Get your own image badge on microbadger.com")

* Docker image: [ibisba/retropath2](https://hub.docker.com/r/ibisba/retropath2)
* Base images: [ibsiba/knime-workflow-base](https://hub.docker.com/r/ibisba/knime-workflow-base/)
* Source: [Dockerfile](https://github.com/ibisba/RetroPath2-cwl/blob/master/Dockerfile), [RetroPath2.0](https://www.myexperiment.org/workflows/4987.html)

RetroPath2.0 builds a reaction network from a set of source compounds to a set of sink compounds.

## Quick start

If you have `cwl-runner` installed, you can run RetroPath2.0 on the [carotene](examples/carotene) example:

```
cwl-runner --no-match-user workflows/rp2-to-rp2path-job.yaml
```

The easiest way to get started with your own computations is to use [`rp2-to-rp2path-job.yaml`](workflows/rp2-to-rp2path-job.yaml) as a template for your own jobs.

## Contributing

To build the docker image yourself, use

```
docker build -t ibisba/retropath2 .
```

### How to cite RetroPath2.0?
Please cite:

Delépine B, Duigou T, Carbonell P, Faulon JL. RetroPath2.0: A retrosynthesis workflow for metabolic engineers. Metabolic Engineering, 45: 158-170, 2018. DOI: https://doi.org/10.1016/j.ymben.2017.12.002

## License

Different licenses apply to files added by different Docker layers:

* ibisba/RetroPath2-cwl [Dockerfile](https://github.com/ibisba/RetroPath2-cwl/blob/master/Dockerfile): [Apache License, version 2.0](http://www.apache.org/licenses/LICENSE-2.0)
* RetroPath2.0 (`/payload/workflow` in the image): [CC BY-NC-SA 3.0](http://creativecommons.org/licenses/by-nc-sa/3.0/)
