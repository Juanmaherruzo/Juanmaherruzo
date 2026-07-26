I'm a third-year Forestry Engineering student developing production-grade Python pipelines that bring together UAV photogrammetry, multispectral remote sensing, and machine learning to automate forest inventory. My goal is to close the gap between classical silviculture and modern geospatial data science — bringing operational rigor to a field that still relies heavily on manual sampling, paper-to-spreadsheet workflows, and stratification decisions made from memory and PDFs.

The bottleneck in forestry today isn't data. It's tooling. Every meaningful input — UAV imagery, Sentinel-2 time series, LiDAR, NDVI — is already available, often for free. What's missing are pipelines that someone trained as a forester (not as a software engineer) can actually run, on real datasets, on hardware they own. That's the gap I'm trying to work in.

**What I build**

Three open-source projects on GitHub anchor my work, all MIT-licensed and written in professional English.

**Dehesa-Crown-Segmentation-YOLOv11** is an instance-segmentation system for individual tree crown detection on UAV orthomosaics. It uses YOLOv11 with a producer-consumer inference architecture I designed to eliminate VRAM exhaustion on 4 GB laptop GPUs. The pipeline has been validated on a 14,506-hectare dehesa dataset, detecting 357,185 individual trees with documented precision, recall, and mAP metrics for both box and mask predictions.

**sentinel2-spectraldex** is a Sentinel-2 Level-2A processing pipeline running entirely on the free Copernicus CDSE API. It handles AOI-driven scene search with cloud-cover filtering, OAuth2 authentication with exponential backoff, selective band download, multi-tile MGRS merging in memory, and computation of six spectral indices (NDVI, SAVI, EVI, NBR, NDRE, NDWI). It includes a validation dashboard and a technical note on why NDRE complements NDVI in closed canopies where NDVI saturates.

**annotation-station** is a full-stack, privacy-first image annotation platform built with FastAPI, React, and SAM 2.1. It's designed for users who cannot send sensitive imagery to cloud-based labelling services. The system uses a three-level embedding cache to run smoothly on 4 GB VRAM laptop GPUs and exports to YOLO-segmentation, YOLO-detection, and COCO formats. The repository includes measured performance comparisons against Roboflow, CVAT, and Label Studio for the local-first use case.

**How I'm growing**

Alongside my degree, I'm following a structured self-directed roadmap across machine learning, deep learning, computer vision, and geospatial data engineering. The progression covers mathematical foundations, the scikit-learn ecosystem and ensemble methods, PyTorch and CNN architectures, transfer learning, and computer vision applied to remote sensing.  My goal is to combine academic forestry training with the technical depth needed to deliver production-grade geospatial tools.

**Where I'm headed**

I'm interested in operational remote sensing, forest carbon MRV, adaptive management of Mediterranean woodlands, and the integration of GIS and AI inside forestry consultancies and research groups. I see myself contributing to organisations that are serious about turning satellite and UAV data into decisions on the ground — whether that's a consultancy, a public research institute, or a startup working on natural-capital monitoring.

**Open to**

- Internships in geospatial ML, precision forestry, remote sensing, or computer vision (Spain or remote).
- R&D collaborations with research groups, public institutes, or companies working on operational forest monitoring.
- Technical conversations with people building at the intersection of forestry, earth observation, and applied AI.
- Mentorship from senior engineers and researchers — I'm at the stage where good feedback is worth more than gold.

If any of this resonates, and you want to talk afterwards, I'd be glad to.

Córdoba, Spain · GitHub: Juanmaherruzo
