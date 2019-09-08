## Welcome to PRIME-RE
### The PRIMatE Research Exchange

The preprocessing and analysis of nonhuman primate (NHP) magnetic resonance imaging (MRI) data presents some unique challenges.
PRIME-RE aims to provide a description of the main difficulties and the existing solutions associated with each of the processing steps commonly performed on NHP MRI data.
PRIME-RE is maintained and curated by members of the [PRIME-DE consortium](http://fcon_1000.projects.nitrc.org/indi/indiPRIME.html). 

![logo](images/social_preview_image.png)

### [Structural preprocessing](#structpreproc)
  
  - [What is it about?](#description)
  - [Issues linked to NHP imaging](#issues)
  - [Steps](#steps)
      - [Preparation of data (Cropping, deoblique…)](#preparation)
      - [Registration to template](#registration)
      - [Brain extraction / skull stripping](#extraction)
      - [Segmentation (GM, WM, CSF? Subcortical?bone, non brain soft tissue? air?)](#segmentation)
      - [Surface generation](#surf)
      - [Morphometry measures (thickness, curvature etc)](#measures)
      
  - [Pipelines Reviews](pipelines/pipelines_reviews.md#links)  
    &rarr; Direct Access:
     - [Chris' notebook html](structural_preprocessing/surfaces_and_flatmaps_notebook/Surfaces_and_Flatmaps.html) - [Download Chris' notebook](structural_preprocessing/surfaces_and_flatmaps_notebook/Surfaces_and_Flatmaps.ipynb)
     - [macapype](https://github.com/BastienCagna/macapype)
  - [Communication](structural_preprocessing/data_preparation.md#communication)
   

### [fMRI preprocessing](functional_preprocessing/)


<a name="structpreproc"></a> 
# Structural preprocessing
<a name="description"></a> 
## What is it about?
Several steps to obtain a segmented brain with possibility to create surfaces

<a name="issues"></a> 
## Issues specific to NHP imaging
- non standard orientation: sphinx position, oblique orientation
<p align="center"><img src="images/misorientation.png" width="400"></p>
- strong intensity bias due to a huge variety of coils used
<p align="center"><img src="images/bias.png" width="250"></p>
- large FOV / non brain tissue
<p align="center"><img src="images/non_brain.png" width="250"></p>

<a name="steps"></a> 
## Steps
<a name="steps"></a> 
### Preparation of data (Cropping, deoblique…)

- **What is is about?**

- **Solutions**
<a name="registration"></a>  
### Registration to template
<a name="extraction"></a> 
### Brain extraction / skull stripping
<a name="segmentation"></a> 
### Segmentation (GM, WM, CSF? Subcortical?bone, non brain soft tissue? air?)
<a name="surf"></a> 
### Surface generation
<a name="measures"></a> 
### Morphometry measures (thickness, curvature etc)

<a name="links"></a> 
## Links to pipelines

<a name="communication"></a> 
## Communication
Link to the communication channel for your project. You can, for example, create a [Mattermost channel](https://mattermost.brainhack.org/brainhack/channels/prime-de) for your project inside the Brainhack community, and include a Mattermost badge <br/>[![Mattermost30px](https://user-images.githubusercontent.com/6297454/64487455-57d52280-d23b-11e9-9dd4-e6d75bad44fc.png)](https://mattermost.brainhack.org/brainhack/channels/prime-de) to invite people to Brainhack Mattermost, where they can then find and join your channel.  
Or create a community on [gitter](https://gitter.im/) and link to the chat by including a Gitter badge linking to your community 
[![Gitter chat](https://badges.gitter.im/gitterHQ/gitter.png)](https://gitter.im/yourRoom/Lobby#)





