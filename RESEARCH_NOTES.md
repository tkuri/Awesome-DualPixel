# Literature review notes

Review date: **2026-10-11 (Japan time)**.

The update adds **30 paper entries** to the original 28: 21 DP-specific papers, six restoration methods with explicit DP use, and three related QP papers. The dataset tables gain nine DP/data-generation resources and three QP resources. Existing entries are retained, with corrections to navigation, venue names, a stale paper link, and spelling.

## Selection and search

The existing list includes CVPR, ICCV, ECCV, SIGGRAPH, ICCP, WACV, 3DV, workshops, specialist conferences, and journals. The requested venue threshold was interpreted as an approximate curation standard, rather than an absolute ranking across research communities. The additions emphasize established peer-reviewed venues, including TPAMI, IJCV, TIFS, IEEE/CAA JAS, NeurIPS, ACM MM, IROS, ICME, ICASSP, and the specialist MVA conference. The two Elsevier journal papers are directly about DP deblurring. Existing lower-profile or workshop entries were not removed.

Searches used `dual pixel`, `dual-pixel`, `dual-pixels`, `quad-pixel`, and `QPD`, combined with years (especially 2024–2026), venue names, and depth/disparity, autofocus, deblurring, simulation, light-field, reflection, raindrop, and fence removal. Candidate titles were also checked against related-work bibliographies, author publication lists, and existing community lists. Final inclusion relies on primary paper/proceedings pages, author repositories, or publisher-deposited DOI metadata; community lists were discovery aids only.

DP-pair input, DP-specific supervision, sensor modeling, and actual use of DP hardware were checked separately from use of the single-image DPDD benchmark. Four-photodiode QP work is identified as related research. Conference papers and journal extensions are separate entries, even when the title is identical.

## Evidence for DP-specific additions

The paper links in the README provide title and method evidence. The following additional sources resolve venue, year, release status, or otherwise ambiguous details.

