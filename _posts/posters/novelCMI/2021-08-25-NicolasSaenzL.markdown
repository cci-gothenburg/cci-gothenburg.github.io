---
title: "Correlation of optical microscopy and ion beam data for trace element spatial localization in TB lesions"
layout: post
date: 2021-08-25 14:00
image: 
headerImage: false
tag:
- poster
- novel correlative imaging
category: projects
author:
#description: Markdown summary with different options
---

_**Laura Nicolás-Sáenz**<sup>1</sup>, Melanie J. Bailey<sup>2</sup>, Catia Costa<sup>3</sup>, Janella de Jesus<sup>4</sup>, Juan José Vaquero<sup>1</sup>, Véronique Dartois<sup>5</sup>, Arrate Muñoz-Barrutia<sup>1</sup>_

1 Departamento de Bioingeniería e Ingeniería Aeroespacial, Universidad Carlos III de Madrid, Madrid, Spain & Instituto de Investigación Sanitaria Gregorio Marañón, Madrid, Spain

2 Department of Chemistry, University of Surrey, Surrey, UK & Surrey Ion Beam Centre, University of Surrey, Surrey, UK

3 Surrey Ion Beam Centre, University of Surrey, Surrey, UK

4 Department of Chemistry, University of Surrey, Surrey, UK

5 Public Health Research Institute, Rutgers University − New Jersey Medical School, 225 Warren St, Newark, New Jersey 07103, United States

## Abstract

Tuberculosis (TB) is one of the top ten causes of death worldwide and develops following infection by Mycobacterium tuberculosis. To further understand TB lesions, a comprehensive study of the tissue composition of these lesions was conducted using Hematoxylin and Eosin (H&E) stained biopsies for structural information and Ion Beam for trace element analysis (IBA).

Two consecutive tissue cuts were obtained from a rabbit TB lesion, one of which was used for Ion Beam analysis. The cuts were later stained with H&E, and imaged using brightfield microscopy. Due to the interaction of the ion beam with the tissue, the area where the beam had incised appeared bleached out after staining, losing information. We propose a method for the reconstruction of the damaged areas to facilitate the correlation of the two image modalities.

The pipeline developed consisted of four steps:

1) Tissue segmentation and registration where the lesions were detected and segmented from the slide background to perform linear registration.

2) The damaged areas were detected. Then, the immediately successive tissue cuts were used to reconstruct the lost information of the samples subjected to the Ion Beam.

3) The IBA data was reassembled since the obtained images were of four heterogeneously overlapping regions within a 2µm area. The area was reconstructed using cross-correlation analysis of the main features of the tissue.

4) The final step was to align the IBA data with the corresponding area in the H&E. Due to changes in the acquisition angle between the confocal microscopy and the Ion Beam, registration of the two modalities had to be performed using overlapping tiles with subsequent stitching.

With this pipeline, we were able to perform a fully automatic and efficient multi-modality matching to obtain the elemental composition of a tuberculosis lesion with a final registration error of 3 pixels.
