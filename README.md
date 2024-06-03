
# Streaming Video Diffusion: Online Video Editing with Diffusion Models
[![Arxiv](https://img.shields.io/badge/Arxiv-b31b1b.svg)](https://arxiv.org/abs/2405.19726) 

We present a novel task called online video editing, which is designed to edit streaming frames while maintaining temporal consistency. Unlike existing offline video editing assuming all frames are pre-established and accessible, online video editing is tailored to real-life applications such as live streaming and online chat, requiring (1) fast continual step inference, (2) long-term temporal modeling, and (3) zero-shot video editing capability. To solve these issues, we propose Streaming Video Diffusion (SVDiff), which incorporates the compact spatial-aware temporal recurrence into off-the-shelf Stable Diffusion and is trained with the segment-level scheme on large-scale long videos. This simple yet effective setup allows us to obtain a single model that is capable of executing a broad range of videos and editing each streaming frame with temporal coherence. Our experiments indicate that our model can edit long, high-quality videos with remarkable results, achieving a real-time inference speed of 15.2 FPS at a resolution of 512x512.

## Gallery

<table style="width:100%; text-align:center;">
<tr>
  <td align="center">Input Video</td>
  <td align="center">Output video</td>
  <td align="center">Input image</td>
  <td align="center">Output video</td>
</tr>
<tr>
  <td align="center"><img src="visual_editing/car/car-roundabout.mp4" width="100%"></td>
  <td align="center"><img src="visual_editing/car/car-roundabout-mountain.mp4" width="100%"></td>
  <td align="center"><img src="visual_editing/car/car-roundabout-jeep-oil.mp4" width="100%"></td>
  <td align="center"><img src="visual_editing/car/car-roundabout-fire.mp4" width="100%"></td>
</tr>
</table>
