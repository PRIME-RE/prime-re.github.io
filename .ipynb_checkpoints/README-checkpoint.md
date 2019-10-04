# Welcome to PRIME-RE
## The PRIMatE Research Exchange

The preprocessing and analysis of nonhuman primate (NHP) magnetic resonance imaging (MRI) data presents some unique challenges. Over the years, many laboratories and researchers have created their own custom solutions to many of these problems. PRIME-RE aims to provide a overview of the main difficulties and curate a collection of solutions that currently exist within the broader NHP-MRI communnity for specific processing steps that are commonly performed on NHP MRI data. Since this is a cimmunity effort, we strongly encourage you to contribute your workflows and pipelines. 

PRIME-RE is maintained by members of the [PRIME-DE consortium](http://fcon_1000.projects.nitrc.org/indi/indiPRIME.html). 

![logo](images/social_preview_image.png)

### How to contribute ?
Send new content by using [this template file](New_Resource_Template.md) to create a new issue [here](https://github.com/PRIME-RE/prime-re.github.io/issues)! You can also join our communication channel around the Primate Data Exchange on the Brainhack community on [PRIME-DE Mattermost-channel](https://mattermost.brainhack.org/brainhack/channels/prime-de) or specifically for this Primate Resource Exchange via on [PRIME-RE Mattermost-channel](https://mattermost.brainhack.org/brainhack/channels/prime-re) .

### Wiki
A [wiki](https://github.com/PRIME-RE/prime-re.github.io/wiki/Structural-preprocessing) have been set up to share knowledge about NHP MRI acquisition and image processing. Anyone can share knowledge and experience (problems with solutions, fixes, tricks...).

<a name="summary"></a> 
### Resources
- [Templates and Atlases](#atlases)
    - [Macaque species](#macaque_atlases)
    - [Marmoset species](#marmoset_atlases)
    - [Other species](#other_atlases)

- [Pipelines](#pipelines)
    - [Structural preprocessing](#structpreproc)
    - [fMRI preprocessing](#funcpreproc)

<a name="atlases"></a>
# Templates and atlases
**Template:** A standard brain, typically used for registering multiple individuals into a common coordinate space. This space can be either volumetric (3D coordinates system), surface-based (mesh), or a combination of both.

**Atlas:** a percellation of the brain into areas, often provided in a specific template space. Atlases are typically used for defining regions-of-interest (ROIs) or for identifying the location of activation sites.

For human MRI, the [MNI template](http://www.bic.mni.mcgill.ca/ServicesAtlases/ICBM152NLin2009) serves as the community standard volumetric template. Its integration into most major software packages makes it easy for researchers to register their results to MNI space and facilitates data-sharing, cross-study comparisons and metanalyses. Most human brain atlases are also provided in MNI space. For surface-based analysis the [FsAverage](https://surfer.nmr.mgh.harvard.edu/fswiki/FsAverage) (freesurfer average) template serves the same purpose.

When it comes to NHP neuroimaging though, there are two compications:
1. The usage of multple species creates the need for species-specific templates
2. Even for the most commonly imaged species (macaques and marmosets), multiple templates are available, with no single one of them adopted as the go-to community standard.

Below, we provide a non-exhaustive list of existing templates and atlases.

<a name="macaque_atlases"></a>
## Macaque species

| Template Name | Species | T1 Resolution | Number of monkeys | Accompanying Atlas | Volume format | Surface format | Links |
| --- | --- | --- | --- | --- | --- | --- | --- |
| NMT | _Macaca mulatta_ | 0.25 mm<sup>3</sup> | 31 | Registered to D99-SL | NIFTI | GIFTI | [reference](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC5660669/) [download](https://github.com/jms290/NMT) |
| D99 | _Macaca mulatta_ | 0.25 mm<sup>3</sup> | 1 | Saleem Logothetis (D99-SL) | NIFTI | GIFTI | [reference](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC6075609/) [download](https://afni.nimh.nih.gov/Macaque) |
| INIA19 | _Macaca mulatta_ | 0.50 mm<sup>3</sup> | 19 | Neuromaps | NIFTI | None | [reference](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3515865/) [download](https://www.nitrc.org/projects/inia19/https://www.nitrc.org/projects/inia19/) |
| MNI macaque | _Macaca fascicularis_ and _mulatta_ | 0.25 mm<sup>3</sup> | 18 and 7 respectively | Paxinos | MINC and NIFTI | None | [reference](https://www.ncbi.nlm.nih.gov/pubmed/21256229) - [download](http://www.bic.mni.mcgill.ca/ServicesAtlases/Macaque) |
| Yerkes19 | _Macaca mulatta_ | 0.50 mm<sup>3</sup> | 19 | registered to F99 | NIFTI and MGZ | GIFTI and MGZ | [reference 1](https://www.pnas.org/content/115/22/E5183) [reference 2](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3500860/) [download 1](https://balsa.wustl.edu/reference/show/976nz) [download 2](https://github.com/Washington-University/NHPPipelines) |
| Japanese macaque atlas| _Macaca fuscata_ | 0.50 mm<sup>3</sup> | 16 | None | ANALYZE | None | [reference](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3221050/) [download](https://brainatlas.brain.riken.jp/jm/modules/xoonips/listitem.php?index_id=9) |
| 112RM-SL | _Macaca mulatta_ | 0.50 mm<sup>3</sup> | 112 | registered to D99-SL and F99 | NIFTI | None | [reference](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC2659879/) [download](http://brainmap.wisc.edu/pages) currently unavailable |
| UNC-Emory developmental atlas | _Macaca mulatta_ | 0.60 mm<sup>3</sup> | 40 | registered to multiple | NRRD | None | [reference](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC5222830//) [download](https://www.nitrc.org/projects/macaque_atlas/) |

<a name="marmoset_atlases"></a>
## Marmoset species

<a name="other_atlases"></a>
## Other species

<a name="pipelines"></a> 
# Pipelines
<a name="structpreproc"></a> 
## Structural preprocessing
[go up](#summary)
### Overview

| Name | Short description | Links |
| --- | --- | --- |
| Surfaces and flatmaps | Jupyter notebook that ... | [view](structural_preprocessing/surfaces_and_flatmaps_notebook/Surfaces_and_Flatmaps.html) - [download](structural_preprocessing/surfaces_and_flatmaps_notebook/Surfaces_and_Flatmaps.ipynb) |
| Macapype | Python package for anatomical preprosessing using Nipype. | [github](https://framagit.org/mars-hackat2019/anat-mri-pipeline/macapype) - [details](https://github.com/PRIME-RE/prime-re.github.io/issues/7) |

### Details
#### Chris' notebook
(description should be here)
[Chris' notebook html](structural_preprocessing/surfaces_and_flatmaps_notebook/Surfaces_and_Flatmaps.html)  - [Download Chris' notebook](structural_preprocessing/surfaces_and_flatmaps_notebook/Surfaces_and_Flatmaps.ipynb)
#### Macapype
Python package that provides pipelines for NHP anatomical preprocessing using Nipype.
[framagit repository](https://framagit.org/mars-hackat2019/anat-mri-pipeline/macapype)


<a name="funcpreproc"></a>
## Functional Preprocessing
[go up](#summary)
### Overview
Nothing here. Need of contributions ! :)

| Name | Short description | Links |
| --- | --- | --- |
