<img src="https://github.com/toledoangel/tomatoDetectionDeep/blob/e52a7e88ca27fb2c9cf879c1dc0ecd71c482f0b7/imagesREADME/Logotipo%20condensado.png" width="150" >
# WeedtomatoDetection

Automatic tomato weed detection and classification system using convolutional neural networks and deep learning.



## Context
ss
Weed detection in tomato crops (Weedetec Tomato) is a project that was carried out during my intership at the Centro de Automática y Robótica del Consejo Superior de Investigaciones Científicas (CAR-CSIC) in Madrid, Spain. The objective is to incorporate an intelligent weed detection system to the herbicide application for a precise application based on the real needs of the field. 

## Resumen

Industrial tomato (Solanum lycopersicum L.) is one of the most important agricultural crops worldwide. Weed control is of high importance due to the associated cost on this crop. Although weeds are heterogeneously present on the field creating weed patches, the conventional approach is to carry out an uniform herbicide application. Thus, site-specific management plays an important role by detecting and spatial positioning weed distribution within the fields. Object detection systems, using neural networks based on deep learning, are a potentially viable option given their extraordinary versatility. The present work aims to develop an automatic weed detection and classification system for the following species: Portulaca oleracea L., Cyperus rotundus L., Solanum nigrum L. Echinocloa cruzgalli L., Setaria italica L. It employs one-stage object detection algorithm based on neural networks. For this purpose, a data set formed by RGB images, properly labeled in the European and Mediterranean Plant Protection Organization (EPPO) code, was developed and trained using Retina Net Object Detection Model. The performance evaluation with the mean Average Precision (mAP) metric, showed a result of correct classification higher than 90%, discriminating between tomato crops and the two groups broadleaf and narrowleaf weeds. In addition narrow leaf weeds were properly separated, such as, Cyperaceae and Poaceae families. This research is the basis of the development of intelligent tools for weed control in tomato fields looking for a more sustainable agriculture

## Introduction 

Tomato (Solanum lycopersicum L.) is one of the most important agricultural crops in the world. Weed control is of great importance due to the cost associated with this crop as it can jeopardize its production. Although weeds are heterogeneously present in the field. The conventional approach is to carry out a uniform herbicide application. Therefore, site-specific management plays an important role in detecting and spatially positioning the distribution of weeds in fields with economic, environmental benefits and achieving better food quality.   Object detection systems, using neural networks based on deep learning, are a potentially viable option given their extraordinary versatility.  

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

## Training

The dataset was divided into 70% for training set and 30% for validation set. It was trained using transfer learning with the Retina Net one-step object detection and classification model using the implementation proposed by Gaiser et. Al. (2019)}.

The prediction error was quantified using the mean Average Precision (MAP) metric and the results were as follows: 
The dataset efficiently represented two of the major weed groups: broad-leaved weeds and narrow-leaved weeds. 
100 training epochs were run and a mean pressure value (mAP: 0.92755) was obtained over the validation set. The mAP values per species are shown in Table 1.
Discrimination between species with higher frequency and invasiveness in tomato crops in Spain, which are controlled with different types of herbicides.
Discrimination between species within the same family.

## Conclusion

The present work shows that automatic detection of the main weeds affecting tomato crop production in Spain is possible under real growing conditions. The precision values obtained are sufficiently high to perform effective selective controls. In addition, the obtained results of discrimination between species within the same family show a great potential for the identification of species with herbicide resistance. This weed species detection method based on Object Detection Neural Networks presents promising results not only for weed vs. crop selective controls, but also for weed species under selective controls.

## References
<ul>
<li> EPPO European and Mediterranean Plant Protection Organization code system, http://eppt.eppo.org/, last accessed 1 December 2020; EPPO Plant Protection Thesaurus. </li>
<li> FERNÁNDEZ-QUINTANILLA, C.; PEÑA, J.M.; ANDÚJAR, D.; DORADO, J.; RIBEIRO, A.; LÓPEZ-GRANADOS, F. 2018. Is the current state of the art of weed monitoring suitable for site-specific weed management in arable crops?, Weed Research, 58, 259–272. </li>
<li>  GAISER, H., DE VRIES, M., LACATUSU, V., & WILLIAMSON, A. 2019. fizyr/keras-retinanet 0.5. 1. Zenodo. </li>
<li> FOOD AND AGRICULTURAL ORGANIZATION (FAO) (2017). FAO Production year book, Rome, Italy; 2017.</li>
<li> LIN, T. Y., GOYAL, P., GIRSHICK, R., HE, K., & DOLLÁR, P. 2017. Focal loss for dense object detection. In Proceedings of the IEEE international conference on computer vision (pp. 2980-2988).</li>
<li> PADILLA, R., NETTO, S. L., & DA SILVA, E. A. 2020. A survey on performance metrics for object-detection algorithms. In 2020 International Conference on Systems, Signals and Image Processing (IWSSIP) (pp. 237-242). IEEE.</li>
<li> PÉREZ-ORTIZ, M.; PEÑA, J.M.; GUTIÉRREZ, P.A.; TORRES-SÁNCHEZ, J.; HERVÁS-MARTÍNEZ, C.; LÓPEZ-GRANADOS, F. 2016. Selecting patterns and features for between- and within- crop-row weed mapping using UAV-imagery. Expert Systems .</li>
<li> TANGET, J. L., CHEN, X. Q., MIAO, R. H., & WANG, D. 2016. Weed detection using image processing under different illumination for site-specific areas spraying. Computers and Electronics in Agriculture, 122, 103-111.</li>
<li> TZUTALIN, D. 2015. LabelImg. Git code.</li>
</ul>

