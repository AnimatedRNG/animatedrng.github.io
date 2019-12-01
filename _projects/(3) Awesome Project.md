---
name: Differentiable SDF Rendering
tools: [PyTorch, Halide, CUDA]
description: Differentiable Volume Rendering using Signed Distance Functions
---

# Differentiable SDF Rendering (MEng Thesis)

Gradient-based methods are often used in a computer graphics and
computer vision context to solve inverse rendering problems. These methods can be used to infer camera parameters, material properties, and even object pose and geometry from 2D images.

One of the challenges that faces differentiable rendering systems is handling visibility terms in the rendering equation, which are not continuous on object boundaries. We present a renderer that solves this problem by introducing a form of visibility that is not discontinuous, and thus can be
differentiated. This “soft visibility” is inspired by volumetric
rendering, and is facilitated by our decision to represent geometry within the scene as a signed distance function. We also present methods for performing gradient descent upon distance fields while preserving Lipschitz continuity. Unlike most differentiable mesh-based renderers, our renderer can optimize between geometry of different homeomorphism classes in a variety of image-based shape fitting tasks.

Read more about our results [here](/portfolYOU/assets/thesis.pdf).
