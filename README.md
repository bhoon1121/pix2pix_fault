---
# Synthetic seismic data generation with pix2pix for enhanced fault detection model training
### Byunghoon Choi, Sukjoon Pyun, Woochang Choi, and Yongchae Cho
---

## Description
In this study, we employ the pix2pix model (Isola et al., 2017) to generate seismic sections for fault detection, integrating it with sketch-based modeling (SBM) (Ferreira et al., 2019). Pix2pix is an image-to-image translation model within a conditional generative adversarial networks framework, tailored to the user needs by using images as conditional variables. We experiment with our proposed method using field data examples from the Netherlands Offshore F3 Block. Our approach successfully replicates texture-related attributes, including noise, frequency, and amplitude, to resemble field data, thereby facilitating fault interpretation. We provide insights from variations in seismic data and fault interpretation results based on four sketch generation methods and loss function weights of pix2pix. 

![image](https://github.com/bhoon1121/pix2pix_fault/assets/46484101/494434e7-402d-46c5-9938-ad93fe7e9489)
#### Figure. Workflow of pix2pix-based fault detection

---
## References
- [Isola, P., Zhu, J. Y., Zhou, T., Efros, A. A., 2017. Image-to-image translation with conditional adversarial networks. In Proceedings of the IEEE conference on computer vision and pattern recognition, 1125-1134.](https://doi.org/10.48550/arXiv.1611.07004.)
- [Ferreira, R. S., Noce, J., Oliveira, D. A., Brazil, E. V., 2019. Generating sketch-based synthetic seismic images with generative adversarial networks. IEEE Geoscience and Remote Sensing Letters, 17 (8), 1460-1464.](https://doi.org/10.1109/LGRS.2019.2945680.)

---
## Data

---
## Code
The implementation of the methodology is divided into two folders.
You can execute the code provided in each folder in the order indicated by the prefixed index.
- https://github.com/bhoon1121/pix2pix_fault/tree/main/Loss_weight_compare
- https://github.com/bhoon1121/pix2pix_fault/tree/main/P_PT_PA_PTA_method

