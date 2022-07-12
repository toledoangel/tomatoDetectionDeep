# tomatoDetectionDeep
Automatic tomato weed detection and classification system using convolutional neural networks and deep learning.



## Context

Weed detection in tomato crops (Weedetec Tomato) is a project that was carried out during my intership at the Centro de Automática y Robótica del Consejo Superior de Investigaciones Científicas (CAR-CSIC) in Madrid, Spain. The objective is to incorporate an intelligent weed detection system to the herbicide application for a precise application based on the real needs of the field. 

## Resumen

Industrial tomato (Solanum lycopersicum L.) is one of the most important agricultural crops worldwide. Weed control is of high importance due to the associated cost on this crop. Although weeds are heterogeneously present on the field creating weed patches, the conventional approach is to carry out an uniform herbicide application. Thus, site-specific management plays an important role by detecting and spatial positioning weed distribution within the fields. Object detection systems, using neural networks based on deep learning, are a potentially viable option given their extraordinary versatility. The present work aims to develop an automatic weed detection and classification system for the following species: Portulaca oleracea L., Cyperus rotundus L., Solanum nigrum L. Echinocloa cruzgalli L., Setaria italica L. It employs one-stage object detection algorithm based on neural networks. For this purpose, a data set formed by RGB images, properly labeled in the European and Mediterranean Plant Protection Organization (EPPO) code, was developed and trained using Retina Net Object Detection Model. The performance evaluation with the mean Average Precision (mAP) metric, showed a result of correct classification higher than 90%, discriminating between tomato crops and the two groups broadleaf and narrowleaf weeds. In addition narrow leaf weeds were properly separated, such as, Cyperaceae and Poaceae families. This research is the basis of the development of intelligent tools for weed control in tomato fields looking for a more sustainable agriculture

## Introduction 

Tomato (Solanum lycopersicum L.) is one of the most important agricultural crops in the world. Weed control is of great importance due to the cost associated with this crop as it can jeopardize its production. Although weeds are heterogeneously present in the field. The conventional approach is to carry out a uniform herbicide application. Therefore, site-specific management plays an important role in detecting and spatially positioning the distribution of weeds in fields with economic, environmental benefits and achieving better food quality.   Object detection systems, using neural networks based on deep learning, are a potentially viable option given their extraordinary versatility.  

The present work aims to develop an automatic weed detection and classification system for the following species: Portulaca oleracea L., Cyperus rotundus L., Solanum nigrum L. Echinocloa cruzgalli L., Setaria italica L.

## Dataset

This repository contains a dataset of images acquired in the province of Badajoz (Spain). It has been labelled using Labelimg and the labels can be found in pascal voc format, or in csv. The code used for the labels was the European and Mediterranean Plant Protection Organisation (EPPO) code.
The labelled species are: 
<i>Cyperus rotundus L.</i> (CYP-CYPRO)
<i> Echinocloa cruz gallo L. </i> (ECHCG)
<i>Setaria italica L. </i> (SETIT)
<i>Portulaca oleracea L.</i> (POROL)
<i>Solanum nigrum L.</i> (SOLNI)
Tomato crop label added
<i>Solanum lycopersicum L.</i> (Lypes)
And a category for unrecognised weeds was added. 
<i>Unrecognised weeds</i> (NCI)

