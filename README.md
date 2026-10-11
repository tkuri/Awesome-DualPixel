<!-- A curated list of research on Dual-Pixel Imaging -->
<!-- PROJECT LOGO -->
<p align="center">
  <h3 align="center">Dual Pixel</h3>
</p>

A curated list of Dual-Pixel (DP) imaging research: depth/disparity, defocus deblurring, autofocus, simulation, and computational photography.

Last literature review: **2026-10-11**. See [research notes](RESEARCH_NOTES.md) for verification sources and limitations.

## Table of contents

- [Scope](#scope)
- [Dual Pixel](#dual-pixel)
- [Restoration methods using DP data](#restoration-methods-using-dp-data)
- [Related Quad-Pixel research](#related-quad-pixel-research)
- [Dataset](#dataset)

## Scope

New entries prioritize peer-reviewed work at established vision, computational photography, graphics, robotics, and signal-processing conferences, and archival journals comparable to those already represented here. Acceptance/publication must be confirmed by proceedings, publisher metadata, or an author-maintained publication/project page. Preprints without confirmed acceptance are excluded.

The main table covers DP measurements and DP image formation, alongside the existing sensor papers. General restoration methods with explicit DP training or DP-pair experiments and Quad-Pixel (QP/QPD) extensions are listed separately. Merely using the single-image portion of DPDD or conventional stereo does not qualify. `Year` is the conference or journal volume year, rather than the first preprint date. Journal extensions are listed separately. Empty repository cells mean no official release was verified; placeholders and partial releases are labeled.

## Dual Pixel

|Year|Pub|Paper|App|Repo|
|:---:|:---:|:---:|:---:|:---:|
|2018|SIGGRAPH|[Synthetic Depth-of-Field with a Single-Camera Mobile Phone](https://arxiv.org/abs/1806.04171)|Depth / Segmentation / Synthetic DoF||
|2019|CVPR|[Reflection Removal Using a Dual-Pixel Sensor](https://abhijithpunnappurath.github.io/dprr.html)|Reflection Removal|[Code](https://github.com/abhijithpunnappurath/dprr)|
|2019|ICCV|[Learning Single Camera Depth Estimation using Dual-Pixels](https://arxiv.org/abs/1904.05822)|Depth|[Code & Dataset](https://github.com/google-research/google-research/tree/master/dual_pixels)|
|2020|ICCP|[Modeling Defocus-Disparity in Dual-Pixel Sensors](https://abhijithpunnappurath.github.io/ICCP2020.pdf)|Depth|[Code & Dataset](https://github.com/abhijithpunnappurath/dual-pixel-defocus-disparity)|
|2020|CVPR|[Learning to Autofocus](https://learntoautofocus-google.github.io/)|Autofocus|[Dataset](https://learntoautofocus-google.github.io/)|
|2020|ECCV|[Du2Net: Learning Depth Estimation from Dual-Cameras and Dual-Pixels](https://augmentedperception.github.io/du2net/)|Disparity (w/Stereo)||
|2020|ECCV|[Defocus Deblurring Using Dual-Pixel Data](https://www.ecva.net/papers/eccv_2020/papers_ECCV/html/1003_ECCV_2020_paper.php)|Deblur|[Code & Dataset](https://github.com/Abdullah-Abuolaim/defocus-deblurring-dual-pixel)|
|2021|CVPR|[Dual Pixel Exploration: Simultaneous Depth Estimation and Image Restoration](https://openaccess.thecvf.com/content/CVPR2021/html/Pan_Dual_Pixel_Exploration_Simultaneous_Depth_Estimation_and_Image_Restoration_CVPR_2021_paper.html)|Depth / Deblur|[Code & Dataset](https://github.com/panpanfei/Dual-Pixel-Exploration-Simultaneous-Depth-Estimation-and-Image-Restoration)|
|2021|CVPRW|[NTIRE 2021 Challenge for Defocus Deblurring Using Dual-pixel Images: Methods and Results](https://openaccess.thecvf.com/content/CVPR2021W/NTIRE/html/Abuolaim_NTIRE_2021_Challenge_for_Defocus_Deblurring_Using_Dual-Pixel_Images_Methods_CVPRW_2021_paper.html)|Deblur||
|2021|CVPRW|[ATTSF Attention! Stay Focus!](https://arxiv.org/abs/2104.07925)|Deblur|[Code](https://github.com/tuvovan/ATTSF)|
|2021|ICCV|[Defocus Map Estimation and Deblurring From a Single Dual-Pixel Image](https://openaccess.thecvf.com/content/ICCV2021/html/Xin_Defocus_Map_Estimation_and_Deblurring_From_a_Single_Dual-Pixel_Image_ICCV_2021_paper.html)|Deblur /  Defocus Map|[Code & Dataset](https://github.com/cmu-ci-lab/dual_pixel_defocus_estimation_deblurring)|
|2021|ICCV|[Learning to Reduce Defocus Blur by Realistically Modeling Dual-Pixel Data](https://openaccess.thecvf.com/content/ICCV2021/html/Abuolaim_Learning_To_Reduce_Defocus_Blur_by_Realistically_Modeling_Dual-Pixel_Data_ICCV_2021_paper.html)|Deblur|[Code & Dataset](https://github.com/Abdullah-Abuolaim/recurrent-defocus-deblurring-synth-dual-pixel)|
|2021|Hot Chips|[World Largest Mobile Image Sensor with All Directional Phase Detection Auto Focus Function](https://ieeexplore.ieee.org/document/9567122)|Sensor / Autofocus||
|2021|ICTC|[Disparity probability volume guided defocus deblurring using dual pixel data](https://ieeexplore.ieee.org/document/9621024)|Deblur||
|2021|Journal of Electronic Imaging|[Defocus deblurring: a designed deep model based on CNN](https://www.spiedigitallibrary.org/journals/journal-of-electronic-imaging/volume-30/issue-6/063013/Defocus-deblurring-a-designed-deep-model-based-on-CNN/10.1117/1.JEI.30.6.063013.short?SSO=1)|Deblur||
|2021|VLSI Symposium|[All-Directional Dual Pixel Auto Focus Technology in CMOS Image Sensors](https://ieeexplore.ieee.org/document/9492472)|Circuits / Autofocus||
|2021|TIFS|[Single-Shot Face Anti-Spoofing for Dual Pixel Camera](https://doi.org/10.1109/TIFS.2020.3035879)|Depth / Anti-spoofing||
|2022|WACV|[Improving Single-Image Defocus Deblurring: How Dual-Pixel Images Help Through Multi-Task Learning](https://arxiv.org/abs/2108.05251)|Deblur|[Code & Dataset](https://github.com/Abdullah-Abuolaim/multi-task-defocus-deblurring-dual-pixel-nimat)|
|2022|ISSCC|[A 1/1.57-inch 50Mpixel CMOS Image Sensor With 1.0μm All-Directional Dual Pixel by 0.5μm-Pitch Full-Depth Deep-Trench Isolation Technology](https://ieeexplore.ieee.org/document/9731567)|Circuits||
|2022|ECCV|[Facial Depth and Normal Estimation using Single Dual-Pixel Camera](https://arxiv.org/abs/2111.12928)|Depth / Surface Normal / Anti-spoofing / Relighting|[Code & Dataset](https://github.com/MinJunKang/DualPixelFace)|
|2022|IEEE/CAA JAS|[BaMBNet: A Blur-Aware Multi-Branch Network for Dual-Pixel Defocus Deblurring](https://www.ieee-jas.net/en/article/doi/10.1109/JAS.2022.105563)|Deblur / Defocus Map|[Code](https://github.com/junjun-jiang/BaMBNet)|
|2022|ICME|[Dynamic Multi-Scale Network for Dual-Pixel Images Defocus Deblurring with Transformer](https://doi.org/10.1109/ICME52920.2022.9859631)|Deblur||
|2022|BMVC|[Dual-Pixel Raindrop Removal](https://arxiv.org/abs/2210.13321)|Raindrop Removal|[Code & Dataset](https://github.com/Yizhou-Li-CV/DPRRN)|
|2023|CVPR|[K3DN: Disparity-Aware Kernel Estimation for Dual-Pixel Defocus Deblurring](https://openaccess.thecvf.com/content/CVPR2023/html/Yang_K3DN_Disparity-Aware_Kernel_Estimation_for_Dual-Pixel_Defocus_Deblurring_CVPR_2023_paper.html)|Deblur||
|2023|CVPR|[Spatio-Focal Bidirectional Disparity Estimation From a Dual-Pixel Image](https://openaccess.thecvf.com/content/CVPR2023/html/Kim_Spatio-Focal_Bidirectional_Disparity_Estimation_From_a_Dual-Pixel_Image_CVPR_2023_paper.html)|Depth / Disparity|[Code](https://github.com/KAIST-VCLAB/dual-pixel-disparity)|
|2023|ICCP|[Learning to Synthesize Photorealistic Dual-pixel Images from RGBD frames](https://ai.sony/publications/Learning-to-Synthesize-Photorealistic-Dual-pixel-Images-from-RGBD-frames/)|Simulator|[Code & Dataset](https://github.com/feiran-l/Neural-Dual-Pixel-Simulator)|
|2023|ICCV|[Exploring Positional Characteristics of Dual-Pixel Data for Camera Autofocus](https://openaccess.thecvf.com/content/ICCV2023/html/Choi_Exploring_Positional_Characteristics_of_Dual-Pixel_Data_for_Camera_Autofocus_ICCV_2023_paper.html)|Autofocus||
|2023|ICASSP|[MRNET: Multi-Refinement Network for Dual-Pixel Images Defocus Deblurring](https://doi.org/10.1109/ICASSP49357.2023.10096428)|Deblur||
|2024|CVPR|[CADS: Passive Snapshot Coded Aperture Dual-Pixel RGB-D Imaging](https://shadowfax11.github.io/cads/)|Depth / Deblur|[Code](https://github.com/shadowfax11/coded-dual-pixels/)|
|2024|CVPR|[LDP: Language-driven Dual-Pixel Image Defocus Deblurring Network](https://openaccess.thecvf.com/content/CVPR2024/html/Yang_LDP_Language-driven_Dual-Pixel_Image_Defocus_Deblurring_Network_CVPR_2024_paper.html)|Deblur|[Code](https://github.com/noxsine/LDP)|
|2024|3DV|[Continuous Cost Aggregation for Dual-Pixel Disparity Extraction](https://arxiv.org/abs/2306.07921)|Depth / Disparity|[Code](https://github.com/SagiMonin/CCA-public)|
|2024|ECCV|[Resolving Scale Ambiguity in Multi-view 3D Reconstruction using Dual-Pixel Sensors](https://www.ecva.net/papers/eccv_2024/papers_ECCV/papers/06658.pdf)|Depth|[Code](https://github.com/kohei-ashida/dp-sfm)|
|2024|ICCP|[Stereo-Knowledge Distillation from dpMV to Dual Pixels for Light Field Video Reconstruction](https://doi.org/10.1109/ICCP61108.2024.10644854)|Disparity / Light Field Video|[Code](https://github.com/Aryan-Garg/dp-LFVR)|
|2024|SIGGRAPH / TOG|[Split-Aperture 2-in-1 Computational Cameras](https://light.princeton.edu/publication/2in1-camera/)|Depth / HDR / Hyperspectral Imaging|[Project & Code links](https://light.princeton.edu/publication/2in1-camera/)|
|2024|TPAMI|[Weakly-Supervised Depth Estimation and Image Deblurring via Dual-Pixel Sensors](https://doi.org/10.1109/TPAMI.2024.3458974)|Depth / Deblur|[Warping component](https://github.com/zwxu064/DiffImageWarpingCUDA)|
|2024|TPAMI|[Dual-Pixel Raindrop Removal](https://doi.org/10.1109/TPAMI.2024.3442955)|Raindrop Removal|[Code & Dataset](https://github.com/Yizhou-Li-CV/DPRRN)|
|2025|WACV|[Revisiting Disparity from Dual-Pixel Images: Physics-Informed Lightweight Depth Estimation](https://openaccess.thecvf.com/content/WACV2025/html/Kurita_Revisiting_Disparity_from_Dual-Pixel_Images_Physics-Informed_Lightweight_Depth_Estimation_WACV_2025_paper.html)|Depth / Disparity|[Code & Dataset](https://github.com/sony/dual-pixel-disparity)|
|2025|Neurocomputing|[Learning dual-pixel alignment for defocus deblurring](https://doi.org/10.1016/j.neucom.2024.128880)|Deblur / Alignment|[Code](https://github.com/liyucs/DPANet)|
|2025|Engineering Applications of Artificial Intelligence|[Parallax-aware dual-view feature enhancement and adaptive detail compensation for dual-pixel defocus deblurring](https://doi.org/10.1016/j.engappai.2024.109612)|Deblur / Alignment||
|2025|MVA|[FMDP: Leveraging a Foundation Model for Dual-Pixel Disparity Estimation](https://doi.org/10.34385/proc.93.O1-1-2)|Depth / Disparity||
|2025|ICCV|[Simulating Dual-Pixel Images From Ray Tracing For Depth Estimation](https://openaccess.thecvf.com/content/ICCV2025/html/He_Simulating_Dual-Pixel_Images_From_Ray_Tracing_For_Depth_Estimation_ICCV_2025_paper.html)|Simulator / Depth|[Code & Dataset](https://github.com/LinYark/Sdirt)|
|2025|ICCV|[Spatially-Varying Autofocus](https://imaging.cs.cmu.edu/svaf/)|Autofocus / Depth / Optical All-in-Focus Imaging|[Project & Code links](https://imaging.cs.cmu.edu/svaf/)|
|2025|IROS|[DiFuse-Net: RGB and Dual-Pixel Depth Estimation using Window Bi-directional Parallax Attention and Cross-modal Transfer Learning](https://arxiv.org/abs/2506.14709)|RGB + DP Depth / DCDP Dataset||
|2025|ACM MM|[Enhanced Dual-Pixel Image Reflection Removal via Gaussian Splatting](https://doi.org/10.1145/3746027.3755094)|Reflection Removal / 3D Gaussian Splatting||
|2025|NeurIPS|[User-Instructed Disparity-aware Defocus Control](https://proceedings.neurips.cc/paper_files/paper/2025/hash/180836fd0a8f164d189d7e244ec8841a-Abstract-Conference.html)|Deblur / Refocus / DoF Control||
|2026|ICASSP|[Freq-DP Net: A Dual-Branch Network for Fence Removal using Dual-Pixel and Fourier Priors](https://arxiv.org/abs/2602.14226)|Fence Removal||
|2026|IJCV|[DCRR++: Unsupervised Reflection Removal and Novel View Synthesis via Dual-Pixel Guided 3D Gaussian Splatting](https://link.springer.com/article/10.1007/s11263-026-02892-2)|Reflection Removal / Novel View Synthesis||
|2026|TPAMI|[DP-SfM: Dual-Pixel Structure-from-Motion without Scale Ambiguity](https://doi.org/10.1109/TPAMI.2026.3690655)|Metric 3D Reconstruction|[Repository (code/data upcoming)](https://github.com/lilika-makabe/dp-sfm-tpami)|
|2026|ECCV (accepted)|[FoundDP: Revisiting Weak Disparity Observability in Dual-Pixel Depth Estimation](https://arxiv.org/abs/2607.01900)|Depth / Foundation Model|[Project (full code/data pending)](https://github.com/EchoLighting/FoundDP)|


## Restoration methods using DP data

These papers use DP pairs for training or evaluate a DP-pair input variant; their broader restoration architectures are not specific to DP sensors.

|Year|Pub|Paper|DP relevance|Repo|
|:---:|:---:|:---:|:---:|:---:|
|2021|CVPR|[Iterative Filter Adaptive Network for Single Image Defocus Deblurring](https://openaccess.thecvf.com/content/CVPR2021/html/Lee_Iterative_Filter_Adaptive_Network_for_Single_Image_Defocus_Deblurring_CVPR_2021_paper.html)|IFAN: DP disparity supervision during training; single-image inference and a DP-pair variant|[Code](https://github.com/codeslake/IFAN)|
|2022|CVPR|[Restormer: Efficient Transformer for High-Resolution Image Restoration](https://openaccess.thecvf.com/content/CVPR2022/html/Zamir_Restormer_Efficient_Transformer_for_High-Resolution_Image_Restoration_CVPR_2022_paper.html)|Single-image and DP-pair defocus deblurring|[Code](https://github.com/swz30/Restormer)|
|2023|TPAMI|[Learning Enriched Features for Fast Image Restoration and Enhancement](https://doi.org/10.1109/TPAMI.2022.3167175)|MIRNet-v2: DP-pair defocus deblurring|[Code](https://github.com/swz30/MIRNetv2)|
|2023|CVPR|[Efficient and Explicit Modelling of Image Hierarchies for Image Restoration](https://openaccess.thecvf.com/content/CVPR2023/html/Li_Efficient_and_Explicit_Modelling_of_Image_Hierarchies_for_Image_Restoration_CVPR_2023_paper.html)|GRL: single-image and DP-pair defocus deblurring|[Code](https://github.com/ofsoundof/GRL-Image-Restoration)|
|2024|CVPR|[Boosting Image Restoration via Priors from Pre-trained Models](https://openaccess.thecvf.com/content/CVPR2024/html/Xu_Boosting_Image_Restoration_via_Priors_from_Pre-trained_Models_CVPR_2024_paper.html)|PTG-RM: refinement of GRL for DP-pair defocus deblurring||
|2025|WACV|[F2former: When Fractional Fourier Meets Deep Wiener Deconvolution and Selective Frequency Transformer for Image Deblurring](https://openaccess.thecvf.com/content/WACV2025/html/Paul_F2former_When_Fractional_Fourier_Meets_Deep_Wiener_Deconvolution_and_Selective_WACV_2025_paper.html)|Single-image and DP-pair defocus deblurring||

## Related Quad-Pixel research

QP/QPD sensors provide four sub-aperture measurements rather than the two of a DP sensor. Related datasets are kept separate below.

|Year|Pub|Paper|App|Repo|
|:---:|:---:|:---:|:---:|:---:|
|2024|BMVC|[Disparity Estimation Using a Quad-Pixel Sensor](https://bmva-archive.org.uk/bmvc/2024/papers/Paper_480/paper.pdf)|QP Disparity / Synthetic Data|[Code & Dataset](https://github.com/Zhuofeng-Wu/QPDNet)|
|2025|CVPR|[All-directional Disparity Estimation for Real-world QPD Images](https://openaccess.thecvf.com/content/CVPR2025/html/Yu_All-directional_Disparity_Estimation_for_Real-world_QPD_Images_CVPR_2025_paper.html)|DP / QPD Disparity / QPD2K Dataset||
|2025|CVPR|[Quad-Pixel Image Defocus Deblurring: A New Benchmark and Model](https://openaccess.thecvf.com/content/CVPR2025/html/Chen_Quad-Pixel_Image_Defocus_Deblurring_A_New_Benchmark_and_Model_CVPR_2025_paper.html)|QP Defocus Deblurring / QPDD Dataset||

## Dataset

Links lead to author download instructions or papers describing the data; access restrictions and unverified download availability are indicated. Counts denote scenes, image sets, or pairs as specified.

|Year|Pub|Paper|Detail|
|:---:|:---:|:---:|:---:|
|2019|ICCV|[Learning Single Camera Depth Estimation using Dual-Pixels](https://github.com/google-research/google-research/tree/master/dual_pixels)|Train:2506, Test:684, Res:1512x2016(DP), 16bit png, DP Raw / Depth|
|2020|ICCP|[Modeling Defocus-Disparity in Dual-Pixel Sensors](https://github.com/abhijithpunnappurath/dual-pixel-defocus-disparity)|Num:100, Res:5180x2940, RGB 8bit jpg / 16bit tif Depth, DP LR / Depth|
|2020|ECCV|[Defocus Deblurring Using Dual-Pixel Data](https://github.com/Abdullah-Abuolaim/defocus-deblurring-dual-pixel)|DPDD: 500 scenes (350 train / 74 validation / 76 test), Res:1680x1120, 16bit; DP L/R, combined blurry and sharp reference images; used for NTIRE 2021 (CVPRW)|
|2020|CVPR|[Learning to Autofocus](https://learntoautofocus-google.github.io/)|510 focal stacks with conventional/DP measurements and per-pixel depth from multi-view stereo; download instructions on the project page|
|2021|CVPR|[Dual Pixel Exploration: Simultaneous Depth Estimation and Image Restoration](https://github.com/panpanfei/Dual-Pixel-Exploration-Simultaneous-Depth-Estimation-and-Image-Restoration)|DP Simulator from [NYUD Dataset](https://cs.nyu.edu/~silberman/datasets/nyu_depth_v2.html)|
|2021|ICCV|[Learning to Reduce Defocus Blur by Realistically Modeling Dual-Pixel Data](https://github.com/Abdullah-Abuolaim/recurrent-defocus-deblurring-synth-dual-pixel)|DP Simulator from [SYNTHIA-SF dataset](https://synthia-dataset.net/downloads/)|
|2021|ICCV|[Defocus Map Estimation and Deblurring From a Single Dual-Pixel Image](https://github.com/cmu-ci-lab/dual_pixel_defocus_estimation_deblurring)|17 indoor/outdoor scenes captured with Google Pixel 4; green-channel 14-bit DP data, calibrated blur kernels and vignetting patterns included in the repository|
|2022|ECCV|[Facial Depth and Normal Estimation using Single Dual-Pixel Camera](https://github.com/MinJunKang/DualPixelFace)|More than 135K images of 101 people; metric depth, normals and calibration; signed license agreement and author request required|
|2023|ICCP|[Learning to Synthesize Photorealistic Dual-pixel Images from RGBD frames](https://github.com/feiran-l/Neural-Dual-Pixel-Simulator)|Num:5130, Res:1680x1120, RGB(DP LRC) 8bit png / Depth 16bit png|
|2024|TPAMI (BMVC 2022 precursor)|[Dual-Pixel Raindrop Removal](https://github.com/Yizhou-Li-CV/DPRRN)|Synthetic-Raindrop: 1960 train / 492 test pairs for each tilted/vertical setting; Real-Waterdrop: 130 tilted / 125 vertical test pairs; Real-Car: 94 tilted pairs; BMVC and expanded TPAMI versions available|
|2024|ICCP|[Stereo-Knowledge Distillation from dpMV to Dual Pixels for Light Field Video Reconstruction](https://arxiv.org/abs/2405.11823)|dpMV: three-view DP video data for stereo distillation and light-field video reconstruction; public download not verified|
|2024|ECCV|[Resolving Scale Ambiguity in Multi-view 3D Reconstruction using Dual-Pixel Sensors](https://github.com/kohei-ashida/dp-sfm)|DSLR/phone multi-view DP sequences for metric 3D reconstruction; download links in the repository|
|2025|WACV|[Revisiting Disparity from Dual-Pixel Images: Physics-Informed Lightweight Depth Estimation](https://github.com/sony/dual-pixel-disparity)|SEDC (Synthetic Edge Depth Completion): synthetic training data for DP disparity estimation, not real DP captures; Microsoft account and author-granted access required|
|2025|ICCV|[Simulating Dual-Pixel Images From Ray Tracing For Depth Estimation](https://github.com/LinYark/Sdirt)|DP119: real DP/depth test set, Canon R6 Mark II + RF50mm, fixed focus at 1m and F/4; simulator and sample data also provided|
|2025|IROS|[DiFuse-Net](https://arxiv.org/abs/2506.14709)|DCDP (Dual-Camera Dual-Pixel): real RGB/DP/depth training benchmark introduced in the paper; public download not verified|

### Related QP datasets

|Year|Pub|Paper / Dataset|Detail|
|:---:|:---:|:---:|:---:|
|2024|BMVC|[QPDNet synthetic dataset](https://github.com/Zhuofeng-Wu/QPDNet)|Synthetic QP views and disparity generated from RGB-D data; see repository download instructions|
|2025|CVPR|[QPD2K](https://openaccess.thecvf.com/content/CVPR2025/html/Yu_All-directional_Disparity_Estimation_for_Real-world_QPD_Images_CVPR_2025_paper.html)|2100 real-world QPD image sets with disparity maps; public download not verified|
|2025|CVPR|[QPDD](https://openaccess.thecvf.com/content/CVPR2025/html/Chen_Quad-Pixel_Image_Defocus_Deblurring_A_New_Benchmark_and_Model_CVPR_2025_paper.html)|Quad-Pixel defocus deblurring benchmark; public download not verified|
