---
layout: default
title: Change Detection
parent-collection: projects
---

## Change Detection of Small Water Bodies in Alluvial Gold Mining Satellite Imagery

Monitoring change detection of the land surface is one of the critical concepts in the mean of natural
resource management, deforestation, and conservation. One of the most causes of land degradation,
deforestation, and water pollution is artisanal and small-scale mining (ASM) which is basically related to
water bodies. To monitor the water bodies that are potential ASM ponds and detect the changes
satellite imagery is commonly used. For fine-scale change detection, satellite images can be challenging
because of atmospheric conditions on spectral data and representing individual objects with connecting
pixels.


In this project, we investigate the change detection in the context of a current conservation challenge,
artisanal-scale gold mining (ASGM) performance of two machine learning approaches (supervised and
semi-supervised learning) on Sentinel-2 images. We obtained Sentinel-2 imagery and created an open-
source labeled (binary and multiclass: ‘increase, decrease, water existence/absence’) land-cover change
dataset for the Madre de Dios (MDD) region in Peru, a hotspot of ASGM activity, as well as active ASGM
areas in other countries (Venezuela, Indonesia, and Myanmar). As supervised learning, we used E-
ReCNN model and for semi-supervised learning, we used the SVM-STV approach with histogram
matching preprocessing steps on multiple channels and additional La*b* color space improved
performance and reduce the influence of atmospheric effects.