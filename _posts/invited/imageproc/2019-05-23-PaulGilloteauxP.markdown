---
title: "Paul-Gilloteaux, P. | Automatic Registration of Correlative Microscopies with Error Assessment and Applications for the Optimization of Multimodal Acquisitions"
layout: post
date: 2019-05-23 14:00
image: https://media.scandem2019.se/2018/11/PerrinePaul-Gilloteaux.jpg
headerImage: true
tag:
- invited
- image processing/analysis
category: projects
author:

---

_Amina Achaibou<sup>1</sup>, Guillaume Potier<sup>1</sup>, Romain Capoulade<sup>1</sup>, Jean Mérot<sup>1</sup>, Frédéric Lavancier<sup>2</sup>, Xavier Heiligenstein<sup>3</sup>, Jean Salamero<sup>3</sup>, **Perrine Paul-Gilloteaux**<sup>1,4*</sup>_<br/>

1 l'institut du thorax, UNIV Nantes, CNRS, INSERM, Nantes, France.<br/>
2 Laboratoire de Mathématiques J Leray, UNIV Nantes, CNRS, Nantes, France.<br/>
3 Institut Curie, PSL, CNRS, Paris, France.<br/>
4 Structure Fédérative de Recherche François Bonamy, UNIV Nantes, CNRS, INSERM, Nantes, France.<br/>

## Abstract

Correlative microscopy allows combining different scales of observations and different contents, functional and morphological, based on the large panel of microscopy technologies available for life or material sciences. The purpose is to accurately follow a region of interest across modalities and scales of imaging, for guiding and targeting the specimen preparation procedure needed for another modality, to guide the acquisition at the second microscope and to adjust the field of view of the microscope to this feature. In a last, and most accurate registration step, the acquired data from both modalities are mapped.<br/>

Data fusion (or registration) methods have to be considered and planned initially when developing an imaging workflow, from the sample preparation to imaging acquisition. The challenges in registration for correlative microscopies are due to:   

a)	The variations of densities in the points extracted, due partly to the difference in resolution: several elements of one high-resolution modality, would appear as a single element in a larger field of view modality due to the diffraction limit; <br/>  
b)	Missing data: some modalities are not specific and show the whole content of the area imaged, meaning that many structures will not appear in a functional imaging modality <br/>  
c)	The large variations in image scale, rotation, and translation, and deformation of the sample due to the sample preparation or to the sample itself;<br/>   
d)	The large diversity of imaging content and scale at the different steps of a correlative microscopy workflow; <br/>  
e)	The lack of methods for computing the accuracy of the registration and even predict it before the experiment. <br/>

To overcome these difficulties, we present a point-based registration paradigm, implemented in a free and open source software Ec-CLEM AutoFinder, an extension to EC-CLEM [1], which presents several advantages. This software is available in the Icy platform [2].<br/>

The only step of our registration workflow which differs between workflows, whatever the dimensionality of data, is the feature extraction step, which can be learned on uncorrelated images. Using an image to image deep learning framework facilitate the task here, but we show that ad-hoc methods can also be faster and efficient. <br/>

It includes a method for the selection model of non-rigid transformation, for which the transformation basis is selected according to its physical significance. <br/>
We also present a statistical framework of error estimation on the registration error allowing to answer the question of the confidence of the matching of structures. This framework can also be used before the experiment to decipher, for example, the density and needed accuracy in localization of external fiducials such as beads or q-dots, or the possibility and accuracy to be expected while using natural common elements such as vessels, nuclei, mitochondria or any common shape.<br/>

The software is now also able to process images bigger than the computer memory available, and the user experience tends to be facilitated.<br/>

## References:

[1] P Paul-Gilloteaux et al., Nature Methods 14 (2017) p. 102-103.<br/>
[2] F de Chaumont et al., Nature Methods 9 (2012) p. 690-696.<br/>
