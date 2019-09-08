## Welcome to PRIME-RE
### The PRIMatE Research Exchange

The preprocessing and analysis of nonhuman primate (NHP) magnetic resonance imaging (MRI) data presents some unique challenges.
PRIME-RE aims to provide a description of the main difficulties and list the existing solutions associated with each of the processing steps commonly performed on NHP MRI data.
PRIME-RE is maintained and curated by members of the [PRIME-DE consortium](http://fcon_1000.projects.nitrc.org/indi/indiPRIME.html). 

![logo](images/social_preview_image.png)

#### How to contribute ?
Send new content by using [this template file](New_Resource_Template.md) to create a new issue [here](https://github.com/PRIME-RE/prime-re.github.io/issues)! You can also join our communication channel around the Primate Data Exchange on the Brainhack community on [PRIME-DE Mattermost](https://mattermost.brainhack.org/brainhack/channels/prime-de) or specifically for this Primate Resource Exchange via on [PRIME-RE Mattermost](https://mattermost.brainhack.org/brainhack/channels/prime-re) .

### [Atlases](#atlases)

### [Structural preprocessing](#structpreproc)
  
  - [What is it about?](#structdescription)
  - [Issues linked to NHP imaging](#structissues)
  - [Steps](#structsteps)
      - [Preparation of data (Cropping, deoblique…)](#structpreparation)
      - [Registration to template](#structregistration)
      - [Brain extraction / skull stripping](#structextraction)
      - [Segmentation (GM, WM, CSF? Subcortical?bone, non brain soft tissue? air?)](#structsegmentation)
      - [Surface generation](#structsurf)
      - [Morphometry measures (thickness, curvature etc)](#structmeasures)
      
  - [Pipelines Reviews](#structlinks)  
  - [Communication](structural_preprocessing/data_preparation.md#communication)
   

### [fMRI preprocessing](#funcpreproc)


<a name="atlases"></a>
# Atlases
Comming soon...


<a name="structpreproc"></a> 
# Structural preprocessing
<a name="structdescription"></a> 
## What is it about?
Several steps to obtain a segmented brain with possibility to create surfaces

<a name="structissues"></a> 
## Issues specific to NHP imaging
- non standard orientation: sphinx position, oblique orientation
<p align="center"><img src="images/misorientation.png" width="400"></p>
- strong intensity bias due to a huge variety of coils used
<p align="center"><img src="images/bias.png" width="250"></p>
- large FOV / non brain tissue
<p align="center"><img src="images/non_brain.png" width="250"></p>

<a name="structsteps"></a> 
## Steps
<a name="structpreparation"></a> 
### Preparation of data (Cropping, deoblique…)

- **What is is about?**

- **Solutions**


<a name="structregistration"></a>  
### Registration to template

<a name="structextraction"></a> 
### Brain extraction / skull stripping

<a name="structsegmentation"></a> 
### Segmentation (GM, WM, CSF? Subcortical?bone, non brain soft tissue? air?)

<a name="structsurf"></a> 
### Surface generation

<a name="structmeasures"></a> 
### Morphometry measures (thickness, curvature etc)

<a name="structlinks"></a> 
## Pipelines Reviews
### Chris' notebook
(description should be here)
[Chris' notebook html](structural_preprocessing/surfaces_and_flatmaps_notebook/Surfaces_and_Flatmaps.html)  - [Download Chris' notebook](structural_preprocessing/surfaces_and_flatmaps_notebook/Surfaces_and_Flatmaps.ipynb)
### Macapype
Python package that provides pipelines for NHP anatomical preprocessing using Nipype.
[github repository](https://github.com/BastienCagna/macapype)

| Name | Short description | Links |
| --- | --- | --- |
| Surfaces and flatmaps | Jupyter notebook that ... | [view](structural_preprocessing/surfaces_and_flatmaps_notebook/Surfaces_and_Flatmaps.html) - [download](structural_preprocessing/surfaces_and_flatmaps_notebook/Surfaces_and_Flatmaps.ipynb) |
| Macapype | Python package for anatomical preprosessing using Nipype. | [github](https://github.com/BastienCagna/macapype) - [details](https://github.com/PRIME-RE/prime-re.github.io/issues/7) |

<a name="funcpreproc">
# Functional Preprocessing









