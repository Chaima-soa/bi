# Tilapia-RAS Dataset: Underwater Videos and Polygon-Annotated Frames with Physicochemical Metadata

**DOI (Zenodo):** 10.5281/zenodo.17518786

---

## Overview

This dataset provides underwater video recordings of Nile tilapia (*Oreochromis niloticus*) collected at a commercial recirculating aquaponic system (RAS) in Querétaro, Mexico.

The recordings were intentionally captured under challenging, real-world conditions, including moderate turbidity, suspended solids, and variable illumination. The goal is to provide a robust resource for developing and benchmarking computer vision models for aquaculture monitoring.

The dataset includes:

* **31 video clips** (30 seconds each).
* **3,520 annotated frames** (from a subset of 4 clips) in LabelMe JSON format.
* **Physicochemical metadata** (one `.csv` file) synchronized with the clips, detailing water quality parameters like temperature, pH, dissolved oxygen, and turbidity.

## How to Cite

If you use this dataset in your research, please cite the Zenodo repository.

### Dataset Citation

Aragón-Banderas, O.; Trujillo, L.; Salazar-Muñoz, Y.; Baguette, G.J.V.E.; Arce-Valdez, J.L. Tilapia-RAS Dataset: Underwater Videos and Polygon-Annotated Frames with Physicochemical Metadata. Zenodo, 2025. DOI: 10.5281/zenodo.17518786

## License

This dataset is released under the Creative Commons Attribution 4.0 International (CC BY 4.0) license.

## Dataset Structure

The repository is organized as follows. 

Tilapia RAS Dataset/
├── Readme.md                     (This file)
├── Documentation/
│   ├── meta_tilapia_set.csv       (The key metadata file)
│   ├── Variable_Definitions.pdf   (Explains the CSV columns)
│   ├── Capture_Setup.png          (Diagrams of the setup)
│   └── Dataset_Structure.png      (The diagram this text is based on)
├── Videos/
│   ├── Original/                  (The 31 original .mp4 clips)
│   └── Samples/                   (Sample clips, if included)
└── Frames/
    ├── Original/
    │   ├── images/                (The 3,520 original annotated frames)
    │   └── annotation/            (The 3,520 original .json labels)
    └── Augmented/
        ├── AveragedBlur/          (Images/annotations with mean blur)
        └── GaussianBlur/          (Images/annotations with Gaussian blur)
