# NVT OP examples

This repository will contain examples of using [nvtabular](https://github.com/NVIDIA-Merlin/NVTabular) ops to apply preprocessing to your data.

### Ops with examples right now:
1. [Categorify](https://github.com/radekosmulski/nvt_op_examples/blob/main/examples/01_Categorify.ipynb) ([twitter thread](https://twitter.com/radekosmulski/status/1526578320107720705?s=20&t=7BOvRyP-pqvYbyIOO8Z80w))
2. [JoinExternal](https://github.com/radekosmulski/nvt_op_examples/blob/main/examples/02_Join_External.ipynb) ([twitter thread](https://twitter.com/radekosmulski/status/1529115015558537218?s=20&t=7BOvRyP-pqvYbyIOO8Z80w))
3. [HashBucket](https://github.com/radekosmulski/nvt_op_examples/blob/main/examples/03_Hash_Bucket.ipynb) ([twitter thread](https://twitter.com/radekosmulski/status/1531523922713116673?s=20&t=7BOvRyP-pqvYbyIOO8Z80w))
4. [Clip](https://github.com/radekosmulski/nvt_op_examples/blob/main/examples/04_Clip.ipynb) ([twitter thread](https://twitter.com/radekosmulski/status/1534007245368766464?s=20&t=i3s4pww8LhiFA7L3Xpa_PQ))
5. [LogOp](https://github.com/radekosmulski/nvt_op_examples/blob/main/examples/05_LogOp.ipynb) ([twitter thread](https://twitter.com/radekosmulski/status/1534007245368766464?s=20&t=i3s4pww8LhiFA7L3Xpa_PQ))
6. [TargetEncoding](https://github.com/radekosmulski/nvt_op_examples/blob/main/examples/06_Target_Encoding.ipynb) ([twitter thread](https://twitter.com/radekosmulski/status/1536725232823640065?s=20&t=1yiU0_5atln40fD6Z8r9FQ))
7. [Filter](https://github.com/radekosmulski/nvt_op_examples/blob/main/examples/07_Filter.ipynb) ([twitter thread](https://twitter.com/radekosmulski/status/1539080678242803712?s=20&t=C98Rtx212F2G6ZS85YTXHA))
8. [ReduceDtypeSize](https://github.com/radekosmulski/nvt_op_examples/blob/main/examples/08_ReduceDtypeSize.ipynb) ([twitter thread](https://twitter.com/radekosmulski/status/1541617397810876416?s=20&t=C98Rtx212F2G6ZS85YTXHA))
9. [AddMetadata](https://github.com/radekosmulski/nvt_op_examples/blob/main/examples/09_Add_Metadata.ipynb) ([twitter thread](https://twitter.com/radekosmulski/status/1544308474661650432?s=20&t=DFCFJq9zzHCvf0LiBgUihQ))
10. [Bucketize](https://github.com/radekosmulski/nvt_op_examples/blob/main/examples/10_Bucketize.ipynb) ([twitter thread](https://twitter.com/radekosmulski/status/1546988049556721664?s=20&t=HmoUR9Tvab8JI9QMrVw-gg))
11. [DifferenceLag](https://github.com/radekosmulski/nvt_op_examples/blob/main/examples/11_Difference_Lag.ipynb) ([twitter thread](https://twitter.com/radekosmulski/status/1549408766231060481?s=20&t=nYuzwpAp3W2WFWteED4TiA))
12. [FillMissing](https://github.com/radekosmulski/nvt_op_examples/blob/main/examples/12_Fill_Missing.ipynb) ([twitter thread](https://twitter.com/radekosmulski/status/1551925645260857345))
13. [FillMedian](https://github.com/radekosmulski/nvt_op_examples/blob/main/examples/13_Fill_Median.ipynb) ([twitter thread](https://twitter.com/radekosmulski/status/1551925653192249345?s=20&t=hvHzN5tl35SjHJb59c9Eig))
14. [HashedCross](https://github.com/radekosmulski/nvt_op_examples/blob/main/examples/14_Hashed_Cross.ipynb) ([twitter thread](https://twitter.com/radekosmulski/status/1554438012183793665))
15. [Rename](https://github.com/radekosmulski/nvt_op_examples/blob/main/examples/15_Rename.ipynb) ([twitter thread](https://twitter.com/radekosmulski/status/1556906452316344320))
16. [LambdaOp](https://github.com/radekosmulski/nvt_op_examples/blob/main/examples/16_LambdaOp.ipynb)

nvtabular to me is the toolset of the future. It
* abstracts away your hardware (you can process your data on equipment with varying amount of CPU and GPU RAM, you can read your data from various sources)
* speeds up the processing pipeline (GPUs 🔥🔥🔥)
* has a lot of functionality expertly coded to include best practices (some of the ops are really powerful and unlike anything you will find in other libraries)

This repository will document my journey as I learn nvtabular.

## Running the examples

1. Have docker installed (see "Getting started with docker below")
2. From the root of the repository, run `./start_docker_container`.
3. Navigate to `http://localhost:8888` in your browser.

## Getting started with docker

Whether we like it or not, docker is becoming a big piece of data science work. My history of using docker is riddled with suffering, but with time there are actually aspects of docker that I am starting to enjoy.

If you follow along with the work in this repository, you will get up to speed with using docker the way I feel it can be used for cutting edge data science work.

Below are instructions to get started.

1. [Install docker](https://docs.docker.com/get-docker/). (I use [docker on ubuntu server](https://docs.docker.com/engine/install/ubuntu/) and windows subsystem for linux, native GPU support is really nice!)
    * you will have to [install nvidia-container-toolkit](https://github.com/NVIDIA/nvidia-docker/issues/1243#issuecomment-615170541), depending on your OS you might have to go [to the source](https://github.com/NVIDIA/nvidia-docker/issues/1243#issuecomment-615170541)
3. You might want to be able to use docker [as a non-root user](https://docs.docker.com/engine/install/linux-postinstall/). Do note: this comes with security risks.
4. The [docker tutorial](https://docs.docker.com/get-started/) is exquisite. It only tells you a part of the story thought, but the part it tells you it tells really well.
5. Here are the missing pieces
    * You can [create an image from a running container](https://twitter.com/radekosmulski/status/1524915499506839553?s=20&t=oh9b4X-2xFYLxDL39V10aA).
    * You can [start a stopped container](https://twitter.com/radekosmulski/status/1524938153567858688?s=20&t=oh9b4X-2xFYLxDL39V10aA).
6. Equipped with all this information, the only other missing piece of the puzzle is the command to start a docker container. The `start_docker_container` in this repository contains the most commonly required crucial bits.

## Misc

* [Understanding `>>` in Python](https://twitter.com/radekosmulski/status/1514619524657549312?s=20&t=TWs1pW7H-aZleHcjel_znA)
* [A closer look at `>>`](https://twitter.com/radekosmulski/status/1523517199448608769?s=20&t=TWs1pW7H-aZleHcjel_znA)
