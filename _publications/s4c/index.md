---
layout: page
permalink: publications/s4c/
date: 2023_05_30 # determines sorting just take the date of the first publication as YYYY_MM_DD
image: assets/teaser.png
image_mouseover: assets/header_video.mp4

title: "S4C: Self-Supervised Semantic Scene Completion with Neural Fields"
venue: ArXiv, 2023
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

description: "S4C is the first self-supervised approach to the Sematic Scence Completion task. It achives close to state-of-the-art performance on the KITTI-360 SSCBench dataset."

links:
    - name: Project Page
      link: publications/s4c/
    - name: Paper
      link: https://arxiv.org/abs/2305.09527 # change this as soon as the paper is uploaded
      style: "bi bi-file-earmark-richtext"
    # - name: Code
    #  link: # after clean up
    #   style: "bi bi-github"
    # - name: Video
    #   link: # after video was created
    #   style: "bi bi-youtube"

# citation: # insert citation when is published

# acknowledgements: # don't know

# citation: '@article{muhle2023dnls_covs,
#   title={Learning Correspondence Uncertainty via Differentiable Nonlinear Least Squares},
#   author={Dominik Muhle and Lukas Koestler and Krishna Murthy Jatavallabhula and Daniel Cremers},
#   journal={IEEE Conference on Computer Vision and Pattern Recognition (CVPR)},
#   year={2023},
# }'

# acknowledgements: 'This work was supported by the ERC Advanced Grant SIMULACRON, by the Munich Center for Machine Learning and by the EPSRC Programme Grant VisualAI EP/T028572/1.'
# # citation: "@{ASDF}"
---

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
