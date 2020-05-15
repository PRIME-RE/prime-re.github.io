
---

##### [Template/Atlas](templates_and_atlases.md) &nbsp;  - &nbsp;  [General](pipelines_general.md) &nbsp;  - &nbsp;  [Structural](pipelines_structural.md) &nbsp;  - &nbsp;  [fMRI](pipelines_fmri.md) &nbsp;  - &nbsp;  [Diffusion](pipelines_diffusion.md) &nbsp;  - &nbsp;  [Data](data_sharing.md) &nbsp;  - &nbsp; [Software packages](software_packages.md)       

---    

# Structural MRI

## Overview     
- [AFNI @animal_warper](pipelines_structural.md#afni-animal_warper)   
- [BrainBox](pipelines_structural.md#brainbox)
- [CIVET-macaque](pipelines_structural.md#civet-macaque)   
- [C-PAC](pipelines_structural.md#c-pac-the-configurable-pipeline-for-the-analysis-of-connectomes)       
- [Macapype](pipelines_structural.md#macapype)     
- [MR Comparative Anatomy Toolbox (MrCat)](pipelines_structural.md#mr-comparative-anatomy-toolbox-mrcat)
- [NHP-Freesurfer](pipelines_structural.md#nhp-freesurfer)
- [NHP-pycortex](pipelines_structural.md#nhp-pycortex)
- [Precon_all](pipelines_structural.md#precon_all)
- [PREEMACS](pipelines_structural.md#preemacs)
- [Reorient](pipelines_structural.md#reorient)
- [Thresholdmann](pipelines_structural.md#thresholdmann)     
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

### BrainBox       
**Authors**         : Katja Heuer & Roberto Toro                  
**Description**     : A Web application for visualising, annotating & segmenting 3D brain imaging data in real time, collaboratively.   
**Documentation**   : [3 min video](https://www.youtube.com/watch?v=kwsLoVKnw24)     
**Link**            : [https://brainbox.pasteur.fr](https://brainbox.pasteur.fr)       
**Language**        : JavaScript, HTML, CSS                                                                         
**Publication**     : [Open Neuroimaging Laboratory](https://doi.org/10.3897/rio.2.e9113)                                      
**Communication**   : [Mattermost](https://mattermost.brainhack.org/brainhack/channels/brainbox) or [GitHub issues](https://github.com/neuroanatomy/BrainBox/issues)    
**Restrictions**    : Developed and tested in Chrome Browser         

### CIVET-macaque       
**Authors**         : Claude Lepage, Konrad Wagstyl, Ben Jung, Jakob Seidlitz, Caleb Sponheim, Leslie Ungerleider, Xindi Wang, Alan Evans, Adam Messinger                   
**Description**     : Fully automated structural MRI pipeline using the NIH Macaque Template (NMT).  Performs registration, segmentation, and surface reconstruction of T1-weighted anatomical scans.  Provides quality control images and results.    
**Documentation**   : [Github](https://github.com/aces/CIVET_Full_Project)     
**Link**            : [https://github.com/aces/CIVET_Full_Project](https://github.com/aces/CIVET_Full_Project)    
**Language**        : C, minc, NIFTI/GIFTI.  Binaries available on GitHub.                                          
**Publication**     : forthcoming                                                                                       
**Communication**   : tbd               
**Restrictions**    : Cite the forthcoming paper          

### C-PAC: The Configurable Pipeline for the Analysis of Connectomes
**Authors**         : Steven Giavasis, Cameron Craddock, Michael Milham                                                               
**Description**     : The Configurable Pipeline for the Analysis of Connectomes (C-PAC) is a configurable, open-source, Nipype-based, automated processing pipeline for resting state functional MRI (R-fMRI) data, for use by both novice and expert users. It is designed and tested for use with human data (all ages), as well as with non-human primate and rodent data.                   
**Documentation**   : [http://fcp-indi.github.io/](http://fcp-indi.github.io/)                                      
**Link**            : [Quick-Start](http://fcp-indi.github.io/docs/user/quick.html)               
**Language**        : Python                                                  
**Publication**     : [Craddock et al. (2013)](https://www.frontiersin.org/10.3389/conf.fninf.2013.09.00042/event_abstract)         
**Communication**   : [C-PAC Forum](https://groups.google.com/forum/#!forum/cpax_forum)                                             
**Restrictions**    : None      

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

### Precon_all     
**Authors**         : R. Austin Benn, Ting Xu                                                                             
**Description**     : precon_all is an anatomical surface reconstruction pipeline that can be used with Non-Human Primates, and other large animals including pigs, dogs, and potentially many more. The pipeline can be easily modified to work on most species with a reasonable T1 image by simply providing 5 masks. The pipeline provides both freesurfer and HCP compatible outputs in native image space. Group average surfaces and spherical registration templates can also be created within the precon_all framework.                   
**Documentation**   : [precon_all](https://github.com/recoveringyank/precon_all)                                    
**Link**            : [GitHub Link](https://github.com/recoveringyank/precon_all)        
**Language**        : shell                                                       
**Publication**     : In preparation                                                                                       
**Communication**   : [Email](mailto:rabbenn@cnic.es)                                            
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

### Reorient     
**Authors**         : Katja Heuer & Roberto Toro                                                                                     
**Description**     : A Web tool for reorienting and cropping MRI data               
**Documentation**   : [Readme in the GitHub repo](https://github.com/neuroanatomy/reorient)                                             
**Link**            : [GitHub Link](https://neuroanatomy.github.io/reorient)      
**Language**        : JavaScript, HTML, CSS                                                       
**Publication**     : Work in progress                                                                                       
**Communication**   : [GitHub issues](https://github.com/neuroanatomy/reorient/issues)                                                 
**Restrictions**    : Developed and tested in Chrome Browser  

### Thresholdmann     
**Authors**         : Katja Heuer & Roberto Toro                                                                                     
**Description**     : A Web tool for interactively creating adaptive thresholds to segment nifti images               
**Documentation**   : [Readme in the GitHub repo](https://github.com/neuroanatomy/thresholdmann)                                        
**Link**            : [GitHub Link](https://neuroanatomy.github.io/thresholdmann)      
**Language**        : JavaScript, HTML, CSS                                                       
**Publication**     : Work in progress                                                                                       
**Communication**   : [GitHub issues](https://github.com/neuroanatomy/thresholdmann/issues)                                     
**Restrictions**    : Developed and tested in Chrome Browser  

### UNet model for skull stripping and brain masks of anatomical images from PRIME-DE         
**Authors**         : Xindi Wang, Ting Xu                                                                             
**Description**     : The preprocessed brain masks of T1w images for all macaque monkeys from PRIME-DE. A convolutional network - UNet model was used to generate the brain mask for T1w images. The UNet model was initially trained in a large human sample and upgraded with a few macaque data. With a small macaque training sample (N=1-2), the UNet model achieves a decent performance of brain extraction with a minimal processing time (GPU: ~20s, CPU: 2-10 min).                       
**Documentation**   : [UNet model on PRIME-DE](https://github.com/TingsterX/PRIME-DE/tree/master/BrainExtraction)    
**Link**            : [UNet model](https://github.com/to-be-release), [code](https://github.com/to-be-release), [preprocessed brain masks](https://github.com/TingsterX/PRIME-DE/tree/master/BrainExtraction)             
**Language**        : Python                                                       
**Publication**     : [In prepartion](https://github.com/to-be-release)                                 
**Communication**   : [GitHub profile](https://github.com/TingsterX)                                                 
**Restrictions**    : GNU   
