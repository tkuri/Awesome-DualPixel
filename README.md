<!--A curated list of resources for Image and Video Deblurring-->
<!-- PROJECT LOGO -->
<p align="center">
  <h3 align="center">Dual Pixel</h3>
</p>

## Table of contents

- [DualPixel](#dualpixel)
- [Dateset](#dataset)

## Dual Pixel
|Year|Pub|Paper|App|Repo|
|:---:|:---:|:---:|:---:|:---:|
|2018|SIGGRAPH|[Synthetic Depth-of-Field with a Single-Camera Mobile Phone](https://arxiv.org/abs/1806.04171)|Depth / Segmenation / Synthetic DoF||
|2019|CVPR|[Reflection Removal Using a Dual-Pixel Sensor](https://abhijithpunnappurath.github.io/dprr.html)|Reflection Removal|[Code](https://github.com/abhijithpunnappurath/dprr)|
|2019|ICCV|[Learning Single Camera Depth Estimation using Dual-Pixels](https://arxiv.org/abs/1904.05822)|Depth|[Code & Dataset](https://github.com/google-research/google-research/tree/master/dual_pixels)|
|2020|ICCP|[Modeling Defocus-Disparity in Dual-Pixel Sensors](https://abhijithpunnappurath.github.io/ICCP2020.pdf)|Depth|[Code & Dataset](https://github.com/abhijithpunnappurath/dual-pixel-defocus-disparity)|
|2020|ECCV|[Du2Net: Learning Depth Estimation from Dual-Cameras and Dual-Pixels](https://augmentedperception.github.io/du2net/)|Depth (w/Stereo)||
|2020|ECCV|[Defocus Deblurring Using Dual-Pixel Data](https://www.eecs.yorku.ca/~abuolaim/eccv_2020_dp_defocus_deblurring/)|Deblur|[Code & Dataset](https://github.com/Abdullah-Abuolaim/defocus-deblurring-dual-pixel)|
|2021|CVPR|[Dual Pixel Exploration: Simultaneous Depth Estimation and Image Restoration](https://openaccess.thecvf.com/content/CVPR2021/html/Pan_Dual_Pixel_Exploration_Simultaneous_Depth_Estimation_and_Image_Restoration_CVPR_2021_paper.html)|Depth / Deblur|[Code & Dataset](https://github.com/panpanfei/Dual-Pixel-Exploration-Simultaneous-Depth-Estimation-and-Image-Restoration)|
|2021|CVPRW|[NTIRE 2021 Challenge for Defocus Deblurring Using Dual-pixel Images: Methods and Results](https://openaccess.thecvf.com/content/CVPR2021W/NTIRE/html/Abuolaim_NTIRE_2021_Challenge_for_Defocus_Deblurring_Using_Dual-Pixel_Images_Methods_CVPRW_2021_paper.html)|Deblur||
|2021|CVPRW|[ATTSF Attention! Stay Focus!](https://arxiv.org/abs/2104.07925)|Deblur|[Code](https://github.com/tuvovan/ATTSF)|
|2021|ICCV|[Defocus Map Estimation and Deblurring From a Single Dual-Pixel Image](https://openaccess.thecvf.com/content/ICCV2021/html/Xin_Defocus_Map_Estimation_and_Deblurring_From_a_Single_Dual-Pixel_Image_ICCV_2021_paper.html)|Deblur /  Defocus Map||
|2021|ICCV|[Learning to Reduce Defocus Blur by Realistically Modeling Dual-Pixel Data](https://openaccess.thecvf.com/content/ICCV2021/html/Abuolaim_Learning_To_Reduce_Defocus_Blur_by_Realistically_Modeling_Dual-Pixel_Data_ICCV_2021_paper.html)|Deblur|[Code & Dataset](https://github.com/Abdullah-Abuolaim/recurrent-defocus-deblurring-synth-dual-pixel)|
|2021|Arxiv|[Facial Depth and Normal Estimation using Single Dual-Pixel Camera](https://arxiv.org/abs/2111.12928)|Depth / Surface Normal / Anti-spoofing / Relighting||

## Dataset
|Year|Pub|Paper|Detail|
|:---:|:---:|:---:|:---:|
|2019|ICCV|[Learning Single Camera Depth Estimation using Dual-Pixels](https://github.com/google-research/google-research/tree/master/dual_pixels)|Train:2506, Test:684, Res:1512x2016(DP), 16bit png, DP Raw / Depth|
|2020|ICCP|[Modeling Defocus-Disparity in Dual-Pixel Sensors](https://github.com/abhijithpunnappurath/dual-pixel-defocus-disparity)|Num:100, Res:5180x2940, RGB 8bit jpg / 16bit tif Depth, DP LR / Depth|
|2020|ECCV|[Defocus Deblurring Using Dual-Pixel Data](https://github.com/Abdullah-Abuolaim/defocus-deblurring-dual-pixel)|Num:500, Res:1680x1120, 16bit, Used for NTIRE 2021 Challenge (CVPRW)|
|2021|CVPR|[Dual Pixel Exploration: Simultaneous Depth Estimation and Image Restoration](https://github.com/panpanfei/Dual-Pixel-Exploration-Simultaneous-Depth-Estimation-and-Image-Restoration)|DP Simulator from [NYUD Dataset](https://cs.nyu.edu/~silberman/datasets/nyu_depth_v2.html)|
|2021|ICCV|[Learning to Reduce Defocus Blur by Realistically Modeling Dual-Pixel Data](https://github.com/Abdullah-Abuolaim/recurrent-defocus-deblurring-synth-dual-pixel)|DP Simulator form [SYNTHIA-SF dataset](https://synthia-dataset.net/downloads/)|
