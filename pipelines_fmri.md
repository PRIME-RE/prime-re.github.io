
---

##### [Template/Atlas](templates_and_atlases.md) &nbsp;  - &nbsp;  [General](pipelines_general.md) &nbsp;  - &nbsp;  [Structural](pipelines_structural.md) &nbsp;  - &nbsp;  [fMRI](pipelines_fmri.md) &nbsp;  - &nbsp;  [Diffusion](pipelines_diffusion.md) &nbsp;  - &nbsp;  [Data](data_sharing.md) &nbsp;  - &nbsp; [Software packages](software_packages.md)      

---    

# fMRI

## Overview
- [afni_proc.py](pipelines_fmri.md#afni_procpy)       
- [C-PAC](pipelines_fmri.md#c-pac-the-configurable-pipeline-for-the-analysis-of-connectomes) 
- [MR Comparative Anatomy Toolbox (MrCat)](pipelines_fmri.md#mr-comparative-anatomy-toolbox-mrcat)
- [NeuroElf](pipelines_fmri.md#neuroelf) 
- [NHP-BIDS](pipelines_fmri.md#nhp-bids) 
- [NHP-pycortex](pipelines_fmri.md#nhp-pycortex) 
- [Pypreclin](pipelines_fmri.md#pypreclin) 

<br>

## Details

### afni_proc.py       
**Authors**         : Rick Reynolds, Paul Taylor, Daniel Glen, Gang Chen, Bob Cox 	             
**Description**     : FMRI analysis pipeline tool in AFNI.  This widely used, general purpose and flexible tool for creating a full, single subject FMRI processing stream can be used for macaque analyses. This program creates fully commented, single subject processing scripts for all FMRI study designs (task, resting state, naturalistic, etc.) and for either volumetric- or surface-based analyses. The typical goal is to create volumes of aligned response magnitudes (stimulus beta weights from a GLM) to use as input for a group analysis.        
**Documentation**   : [AFNI site](https://afni.nimh.nih.gov/pub/dist/doc/program_help/afni_proc.py.html)     
**Link**            : [https://afni.nimh.nih.gov](https://afni.nimh.nih.gov/)    
**Language**        : python, tcsh, C, AFNI                                                       
**Publication**     : TBD        
**Communication**   : [AFNI message board](https://afni.nimh.nih.gov/afni/community/board/list.php?1)               
**Restrictions**    : None 


### C-PAC: The Configurable Pipeline for the Analysis of Connectomes
**Authors**         : Steven Giavasis, Cameron Craddock, Michael Milham                                                               
**Description**     : The Configurable Pipeline for the Analysis of Connectomes (C-PAC) is a configurable, open-source, Nipype-based, automated processing pipeline for resting state functional MRI (R-fMRI) data, for use by both novice and expert users. It is designed and tested for use with human data (all ages), as well as with non-human primate and rodent data.                   
**Documentation**   : [http://fcp-indi.github.io/](http://fcp-indi.github.io/)                                      
**Link**            : [Quick-Start](http://fcp-indi.github.io/docs/user/quick.html)               
**Language**        : Python                                                  
**Publication**     : [Craddock et al. (2013)](https://www.frontiersin.org/10.3389/conf.fninf.2013.09.00042/event_abstract)         
**Communication**   : [C-PAC Forum](https://groups.google.com/forum/#!forum/cpax_forum)                                             
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

### NeuroElf
**Authors**         : Jochen Weber                                                                             
**Description**     : NeuroElf is a powerful Matlab-based toolbox for working with neuroimaging data.                  
**Documentation**   : [NeuroElf website](http://neuroelf.net/)                                     
**Link**            : [http://neuroelf.net/](http://neuroelf.net/)         
**Language**        : Matlab                                                  
**Publication**     : [http://neuroelf.net/](http://neuroelf.net/)                                                                                        
**Communication**   : [GitHub](https://github.com/neuroelf/neuroelf-matlab)                                            
**Restrictions**    : See [license](http://neuroelf.net/wiki/doku.php?id=neuroelf_license)    


### NHP-BIDS     
**Authors**         : Chris Klink                                                                             
**Description**     : This pipeline uses NiPype to organize and (pre)process NHP-MRI data in accordance with BIDS. It covers the entire pipeline from exporting the data from the scanner, via motion correction and warping, to running a GLM.              
**Documentation**   : [GitHub WIKI](https://github.com/VisionandCognition/NHP-BIDS/wiki)                                                 
**Link**            : [GitHub link](https://github.com/VisionandCognition/NHP-BIDS/tree/public)         
**Language**        : Python, Shell                                                       
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

### Pypreclin
**Authors**         : Jordy Tasserie, Antoine Grigis, Lynn Uhrig, Morgan Dupont, Alexis Amadon and Béchir Jarraya.                 
**Description**     : Pypreclin is a flexible and automatic tool for preprocessing of macaque fMRI data available for the growing community of primate fMRI.                                   
**Documentation**   : [GitHub](https://github.com/neurospin/pypreclin)      
**Link**            : The Python project can be found on [GitHub](https://github.com/neurospin/pypreclin), on the Python Package Index [PyPI](https://pypi.org/project/pypreclin/) for easy installation and upgrading, and also as a [Singularity container](biodev.cea.fr/pypreclin/pypreclin-ubuntu.simg).   <br> 
**Language**        : Python           
**Publication**     : Tasserie J, Grigis A, Uhrig L, Dupont M, Amadon A, Jarraya B. Neuroimage. 2019 Nov 16:116353. doi: 10.1016/j.neuroimage.2019.116353. [Pubmed](https://www.ncbi.nlm.nih.gov/pubmed/31743789) - [Journal website](https://www.sciencedirect.com/science/article/pii/S1053811919309449?via%3Dihub)  <br>
**Communication**   : [GitHub profile](https://github.com/AGrigis)         
**Restrictions**    : Please cite the related publication   
