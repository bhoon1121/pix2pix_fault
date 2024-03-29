---
# Synthetic seismic data generation with pix2pix for enhanced fault detection model training
### Byunghoon Choi, Sukjoon Pyun, Woochang Choi, and Yongchae Cho
---

## Description
In this study, we employ the pix2pix model [(Isola et al., 2017)](https://doi.org/10.48550/arXiv.1611.07004.) to generate seismic sections for fault detection, integrating it with sketch-based modeling (SBM) [(Ferreira et al., 2019)](https://doi.org/10.1109/LGRS.2019.2945680.). Pix2pix is an image-to-image translation model within a conditional generative adversarial networks framework, tailored to the user needs by using images as conditional variables. We experiment with our proposed method using field data examples from the Netherlands Offshore F3 Block. Our approach successfully replicates texture-related attributes, including noise, frequency, and amplitude, to resemble field data, thereby facilitating fault interpretation. We provide insights from variations in seismic data and fault interpretation results based on four sketch generation methods and loss function weights of pix2pix. 

![image](https://github.com/bhoon1121/pix2pix_fault/assets/46484101/494434e7-402d-46c5-9938-ad93fe7e9489)
#### Figure. Workflow of pix2pix-based fault detection

---
## Dataset
We provide only a few samples that can be implemented quickly in the code. If you want to implement this methodology, you'll need two datasets. One is the target dataset for interpreting faults, and the other is the reflectivity models with Labels.  

In this example, we used the Netherlands Offshore F3 Block as the target dataset.
- https://terranubis.com/datainfo/F3-Demo-2020

We created the reflectivity models and labels based on the paper referenced below. ***If there are any sketches available that closely resemble the structural characteristics of the field data, you can use those instead of reflectivity models.***
- Choi, W., & Pyun, S. (2021). Synthetic Training Data Generation for Fault Detection Based on Deep Learning. Geophysics and Geophysical Exploration, 24(3), 89–97. https://doi.org/10.7582/GGE.2021.24.3.089 [KOREAN]   


---
## Code
The implementation of the methodology is divided into two folders.
You can execute the code provided in each folder in the order indicated by the prefixed number index.
- https://github.com/bhoon1121/pix2pix_fault/tree/main/Loss_weight_compare
- https://github.com/bhoon1121/pix2pix_fault/tree/main/P_PT_PA_PTA_method

