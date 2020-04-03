
---

#### [Template/Atlas](templates_and_atlases.md) &nbsp;  - &nbsp;  [Versatile](versatile_tools.md) &nbsp;  - &nbsp;  [Structural](pipelines_structural.md) &nbsp;  - &nbsp;  [fMRI](pipelines_fmri.md) &nbsp;  - &nbsp;  [Diffusion](pipelines_diffusion.md) &nbsp;  - &nbsp;  [Software packages](software_packages.md)   

---    

# Templates and atlases

## Overview     
- [D99](templates_and_atlases2.md#D99)     
- [NMT v1.3](templates_and_atlases2.md#NMTv1.3)     
- [NMT v2.0](templates_and_atlases2.md#NMTv2.0)

<br>     

## Details

<a name="D99"></a>
### D99 Template and Atlas       
**Authors**         : Saleem KS, Reveley C, Gruslys A, Ye FQ, Glen D, Samaha J, Russ BE, Saad Z, Seth AK, Leopold DA	     
**Description**     : Digital version of the Saleem and Logothetis atlas with a newer, higher quality D99 surrogate MRI template. Integrated into AFNI/SUMA software.                                         
**Documentation**   : [AFNI site](https://afni.nimh.nih.gov/Macaque)     
**Link**            : [https://afni.nimh.nih.gov/pub/dist/atlases/macaque](https://afni.nimh.nih.gov/pub/dist/atlases/macaque/)    
**Language**        : NIFTI format     
**Publication**     : [Reveley et al. (2016)](https://doi.org/10.1093/cercor/bhw248)                     
**Communication**   : [email](mailto:kadharbatcha.saleem.ctr@usuhs.edu), [AFNI message board](https://afni.nimh.nih.gov/afni/community/board/list.php?1)    
**Restrictions**    : None

<a name="NMTv1.3"></a>
### NMT v1.3 (NIMH Macaque Template - version 1.3)       
**Authors**         : Adam Messinger, Benjamin Jung, Jakob Seidlitz, Paul Taylor, Daniel Glen	             
**Description**     : A volumetric template of the rhesus macaque created by nonlinear averaging of T1-weighted anatomical MRIs from multiple adult monkeys. Surface files are included. Version 1.3 updates include: an improved mapping of the D99 atlas, improved brain masking and normalization, and files that are defined in a common template space (NMT space), using the short data type for improved storage efficiency.                                   
**Documentation**   : [Github](https://github.com/jms290/NMT/blob/master/NMT_v1.3/README.md)     
**Link**            : [Github](https://github.com/jms290/NMT/tree/master/NMT_v1.3)    
**Language**        : Volumetric files are in NIFTI (.nii) format, while surface files are in GIFTI (.gii) format. Scripts for processing single subjects rely on bash shell and AFNI. Some scripts also require ANTs.                        
**Publication**     : Seidlitz, J., Sponheim, C., Glen, D., Ye, F.Q., Saleem, K.S., Leopold, D.A., Ungerleider, L., Messinger, A. A population MRI brain template and analysis tools for the macaque. NeuroImage 170:121-131 (2018). [https://doi.org/10.1016/j.neuroimage.2017.04.063](https://doi.org/10.1016/j.neuroimage.2017.04.063)                       
**Communication**   : Through the GitHub repo or via email to [Dr. Adam Messinger](mailto:Adam.Messinger@nih.gov)                       
**Restrictions**    : To use the NMT_v1.3 cite the above article:  [Seidlitz et al., (2018)](https://doi.org/10.1016/j.neuroimage.2017.04.063). To use the D99 atlas cite [Reveley et al. (2016)](https://doi.org/10.1093/cercor/bhw248).

<a name="NMTv2.0"></a>
### NMT 2.0 Templates (NIMH Macaque Template - version 2.0)           
**Authors**         : Adam Messinger, Benjamin Jung, Jakob Seidlitz, Paul Taylor, Daniel Glen    	             
**Description**     : A collection of volumetric templates of the rhesus macaque created by nonlinear averaging of T1-weighted anatomical MRIs from multiple adult monkeys.  Surface files are included. The NMT 2.0 provides increased flexibility in macaque group analysis by providing symmetric and asymmetric templates. Both templates are available with an expanded, full head field of view.  The templates are available in both AC-PC orientation and in Horsley-Clarke stereotaxic orientation. Updates to the templates include:  an improved mapping of the D99 atlas, improved brain masking and normalization, and files that are defined in a common template space (NMT space), using the short data type for improved storage efficiency.                                   
**Documentation**   : TBD     
**Link**            : TBD    
**Language**        : Volumetric files are in NIFTI (.nii) format, while surface files are in GIFTI (.gii) format. Scripts for processing single subjects rely on bash shell and AFNI. Some scripts also require ANTs.                        
**Publication**     : TBD                       
**Communication**   : Through the GitHub repo or via email to [Dr. Adam Messinger](mailto:Adam.Messinger@nih.gov)         
**Restrictions**    : Usage requires citation of this article: TBD
