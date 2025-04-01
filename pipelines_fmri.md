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
# Functional analysis

## Overview
- [AFNI afni_proc.py](pipelines_fmri.md#afni-afni_procpy)       
- [C-PAC](pipelines_fmri.md#c-pac-the-configurable-pipeline-for-the-analysis-of-connectomes) 
- [MR Comparative Anatomy Toolbox (MrCat)](pipelines_fmri.md#mr-comparative-anatomy-toolbox-mrcat)
- [NeuroElf](pipelines_fmri.md#neuroelf) 
- [NHP-BIDS](pipelines_fmri.md#nhp-bids) 
- [NHP-pycortex](pipelines_fmri.md#nhp-pycortex) 
- [Pypreclin](pipelines_fmri.md#pypreclin) 


## Details

### AFNI afni_proc.py     
<div class="rw-ui-container" data-title="afni_proc.py rating"></div>     
**Authors**         : Rick Reynolds, Paul Taylor, Daniel Glen, Gang Chen, Bob Cox 	             
**Description**     : FMRI analysis pipeline tool in AFNI. This widely used, general purpose and flexible tool for creating a full, single subject FMRI processing stream can be used for macaque analyses. This program creates fully commented, single subject processing scripts for all FMRI study designs (task, resting state, naturalistic, etc.) and for either volumetric- or surface-based analyses. The typical goal is to create volumes of aligned response magnitudes (stimulus beta weights from a GLM) to use as input for a group analysis.         
**Documentation**   : [documentation](https://afni.nimh.nih.gov/pub/dist/doc/program_help/afni_proc.py.html)<br/>[tutorials](https://afni.nimh.nih.gov/pub/dist/doc/htmldoc/nonhuman/macaque_demos/main_toc.html)     
**Link**            : [https://afni.nimh.nih.gov](https://afni.nimh.nih.gov/)    
**Language**        : python, tcsh, C, AFNI                                                       
**Publication**     : [Cox (1996)](https://pubmed.ncbi.nlm.nih.gov/8812068/)<br/>[Jung et al. (submitted)](https://www.biorxiv.org/content/10.1101/2020.08.05.237818v1)        
**Communication**   : [AFNI message board](https://afni.nimh.nih.gov/afni/community/board/list.php?1)               
**Restrictions**    : Please cite the above publications 


### C-PAC: The Configurable Pipeline for the Analysis of Connectomes    
<div class="rw-ui-container" data-title="C-PAC rating"></div>    
**Authors**         : Steven Giavasis, Cameron Craddock, Michael Milham                                                               
**Description**     : The Configurable Pipeline for the Analysis of Connectomes (C-PAC) is a configurable, open-source, Nipype-based, automated processing pipeline for resting state functional MRI (R-fMRI) data, for use by both novice and expert users. It is designed and tested for use with human data (all ages), as well as with non-human primate and rodent data.                   
**Documentation**   : [http://fcp-indi.github.io/](http://fcp-indi.github.io/)                                      
**Link**            : [Quick-Start](http://fcp-indi.github.io/docs/user/quick.html)               
**Language**        : Python                                                  
**Publication**     : [Craddock et al. (2013)](https://www.frontiersin.org/10.3389/conf.fninf.2013.09.00042/event_abstract)         
**Communication**   : [C-PAC Forum](https://groups.google.com/forum/#!forum/cpax_forum)                                             
**Restrictions**    : None       

### MR Comparative Anatomy Toolbox (MrCat)       
<div class="rw-ui-container" data-title="MrCat rating"></div>    
**Authors**         : Rogier B. Mars, Lennart Verhagen, and the members and collaborators of the Cognitive Neuroecology Lab	             
**Description**     : A collection of tools for processing of multi-species neuroimaging data.                               
**Documentation**   : [Online doc](http://www.neuroecologylab.org)     
**Link**            : [www.neuroecologylab.org](http://www.neuroecologylab.org)    
**Language**        : shell, matlab                                                                                  
**Publication**     : [Mars et al. 2016](http://www.rbmars.dds.nl/pubs/Mars2016NBR.pdf), among others                        
**Communication**   : [www.neuroecologylab.org](http://www.neuroecologylab.org)                                           
**Restrictions**    : None  

### NeuroElf    
<div class="rw-ui-container" data-title="NeuroElf rating"></div>    
**Authors**         : Jochen Weber                                                                             
**Description**     : NeuroElf is a powerful Matlab-based toolbox for working with neuroimaging data.                  
**Documentation**   : [NeuroElf website](http://neuroelf.net/)                                     
**Link**            : [http://neuroelf.net/](http://neuroelf.net/)         
**Language**        : Matlab                                                  
**Publication**     : [http://neuroelf.net/](http://neuroelf.net/)                                                                                        
**Communication**   : [GitHub](https://github.com/neuroelf/neuroelf-matlab)                                            
**Restrictions**    : See [license](http://neuroelf.net/wiki/doku.php?id=neuroelf_license)    


### NHP-BIDS     
<div class="rw-ui-container" data-title="NHP-BIDS rating"></div>     
**Authors**         : Chris Klink                                                                             
**Description**     : This pipeline uses NiPype to organize and (pre)process NHP-MRI data in accordance with BIDS. It covers the entire pipeline from exporting the data from the scanner, via motion correction and warping, to running a GLM.              
**Documentation**   : [GitHub WIKI](https://github.com/VisionandCognition/NHP-BIDS/wiki)                                                 
**Link**            : [GitHub link](https://github.com/VisionandCognition/NHP-BIDS/tree/public)         
**Language**        : Python, Shell                                                       
**Publication**     : -                                                                                       
**Communication**   : [GitHub profile](https://github.com/pcklink)                                            
**Restrictions**    : None                                                                                      

### NHP-pycortex     
<div class="rw-ui-container" data-title="NHP-pycortex rating"></div>     
**Authors**         : Chris Klink                                                                             
**Description**     : Import surfaces generated with [NHP-Freesurfer](pipelines_structural.md#NHP-Freesurfer) into a version of pycortex that is adapted for NHP use. This opens up the possibility of using pycortex to visualize fMRI results on the surface.                     
**Documentation**   : Available in Jupyter notebook on GitHub                                                 
**Link**            : [GitHub link](https://github.com/VisionandCognition/NHP-pycortex)         
**Language**        : Jupyter notebooks with Python 3                                                       
**Publication**     : -                                                                                       
**Communication**   : [GitHub profile](https://github.com/pcklink)                                            
**Restrictions**    : None  

### Pypreclin    
<div class="rw-ui-container" data-title="Pypreclin rating"></div>    
**Authors**         : Jordy Tasserie, Antoine Grigis, Lynn Uhrig, Morgan Dupont, Alexis Amadon and Béchir Jarraya.                 
**Description**     : Pypreclin is a flexible and automatic tool for preprocessing of macaque fMRI data available for the growing community of primate fMRI.                                   
**Documentation**   : [GitHub](https://github.com/neurospin/pypreclin)      
**Link**            : The Python project can be found on [GitHub](https://github.com/neurospin/pypreclin), on the Python Package Index [PyPI](https://pypi.org/project/pypreclin/) for easy installation and upgrading, and also as a [Singularity container](biodev.cea.fr/pypreclin/pypreclin-ubuntu.simg).   <br> 
**Language**        : Python           
**Publication**     : Tasserie J, Grigis A, Uhrig L, Dupont M, Amadon A, Jarraya B. Neuroimage. 2019 Nov 16:116353. doi: 10.1016/j.neuroimage.2019.116353. [Pubmed](https://www.ncbi.nlm.nih.gov/pubmed/31743789) - [Journal website](https://www.sciencedirect.com/science/article/pii/S1053811919309449?via%3Dihub)  <br>
**Communication**   : [GitHub profile](https://github.com/AGrigis)         
**Restrictions**    : Please cite the related publication   




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