|Paper / method|Year and venue|Verification source / note|
|:---|:---|:---|
|Single-Shot Face Anti-Spoofing|2021, TIFS|[Publisher-deposited metadata](https://api.crossref.org/works/10.1109/TIFS.2020.3035879). Volume year is 2021; the DOI contains 2020.|
|BaMBNet|2022, IEEE/CAA JAS|[Journal article](https://www.ieee-jas.net/en/article/doi/10.1109/JAS.2022.105563) and [official code](https://github.com/junjun-jiang/BaMBNet).|
|DMTNet|2022, ICME|[Author organization description](https://research.samsung.com/news/Dual-Pixel-Image-Defocus-Deblurring-Technique-at-the-ICME-2022) and [publisher-deposited metadata](https://api.crossref.org/works/10.1109/ICME52920.2022.9859631).|
|Dual-Pixel Raindrop Removal|2022, BMVC|[Conference paper list, paper 439](https://bmvc2022.cvml.group/programme/papers/) and [author repository](https://github.com/Yizhou-Li-CV/DPRRN). The old conference PDF URL returned 404 during the link check; the README uses the author's [preprint](https://arxiv.org/abs/2210.13321).|
|MRNET|2023, ICASSP|[IEEE conference presentation](https://resourcecenter.ieee.org/conferences/icassp-2023/spsicassp23vid0164) and [publisher-deposited paper metadata](https://api.crossref.org/works/10.1109/ICASSP49357.2023.10096428).|
|dpMV / DP light-field video|2024, ICCP|[Author lab publication list](https://www.ee.iitm.ac.in/comp_photolab/) and [official implementation](https://github.com/Aryan-Garg/dp-LFVR). Dataset introduction is confirmed; a public download was not verified.|
|Split-Aperture 2-in-1 Cameras|2024, SIGGRAPH / TOG|[Author project page and BibTeX](https://light.princeton.edu/publication/2in1-camera/). Uses DP hardware for coded/uncoded capture. The project lists TOG 43(4), article 141, DOI 10.1145/3658225; an alternate DOI seen in a community list was not adopted.|
|Weakly-Supervised Depth and Deblurring|2024, TPAMI|[Author institution publication record](https://researchportalplus.anu.edu.au/en/publications/weakly-supervised-depth-estimation-and-image-deblurring-via-dual-/) and [author code](https://github.com/zwxu064/DiffImageWarpingCUDA). The linked code is the differentiable warping component, not a verified complete training implementation.|
|Dual-Pixel Raindrop Removal (extension)|2024, TPAMI|[Author repository](https://github.com/Yizhou-Li-CV/DPRRN) identifies both publications and provides separate BMVC/TPAMI data links and expanded dataset counts.|
|DPANet|2025, Neurocomputing|[Publisher page](https://www.sciencedirect.com/science/article/pii/S0925231224016515): volume 616, 1 February 2025. The 2022 preprint and 2024 DOI/online date are not the volume year.|
|PA-Net|2025, Engineering Applications of Artificial Intelligence|[Publisher page](https://www.sciencedirect.com/science/article/abs/pii/S0952197624017706): volume 139, January 2025.|
|FMDP|2025, MVA|[Conference proceedings record](https://doi.org/10.34385/proc.93.O1-1-2): Machine Vision Applications, 26 July 2025.|
|Sdirt|2025, ICCV|[Official proceedings](https://openaccess.thecvf.com/content/ICCV2025/html/He_Simulating_Dual-Pixel_Images_From_Ray_Tracing_For_Depth_Estimation_ICCV_2025_paper.html) and [official code / DP119](https://github.com/LinYark/Sdirt).|
|Spatially-Varying Autofocus|2025, ICCV|[Author project](https://imaging.cs.cmu.edu/svaf/) identifies ICCV and the DP-based prototype. This is an optical autofocus system, not just an image restoration network.|
|DiFuse-Net|2025, IROS|[Author preprint](https://arxiv.org/abs/2506.14709) explicitly states acceptance at IROS 2025. DCDP is described, but a public dataset release was not verified.|
|Enhanced DP Reflection Removal|2025, ACM MM|[Publisher-deposited metadata](https://api.crossref.org/works/10.1145/3746027.3755094) confirms the exact title and Proceedings of the 33rd ACM International Conference on Multimedia.|
|User-Instructed Defocus Control|2025, NeurIPS|[Official main-conference proceedings](https://proceedings.neurips.cc/paper_files/paper/2025/hash/180836fd0a8f164d189d7e244ec8841a-Abstract-Conference.html).|
|Freq-DP Net|2026, ICASSP|[Official conference program, paper 18299](https://cmsworkshops.com/ICASSP2026/view_paper.php?PaperNum=18299) and [author preprint](https://arxiv.org/abs/2602.14226). Confirmed acceptance makes this eligible despite using an arXiv paper link.|
|DCRR++|2026, IJCV|[Publisher article](https://link.springer.com/article/10.1007/s11263-026-02892-2), published 24 May 2026. Code/data are promised in the article; a release URL was not verified.|
|DP-SfM|2026, TPAMI|[Official author repository and journal citation](https://github.com/lilika-makabe/dp-sfm-tpami) confirm TPAMI 2026 and DOI 10.1109/TPAMI.2026.3690655. Repository still describes code/data as upcoming.|
|FoundDP|2026, ECCV accepted|[Author publication/acceptance announcement](https://linyark.github.io/) and [official project](https://github.com/EchoLighting/FoundDP). Acceptance is verified; final proceedings metadata and full code/data release are not verified.|

## Restoration and QP evidence

|Method|Primary evidence for inclusion|
|:---|:---|
|IFAN, CVPR 2021|[Paper](https://openaccess.thecvf.com/content/CVPR2021/papers/Lee_Iterative_Filter_Adaptive_Network_for_Single_Image_Defocus_Deblurring_CVPR_2021_paper.pdf), section 3.3: DP disparity training. [Official repository](https://github.com/codeslake/IFAN) also provides an `IFAN_dual` variant.|
|Restormer, CVPR 2022|[Proceedings abstract](https://openaccess.thecvf.com/content/CVPR2022/html/Zamir_Restormer_Efficient_Transformer_for_High-Resolution_Image_Restoration_CVPR_2022_paper.html) explicitly lists both single-image and DP-data defocus deblurring.|
|MIRNet-v2, TPAMI 2023|[Author institution publication record](https://research.monash.edu/en/publications/learning-enriched-features-for-fast-image-restoration-and-enhance/) confirms volume 45(2), 2023. [Official repository](https://github.com/swz30/MIRNetv2) includes DP defocus models.|
|GRL, CVPR 2023|[Paper](https://openaccess.thecvf.com/content/CVPR2023/papers/Li_Efficient_and_Explicit_Modelling_of_Image_Hierarchies_for_Image_Restoration_CVPR_2023_paper.pdf) reports a separate DP defocus deblurring evaluation.|
|PTG-RM, CVPR 2024|[Paper](https://openaccess.thecvf.com/content/CVPR2024/papers/Xu_Boosting_Image_Restoration_via_Priors_from_Pre-trained_Models_CVPR_2024_paper.pdf) reports DP defocus refinement, including GRL comparisons and the DP-specific user study.|
|F2former, WACV 2025|[Paper](https://openaccess.thecvf.com/content/WACV2025/papers/Paul_F2former_When_Fractional_Fourier_Meets_Deep_Wiener_Deconvolution_and_Selective_WACV_2025_paper.pdf) evaluates both single-image and DP defocus deblurring.|
|QPDNet, BMVC 2024|[Official conference paper](https://bmva-archive.org.uk/bmvc/2024/papers/Paper_480/paper.pdf) identifies four-photodiode QP sensing and synthetic training data; [official code/data](https://github.com/Zhuofeng-Wu/QPDNet).|
|QuadNet / QPD2K, CVPR 2025|[Official proceedings](https://openaccess.thecvf.com/content/CVPR2025/html/Yu_All-directional_Disparity_Estimation_for_Real-world_QPD_Images_CVPR_2025_paper.html) describes DPNet, QuadNet, and 2100 real-world QPD samples.|
|QP defocus deblurring / QPDD, CVPR 2025|[Official proceedings](https://openaccess.thecvf.com/content/CVPR2025/html/Chen_Quad-Pixel_Image_Defocus_Deblurring_A_New_Benchmark_and_Model_CVPR_2025_paper.html) establishes the QP task and benchmark.|

## Dataset and existing-entry corrections

New dataset summaries use the linked authors' papers/repositories. In particular, [Learning to Autofocus](https://learntoautofocus-google.github.io/) reports 510 focal stacks; [Xin et al.](https://github.com/cmu-ci-lab/dual_pixel_defocus_estimation_deblurring) provide 17 Pixel 4 scenes and device calibration; [DualPixelFace](https://github.com/MinJunKang/DualPixelFace) requires a signed agreement and author request; [SEDC](https://github.com/sony/dual-pixel-disparity) is synthetic depth-completion training data with author-granted access, not a new real-captured DP test set.

The two rows previously labeled only `IEEE` are now identified as Hot Chips and the VLSI Symposium. The [publisher-deposited Hot Chips metadata](https://api.crossref.org/works/10.1109/HCS52781.2021.9567122) confirms the former. The original ECCV 2020 project URL returned 404 and was replaced with the [official ECVA paper page](https://www.ecva.net/papers/eccv_2020/papers_ECCV/html/1003_ECCV_2020_paper.php). LDP's [official implementation](https://github.com/noxsine/LDP) fills an existing empty code cell.

## Exclusions and limitations

- [Adjust Your Focus / MCCNet](https://arxiv.org/abs/2502.11002): no qualifying peer-reviewed venue was confirmed, so it was not added.
- [Revisiting Autofocus for Smartphone Cameras](https://openaccess.thecvf.com/content_ECCV_2018/html/Abdullah_Abuolaim_Revisiting_Autofocus_for_ECCV_2018_paper.html): relevant autofocus background, but the proposed temporal focal-stack benchmark is not a DP measurement method. It was not added to the DP tables.
- Single-image DPDD-only restoration papers and conventional stereo/light-field methods were excluded unless actual DP training or a DP-pair experiment was established. The six restoration entries are a curated set, not an exhaustive inventory of every DPDD baseline.
- Hardware/device workshops and niche journals were not comprehensively expanded; the review focuses on computer vision and computational imaging. Venue comparisons are editorial judgments, not a claim of an objective ranking.
- Metadata verification does not imply reproducibility testing. No models were trained, codebases executed, or large datasets downloaded. Download instructions and restrictions were checked where available.
- Automated HTTP checks encountered publisher bot protection and local TLS failures on some arXiv/journal URLs. These are recorded as access limitations, not evidence that a paper is missing. DOI metadata and browser-search primary sources were used for cross-checks. Definite stale 404 paper links were replaced. Public dataset downloads remain unverified where labeled in the README.
- Search-index coverage and publication/release status can change. This review substantially fills recent and historical gaps, but does not claim complete coverage of all DP-related literature.
