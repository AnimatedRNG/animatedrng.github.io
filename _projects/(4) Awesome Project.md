---
name: Screen-Space Point Cloud Surface Reconstruction
tools: [WebGL, JavaScript]
image: /portfolYOU/assets/cesium_church_ao.png
description: A screen-space point cloud processing pipeline for handling occlusion and inpainting, contributed to the Cesium Project
---

# Screen-Space Point Cloud Surface Reconstruction

I wrote an implementation of [this point cloud surface reconstruction algorithm](https://pdfs.semanticscholar.org/7841/328958c3f52a50e030e15b3df2635acf6f6d.pdf) while I was an intern at Analytical Graphics Inc. on the Cesium team. I was able to make a few improvements on the original paper, including reducing the distracting edge dilation, stenciling the region growing passes, and coming up with a better shading model. Our WebGL implementation could run at interactive frame rates on integrated GPUs.

The ambient occlusion term was particularly useful for visualizing seemingly-invisible details in the point cloud, like creases in a painting. See the demo below.

<video muted autoplay controls>
    <source src="/portfolYOU/assets/demo_2.mp4" type="video/mp4">
</video>
