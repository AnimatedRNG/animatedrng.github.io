---
name: rusty-raisr
tools: [Rust, OpenGL, GPGPU]
image: https://raw.githubusercontent.com/AnimatedRNG/rusty-raisr/master/img/comparison.png
description: OpenGL Compute shader implementation of Google's RAISR algorithm
---

# rusty-raisr

`rusty-raisr` is an implementation of Google's RAISR algorithm, implemented in OpenGL Compute shaders using the `glium` framework in Rust. I presented an [overview of the algorithm](/portfolYOU/assets/RAISR.pdf) while I was an intern at Nvidia.

![preview](/portfolYOU/assets/comparison.png)

(from left to right -- nearest neighbor 2x, bicubic upscaling 2x, and RAISR 2x)

Our [6.819/6.869 final project paper](/portfolYOU/assets/RAISR_kaza.pdf) describes the RAISR algorithm, some improvements that I made, and a comparison to SRGAN. Several optimizations significantly improved performance since then -- it now takes roughly 8 ms to upscale a 1080p image to 4K on a GTX 1070 (GP104). See the slides below.

[Github](https://github.com/animatedrng/rusty-raisr)


<iframe src="https://docs.google.com/presentation/d/e/2PACX-1vT3Ae5n0euwDOmdEUwN4zAVzEHQXU5Tev5YfkDOwueNIp3btNuOv81eItM1jX-xVAEyJuFWZOruWGoj/embed?start=false&loop=false&delayms=3000" frameborder="0" width="480" height="299" allowfullscreen="true" mozallowfullscreen="true" webkitallowfullscreen="true"></iframe>
