<!-- This piece of code configures a dropdown button for resource categories. It should be present on every page where you want the button -->
<head><meta name="viewport" content="width=device-width, initial-scale=1"><style>
.dropbtn {background-color: #1e6bb8; color: white; padding: 16px; font-size: 1rem; border: none; cursor: pointer; width: 30rem}
.dropbtn:hover, .dropbtn:focus {background-color: #2980B9;}
.dropdown {position: relative; display: inline-block;}
.dropdown-content {display: none; position: absolute; background-color: #f1f1f1; min-width: 100%; overflow: auto; box-shadow: 0px 8px 16px 0px rgba(0,0,0,0.2); z-index: 1; text-align: center; font-size: 1rem;}
.dropdown-content a { color: black; padding: 12px 16px; text-decoration: none; display: block;}
.dropdown a:hover {background-color: #ddd;}
.show {display: block;}
.dropbtn + .dropbtn { margin-left: auto; }
@media screen and (min-width: 64em) { .dropbtn { max-width: 64rem; width: 40rem; padding: 0.75rem 1rem; } }
@media screen and (min-width: 42em) and (max-width: 64em) { .dropbtn { width: 30rem; padding: 0.6rem 0.9rem; font-size: 0.9rem; } }
@media screen and (max-width: 42em) { .dropbtn { display: block; width: 20rem; padding: 0.75rem; font-size: 0.9rem; }
.dropbtn + .dropbtn { margin-top: 1rem; margin-left: 0; } }
</style></head>
<!------------------------------------------------------------------------>

<!-- This is the actual button -->
<center><div class="dropdown">
  <button onclick="myFunction()" class="dropbtn">Select Resource Category</button>
  <div id="myDropdown" class="dropdown-content">
    <a href="templates_and_atlases">Templates & atlases</a>
    <a href="pipelines_general">General analysis</a>
    <a href="pipelines_structural">Structural analysis</a>
    <a href="pipelines_fmri">Functional analysis</a>
    <a href="pipelines_diffusion">Diffusion analysis</a>
    <a href="pipelines_cross-species">Cross-species analysis</a>
    <a href="data_sharing">Data sharing</a>
    <a href="software_packages">Software packages</a>
    <a href="hardware">Hardware & protocols</a>
  </div>
</div></center>

<!-- This script handles the button dynamics -->
<script>
function myFunction() {document.getElementById("myDropdown").classList.toggle("show");}
window.onclick = function(event) {
  if (!event.target.matches('.dropbtn')) { var dropdowns = document.getElementsByClassName("dropdown-content"); var i;
    for (i = 0; i < dropdowns.length; i++) {var openDropdown = dropdowns[i]; if (openDropdown.classList.contains('show')) {openDropdown.classList.remove('show'); } } }
} 
</script>



<!-- Start normal content here -->
# Macaque templates & atlases

[<< Back to main templates & atlases page](templates_and_atlases.md)
  

## Overview     
- [CHARM](templates_and_atlases_macaque.md#CHARM)     
- [D99 v1](templates_and_atlases_macaque.md#D99v1)     
- [D99 v2](templates_and_atlases_macaque.md#D99v2)  
- [NMT v1.3](templates_and_atlases_macaque.md#NMTv1.3)     
- [NMT v2.0](templates_and_atlases_macaque.md#NMTv2.0)
- [SARM](templates_and_atlases_macaque.md#SARM)
- [UNC-LPBR 4D](templates_and_atlases_macaque.md#unc-lpbr-4d-cynomolgus-macaque-atlases-from-birth-to-48-months)       

## Details

<a name="CHARM"></a>
### Cortical Hierarchy Atlas of the Rhesus Macaque (CHARM)      
<div class="rw-ui-container" data-title="charm rating"></div>    
**Authors**         : Benjamin Jung, Paul A. Taylor, Jakob Seidlitz, Caleb Sponheim, Pierce Perkins, Leslie G. Ungerleider, Daniel Glen, Adam Messinger    
**Description**     : A novel anatomical parcellation of the macaque cerebral cortex, where the cortical sheet is subdivided into six-levels of increasingly fine-grained parcellation. The broadest level consists of the four cortical lobes and the finest level is based on the D99 atlas, with modifications that make the regions more robust when applied to low resolution (e.g. fMRI) data.      
**Documentation**   : [AFNI](https://afni.nimh.nih.gov/pub/dist/doc/htmldoc/nonhuman/macaque_tempatl/atlas_charm.html)        
**Link**            : [AFNI](https://afni.nimh.nih.gov/pub/dist/doc/htmldoc/nonhuman/macaque_tempatl/atlas_charm.html#download)      
**Language**        : Volumetric files are in NIFTI (.nii) format, while surface files are in GIFTI (.gii) format.      
**Publication**     : [Jung et al. (2021) Neuroimage](https://doi-org.proxy.library.uu.nl/10.1016/j.neuroimage.2021.117997)
**Communication**   : Email to [Dr. Adam Messinger](Adam.Messinger@nih.gov)                                       
**Restrictions**    : Please cite the above publication                                     

<a name="D99v1"></a>
### D99 Template and Atlas v1 (NB! surpassed by v2 below)      
<div class="rw-ui-container" data-title="d99 rating"></div>    
**Authors**         : Reveley C, Gruslys A, Ye FQ, Glen D, Samaha J, Russ BE, Saad Z, Seth AK, Leopold DA, & Saleem KS.     
**Description**     : Digital version of the Saleem and Logothetis atlas with a newer, higher quality D99 surrogate MRI template. Integrated into AFNI/SUMA software.               
**Documentation**   : [AFNI site](https://afni.nimh.nih.gov/Macaque)     
**Link**            : [D99 v1](https://afni.nimh.nih.gov/pub/dist/atlases/macaque/)             
**Language**        : NIFTI format     
**Publication**     : [Reveley et al. (2017)](https://doi.org/10.1093/cercor/bhw248)        
**Communication**   : [email K. Saleem](mailto:kadharbatcha.saleem.ctr@usuhs.edu), [email D. Glen](mailto:glend@mail.nih.gov), [AFNI message board](https://afni.nimh.nih.gov/afni/community/board/list.php?1)    
**Restrictions**    : Please cite the publication above. The original cortical and subcortical parcellations on the atlas should not be modified without prior consent from the authors.    
  
<a name="D99v2"></a>
### D99 Template and Atlas v2      
<div class="rw-ui-container" data-title="d99v2 rating"></div>    
**Authors**         : Saleem KS, Avram AV, Glen D, Yen CC, Ye FQ, Komlosh M, Basser PJ.     
**Description**     : D99 Atlas v2.0: a macaque template and cortical and subcortical atlas. A comprehensive, MRI-histology based atlas of the Rhesus macaque monkey brain with segmentation of both cortical and subcortical areas in one 3D volume.             
**Documentation**   : [AFNI site](https://afni.nimh.nih.gov/pub/dist/doc/htmldoc/nonhuman/macaque_tempatl/atlas_d99v2.html)     
**Link**            : [D99 v2](https://afni.nimh.nih.gov/pub/dist/doc/htmldoc/nonhuman/macaque_tempatl/atlas_d99v2.html)   
**Language**        : NIFTI format     
**Publication**     : [Saleem et al. (2021)](https://doi.org/10.1016/j.neuroimage.2021.118759)                     
**Communication**   : [email K. Saleem](mailto:kadharbatcha.saleem.ctr@usuhs.edu), [email D. Glen](mailto:glend@mail.nih.gov), [AFNI message board](https://afni.nimh.nih.gov/afni/community/board/list.php?1)    
**Restrictions**    : Please cite the publication above. The original cortical and subcortical parcellations on the atlas should not be modified without prior consent from the authors.    

<a name="NMTv1.3"></a>
### NMT v1.3 (NIMH Macaque Template - version 1.3)       
<div class="rw-ui-container" data-title="nmt1 rating"></div>    
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
<div class="rw-ui-container" data-title="nmt2 rating"></div>    
**Authors**         : Benjamin Jung, Paul A. Taylor, Jakob Seidlitz, Caleb Sponheim, Pierce Perkins, Leslie G. Ungerleider, Daniel Glen, Adam Messinger           
**Description**     : A collection of volumetric templates of the rhesus macaque created by nonlinear averaging of T1-weighted anatomical MRIs from multiple adult monkeys. Surface files are included. The NMT 2.0 provides increased flexibility in macaque group analysis by providing symmetric and asymmetric templates. Both templates are available with an expanded, full head field of view in Horsley-Clarke stereotaxic orientation. Updates to the templates include: an improved mapping of the D99 atlas, the addition of the CHARM and SARM atlases, improved brain masking and normalization, and files that are defined in a common template space (NMT space), using the short data type for improved storage efficiency.                                   
**Documentation**   : [AFNI](https://afni.nimh.nih.gov/pub/dist/doc/htmldoc/nonhuman/macaque_tempatl/template_nmtv2.html)     
**Link**            : [AFNI](https://afni.nimh.nih.gov/pub/dist/doc/htmldoc/nonhuman/macaque_tempatl/template_nmtv2.html#download-symmetric-nmt-v2-datasets)       
**Language**        : Volumetric files are in NIFTI (.nii) format, while surface files are in GIFTI (.gii) format. Scripts for processing single subjects rely on bash shell and AFNI.                        
**Publication**     : [Jung et al. (2021) Neuroimage](https://doi-org.proxy.library.uu.nl/10.1016/j.neuroimage.2021.117997)                     
**Communication**   : Email to [Dr. Adam Messinger](Adam.Messinger@nih.gov)             
**Restrictions**    : Please cite the above publication

<a name="SARM"></a>
### Subcortical Atlas of the Rhesus Macaque (SARM)         
<div class="rw-ui-container" data-title="sarm rating"></div>    
**Authors**         : Renée Hartig, Daniel Glen, Benjamin Jung, Nikos K. Logothetis, George Paxinos, Eduardo A. Garza-Villarreal, Adam Messinger, Henry C. Evrard                  
**Description**     : An anatomical parcellation of the entire macaque subcortex tailored for magnetic resonance imaging (MRI). The regions-of-interest (ROIs) are hierarchically organized, with grouping levels suited for both fine structural and spatially broader functional analyses. SARM aims to facilitate the identification, localization, and study of neural interactions involving subcortical regions of the brain.                        
**Documentation**   : [AFNI](https://afni.nimh.nih.gov/pub/dist/doc/htmldoc/nonhuman/macaque_tempatl/atlas_sarm.html)        
**Link**            : [AFNI](https://afni.nimh.nih.gov/pub/dist/doc/htmldoc/nonhuman/macaque_tempatl/atlas_sarm.html#download)     
**Language**        : Volumetric files are in NIFTI (.nii) format, while surface files are in GIFTI (.gii) format.        
**Publication**     : [Hartig et al. (2021) Neuroimage](https://doi-org.proxy.library.uu.nl/10.1016/j.neuroimage.2021.117996)      
**Communication**   : Email to [Dr. Henry Evrard](mailto:henry.evrard@tuebingen.mpg.de) or [Dr. Adam Messinger](mailto:Adam.Messinger@nih.gov)                                      
**Restrictions**    : Please cite the above publication                                      

<a name="UNC-LPBR"></a>
### UNC-LPBR 4D Cynomolgus Macaque Atlases from Birth to 48 Months         
<div class="rw-ui-container" data-title="UNC-LPBR rating"></div>    
**Authors**         : Tao Zhong, Jingkuan Wei, Kunhua Wu, Liangjun Chen, Fenqiang Zhao, Yuchen Pei, Ya Wang, Hongjiang Zhang, Zhengwang Wu, Ying Huang, Tengfei Li, Li Wang, Yongchang Chen, Weizhi Ji, Yu Zhang, Gang Li, Yuyu Niu                           
**Description**     : We construct a comprehensive set of longitudinal brain atlases and associated tissue probability maps (gray matter, white matter, and cerebrospinal fluid) with a totally of 12 time-points from birth to 4 years of age (i.e., 1, 2, 3, 4, 5, 6, 9, 12, 18, 24, 36, and 48 months of age) based on 175 longitudinal structural MRI scans from 39 typically-developing cynomolgus macaques. To facilitate region-based analysis using the atlases, we also provide two popular hierarchy parcellations from NMT v2, i.e., cortical hierarchy maps (6 levels) and subcortical hierarchy maps (6 levels), on these longitudinal macaque brain atlases.                               
**Documentation**   : [NITRC](https://www.nitrc.org/projects/cyno_4d_atlas/)        
**Link**            : [NITRC](https://www.nitrc.org/projects/cyno_4d_atlas/)     
**Language**        : NIFTI (.nii.gz) format        
**Publication**     : [Zhong et al. (2022) Neuroimage](https://www.sciencedirect.com/science/article/pii/S1053811921010703)      
**Communication**   : [Email](mailto:taozh2315@gmail.com)                                      
**Restrictions**    : None    
  
  
[//]: # (This script is necessary to render the rating widgets)
[//]: # (Use this code to insert a widget)
[//]: # (<div class="rw-ui-container" data-title="test rating"></div>)

<script type="text/javascript">(function(d, t, e, m){
    // Async Rating-Widget initialization.
    window.RW_Async_Init = function(){
        RW.init({
            huid: "461543",
            uid: "08f35e7d11687ef3ae7b3e7c219b6114",
            source: "website",
            options: {
                "advanced": {
                    "layout": {
                        "lineHeight": "12px"
                    },
                    "nero": {
                        "showDislike": false
                    },
                    "text": {
                        "rateThis": "Like this resource"
                    }
                },
                "type": "nero",
                "style": "check",
                "isDummy": false,
                "showTooltip": false,
            } 
        });
        RW.render();
    };
        // Append Rating-Widget JavaScript library.
    var rw, s = d.getElementsByTagName(e)[0], id = "rw-js",
        l = d.location, ck = "Y" + t.getFullYear() + 
        "M" + t.getMonth() + "D" + t.getDate(), p = l.protocol,
        f = ((l.search.indexOf("DBG=") > -1) ? "" : ".min"),
        a = ("https:" == p ? "secure." + m + "js/" : "js." + m);
    if (d.getElementById(id)) return;              
    rw = d.createElement(e);
    rw.id = id; rw.async = true; rw.type = "text/javascript";
    rw.src = p + "//" + a + "external" + f + ".js?ck=" + ck;
    s.parentNode.insertBefore(rw, s);
    }(document, new Date(), "script", "rating-widget.com/"));
</script>
