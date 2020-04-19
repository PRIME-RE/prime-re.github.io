
---

#### [Template/Atlas](templates_and_atlases.md) &nbsp;  - &nbsp;  [Versatile](versatile_tools.md) &nbsp;  - &nbsp;  [Structural](pipelines_structural.md) &nbsp;  - &nbsp;  [fMRI](pipelines_fmri.md) &nbsp;  - &nbsp;  [Diffusion](pipelines_diffusion.md) &nbsp;  - &nbsp;  [Software packages](software_packages.md)    

---    

# Structural MRI

## Overview     
- [AFNI @animal_warper](pipelines_structural.md#afni-animal_warper)     
- [Macapype](pipelines_structural.md#macapype)     
- [MR Comparative Anatomy Toolbox (MrCat)](pipelines_structural.md#mr-comparative-anatomy-toolbox-mrcat)
- [NHP-Freesurfer](pipelines_structural.md#nhp-freesurfer)
- [NHP-pycortex](pipelines_structural.md#nhp-pycortex)
- [PREEMACS](pipelines_structural.md#preemacs)
- [UNet model for skull stripping for PRIME-DE](pipelines_structural.md#unet-model-for-skull-stripping-and-brain-masks-of-anatomical-images-from-prime-de)

<br>     

## Details

### AFNI @animal_warper       
**Authors**         : Daniel Glen, Paul Taylor, Adam Messinger, Benjamin Jung, Jakob Seidlitz                 
**Description**     : Nonlinearly aligns an MRI dataset to a template. The reverse transformation can be used to produce a skullstripped (brain-only) version of the native scan, segmentation/atlas info in the native space, and surfaces for each atlas region. The computed transformations between the anatomical scan and the template is provided for use with FMRI pipeline tools like afni_proc.py.                                   
**Documentation**   : [Online doc](https://afni.nimh.nih.gov/pub/dist/doc/program_help/@animal_warper.html)     
**Link**            : [AFNI](https://afni.nimh.nih.gov/)    
**Language**        : tcsh, python, C, AFNI                                                                         
**Publication**     : TBD                                                                                       
**Communication**   : [AFNI message board ](https://afni.nimh.nih.gov/afni/community/board/list.php?1) 

### Macapype       
**Authors**         : Bastien Cagna, David Meunier, Kep kee Loh, Julien Sein, & Régis Trapeau                 
**Description**     : Python package for NHP anatomical MRI segmentation using Nipype.                               
**Documentation**   : [Online doc](https://macatools.github.io/macapype/index.html)     
**Link**            : [https://github.com/Macatools/macapype](https://github.com/Macatools/macapype)    
**Language**        : Python                                                                                  
**Publication**     : -                                                                                       
**Communication**   : [Post issue on GitHub website](https://github.com/Macatools/macapype/issues/new)               
**Restrictions**    : None                                                                                          

### MR Comparative Anatomy Toolbox (MrCat)       
**Authors**         : Rogier B. Mars, Lennart Verhagen, and the members and collaborators of the Cognitive Neuroecology Lab	             
**Description**     : A collection of tools for processing of multi-species neuroimaging data.                               
**Documentation**   : [Online doc](http://www.neuroecologylab.org)     
**Link**            : [www.neuroecologylab.org](http://www.neuroecologylab.org)    
**Language**        : shell, matlab                                                                                  
**Publication**     : [Mars et al. 2016](http://www.rbmars.dds.nl/pubs/Mars2016NBR.pdf), among others                        
**Communication**   : [www.neuroecologylab.org](http://www.neuroecologylab.org)                                           
**Restrictions**    : None   

### NHP-Freesurfer     
**Authors**         : Chris Klink                                                                             
**Description**     : Segmentation and surface generation of monkey brains using Freesurfer, the NMT template, and other tools. Jupyter Notebooks with documentation on how to generate surfaces and project results to it.            
**Documentation**   : Available in Jupyter notebook on GitHub                                                 
**Link**            : [GitHub link](https://github.com/VisionandCognition/NHP-Freesurfer/tree/public)         
**Language**        : Jupyter notebooks with Shell code                                                       
**Publication**     : -                                                                                       
**Communication**   : [GitHub profile](https://github.com/pcklink)                                            
**Restrictions**    : None                                                                                      

### NHP-pycortex     
**Authors**         : Chris Klink                                                                             
**Description**     : Import surfaces generated with [NHP-Freesurfer](pipelines_structural.md#NHP-Freesurfer) into a version of pycortex that is adapted for NHP use. This opens up the possibility of using pycortex to visualize fMRI results on the surface.                   
**Documentation**   : Available in Jupyter notebook on GitHub                                                 
**Link**            : [GitHub link](https://github.com/VisionandCognition/NHP-pycortex)         
**Language**        : Jupyter notebooks with Python 3                                                       
**Publication**     : -                                                                                       
**Communication**   : [GitHub profile](https://github.com/pcklink)                                            
**Restrictions**    : None              

### PREEMACS     
**Authors**         : Pamela Garcia-Saldivar, Arun Garimella, Eduardo A. Garza-Villarreal, Felipe Mendez, Luis Concha and Hugo Merchant                                                                                 
**Description**     : PREEMACS (pipeline for PREprocessing and Extraction of the MACaque brain Surface) is a pipeline to process raw structural images in order to obtain brain surfaces and cortical thickness, without requiring manual editing. PREEMACS has a modular design, with three modules running independently: Preprocessing, Quality Control and Brain Surface estimation based on FreeSurfer.   To evaluate the generalizability of our method, we tested PREEMACS on three different datasets of NHP images: PRIME-DE, UNC-Wisconsin Database and INB-UNAM.  Results showed accurate and robust automatic brain surface extraction in our INB-UNAM database and precise extraction in the UNC-Wisconsin and PRIME-DE databases for images that passed the quality control segment of our pipeline.                   
**Documentation**   : [PREEMACS](https://github.com/pGarciaS/PREEMACS/wiki)                                               
**Link**            : [GitHub Link](https://github.com/pGarciaS/PREEMACS)        
**Language**        : python, shell and matlab                                                       
**Publication**     : -                                                                                       
**Communication**   : [GitHub Profile](https://github.com/pGarciaS)                                            
**Restrictions**    : None  

### UNet model for skull stripping and brain masks of anatomical images from PRIME-DE         
**Authors**         : Xindi Wang, Ting Xu                                                                             
**Description**     : The preprocessed brain masks of T1w images for all macaque monkeys from PRIME-DE. A convolutional network - UNet model was used to generate the brain mask for T1w images. The UNet model was initially trained in a large human sample and upgraded with a few macaque data. With a small macaque training sample (N=1-2), the UNet model achieves a decent performance of brain extraction with a minimal processing time (GPU: ~20s, CPU: 2-10 min).                       
**Documentation**   : [UNet model on PRIME-DE](https://github.com/TingsterX/PRIME-DE/tree/master/BrainExtraction)    
**Link**            : [UNet model](https://github.com/to-be-release), [code](https://github.com/to-be-release), [preprocessed brain masks](https://github.com/TingsterX/PRIME-DE/tree/master/BrainExtraction)             
**Language**        : Python                                                       
**Publication**     : [In prepartion](https://github.com/to-be-release)                                 
**Communication**   : [GitHub profile](https://github.com/TingsterX)                                                 
**Restrictions**    : GNU   
