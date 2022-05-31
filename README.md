# NVT OP examples

This repository will contain examples of using [nvtabular](https://github.com/NVIDIA-Merlin/NVTabular) ops to do cool things with your data.

### Ops with examples right now:
1. [Categorify](https://github.com/radekosmulski/nvt_op_examples/blob/main/examples/01_Categorify.ipynb)

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
2. You might want to be able to use docker [as a non-root user](https://docs.docker.com/engine/install/linux-postinstall/). Do note: this comes with security risks.
3. The [docker tutorial](https://docs.docker.com/get-started/) is exquisite. It only tells you a part of the story thought, but the part it tells you it tells really well.
4. Here are the missing pieces
    * You can [create an image from a running container](https://twitter.com/radekosmulski/status/1524915499506839553?s=20&t=oh9b4X-2xFYLxDL39V10aA).
    * You can [start a stopped container](https://twitter.com/radekosmulski/status/1524938153567858688?s=20&t=oh9b4X-2xFYLxDL39V10aA).
5. Equipped with all this information, the only other missing piece of the puzzle is the command to start a docker container. The `start_docker_container` in this repository contains the most commonly required crucial bits.

## Misc

* [Understanding `>>` in Python](https://twitter.com/radekosmulski/status/1514619524657549312?s=20&t=TWs1pW7H-aZleHcjel_znA)
* [A closer look at `>>`](https://twitter.com/radekosmulski/status/1523517199448608769?s=20&t=TWs1pW7H-aZleHcjel_znA)
