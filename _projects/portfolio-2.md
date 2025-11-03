---
title: "Text-to-3D Flower Model"
excerpt: "Benchmarked Two Texto-to-3D Pipelines in Multi-View Diffusion Mesh Generation<br/><img src='/images/flowers_gif.gif'>"
collection: projects
---

Developed and evaluated two distinct pipelines for generating 3D meshes (of a flower subject) from a text prompt, aiming to recreate photogrammetry implementations inspired by then state-of-the-art models like InstantMesh. Pipeline 1 utilized a Stable Virtual Camera video followed by COLMAP and Open3D for mesh cleaning, resulting in a mesh with greater structural complexity and better noise properties (higher floral surface area variance) at the expense of surface smoothness. Pipeline 2 used Era3D's direct mesh output, achieving significantly better surface smoothness (measured via lower Laplacian Smoothness and higher Mean Normal Dot Product) and greater structural similarity to the input image. Ultimately, while both approaches struggled with structural integrity (watertightness), Pipeline 1 achieved complex, organic shapes while Pipeline 2 achieved smooth, structurally faithful reproductions.

[Report Link](https://drive.google.com/file/d/1y1YMAxlVwLDS-T8N-4XGHt_vJJ23JSWp/view?usp=sharing)
