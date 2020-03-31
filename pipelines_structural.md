
---

#### [Template/Atlas](templates_and_atlases.md) &nbsp;  - &nbsp;  [Versatile](versatile_tools.md) &nbsp;  - &nbsp;  [Structural](pipelines_structural.md) &nbsp;  - &nbsp;  [fMRI](pipelines_fmri.md) &nbsp;  - &nbsp;  [Diffusion](pipelines_diffusion.md) &nbsp;  - &nbsp;  [Software packages](software_packages.md)    

---    

# Structural MRI

## Overview     
- [Macapype](pipelines_structural.md#macapype)     
- [MR Comparative Anatomy Toolbox (MrCat)](pipelines_structural.md#mr-comparative-anatomy-toolbox-mrcat)
- [NHP-Freesurfer](pipelines_structural.md#nhp-freesurfer)
- [NHP-pycortex](pipelines_structural.md#nhp-pycortex)
- [UNet model for skull stripping and brain masks of anatomical images from PRIME-DE](pipelines_structural.md#unet-model-for-skull-stripping-and-brain-masks-of-anatomical-images-from-prime-de)

<br>     

## Details

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

### UNet model for skull stripping and brain masks of anatomical images from PRIME-DE         
**Authors**         : Xindi Wang, Ting Xu                                                                             
**Description**     : The preprocessed brain masks of T1w images for all macaque monkeys from PRIME-DE. A convolutional network - UNet model was used to generate the brain mask for T1w images. The UNet model was initially trained in a large human sample and upgraded with a few macaque data. With a small macaque training sample (N=1-2), the UNet model achieves a decent performance of brain extraction with a minimal processing time (GPU: ~20s, CPU: 2-10 min).                       
**Documentation**   : [UNet model on PRIME-DE](https://github.com/TingsterX/PRIME-DE/tree/master/BrainExtraction)                       
**Link**            : [UNet model](https://github.com/to-be-release), [code](https://github.com/to-be-release), [preprocessed brain masks](https://github.com/to-be-release)             
**Language**        : Python                                                       
**Publication**     : [In prepartion](https://github.com/to-be-release)                                                                 
**Communication**   : GitHub repo, email: ting.xu @childmind.org                                                 
**Restrictions**    : GNU   
