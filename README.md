# NeAR: Coupled Neural Asset–Renderer Stack

Neural asset authoring and neural rendering have emerged as largely disjoint threads: one generates digital assets using neural networks for traditional graphics pipelines, while the other develops neural renderers that map conventional assets to images. However, the joint design of the asset representation and renderer remains largely unexplored. We argue that coupling them can unlock an end-to-end learnable graphics stack with benefits in fidelity, consistency, and efficiency.

## Overview

**On the asset side:** We build on Trellis-style Structured 3D Latents and introduce a lighting-homogenized neural asset: from a casually lit input, a rectified-flow backbone predicts a Lighting-Homogenized SLAT (LH-SLAT) that encodes geometry and intrinsic material cues in a compact, view-agnostic latent.

**On the renderer side:** We design a lighting-aware neural renderer that uses this neural asset, along with explicit view embeddings and HDR environment maps, to produce lighting-aware renderings in realtime.

## Key Features

- **Coupled Design:** Joint optimization of neural asset representation and neural renderer
- **Four Tasks:** (1) G-buffer–based forward rendering, (2) random-lit single-image reconstruction, (3) unknown-lit single-image relighting, and (4) novel-view relighting
- **Real-time Rendering:** Fast feed-forward Rendering without per-object optimization
- **High Quality:** Surpasses state-of-the-art baselines in quantitative metrics and perceptual quality

> For a detailed visualization, see the [project page](https://near.github.io/)

We welcome your attention, use, and feedback!
