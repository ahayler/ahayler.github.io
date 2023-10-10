---
layout: page
permalink: publications/s4c/
date: 2023_10_16 # determines sorting just take the date of the first publication as YYYY_MM_DD
image: assets/teaser.png
image_mouseover: assets/header_video.mp4

title: "S4C: Self-Supervised Semantic Scene Completion with Neural Fields"
venue: 3DV, 2024
authors:
  - name: adrianhayler
    affiliations: "1"
  - name: felixwimbauer
    affiliations: "1,2"
  - name: christianrupprecht
    affiliations: "3"
  - name: danielcremers
    affiliations: "1,2,3"
affiliations:
  - name: tum
    length: short
  - name: mcml
    length: long
  - name: oxford
    length: long

description: "A differentiable nonlinear least squares framework to account for uncertainty in relative pose estimation from feature correspondences regardless of the feature extraction algorithm of choice."

links:
    - name: Project Page
      link: publications/s4c/
    - name: Paper
      link: https://arxiv.org/abs/2305.09527 # change this as soon as the paper is uploaded
      style: "bi bi-file-earmark-richtext"
    - name: Code
      link: # after clean up
      style: "bi bi-github"
    - name: Video
      link: # after video was created
      style: "bi bi-youtube"

citation: # insert citation when is published

acknowledgements: # don't know

<video width="100%" autoplay muted loop>
  <source src="./assets/header_video.mp4" type="video/mp4">
Your browser does not support the video tag.
</video>

***SSC Predictions on KITTI-360.** Input image (top), color-coded voxel grids (bottom). The voxels indicate if a certain region is occupied or not, the color indicates the class. A color to class map can be found in [TODO]. We compare the predictions of our S4C against the ground truth and other fully supervised state-of-the-art methods. The current method is displayed in the bottom left corner.*

# Abstract

Our proposed method can reconstruct a scene from a single image and only relies on videos and pseudo segmentation ground truth generated from off-the-shelf image segmentation network during training.
Unlike existing methods, which use discrete voxel grids, we represent scenes as implicit *semantic fields*.
This formulation allows querying any point within the camera frustum for occupancy and semantic class.
Our architecture is trained through rendering-based self-supervised losses.
Nonetheless, our method achieves performance close to fully supervised state-of-the-art methods.
Additionally, our method demonstrates strong generalization capabilities and can synthesize accurate segmentation maps for far away viewpoints.

---