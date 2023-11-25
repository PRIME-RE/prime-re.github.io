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
# Structural analysis

## Overview     
- [AFNI @animal_warper](pipelines_structural.md#afni-animal_warper)   
- [BETS_formers](pipelines_structural.md#bets_formers-brain-extraction-and-tissue-segmentation-for-macaque-using-transformer-models)  
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
   

## Details

### AFNI @animal_warper       
<div class="rw-ui-container" data-title="animal_warper rating"></div>    
**Authors**         : Daniel Glen, Paul Taylor, Adam Messinger, Benjamin Jung, Jakob Seidlitz                 
**Description**     : Nonlinearly aligns an MRI dataset to a template. The reverse transformation can be used to produce a skullstripped (brain-only) version of the native scan, segmentation/atlas info in the native space, and surfaces for each atlas region. The computed transformations between the anatomical scan and the template is provided for use with FMRI pipeline tools like afni_proc.py.                                   
**Documentation**   : [documentation](https://afni.nimh.nih.gov/pub/dist/doc/program_help/@animal_warper.html)<br/>[tutorials](https://afni.nimh.nih.gov/pub/dist/doc/htmldoc/nonhuman/macaque_demos/main_toc.html)     
**Link**            : [AFNI](https://afni.nimh.nih.gov/)    
**Language**        : tcsh, python, C, AFNI                                                                         
**Publication**     : [Cox (1996)](https://pubmed.ncbi.nlm.nih.gov/8812068/)<br/>[Jung et al. (submitted)](https://www.biorxiv.org/content/10.1101/2020.08.05.237818v1)                                                                   
**Communication**   : [AFNI message board ](https://afni.nimh.nih.gov/afni/community/board/list.php?1) 
**Restrictions**    : Please cite the above publications              
 
### BETS_Formers: Brain Extraction and Tissue Segmentation for Macaque using Transformer Models       
<div class="rw-ui-container" data-title="BETS_formers rating"></div>    
**Authors**         : Tao Zhong, Xueyang Wu, Yuyu Niu, Gang Li, Yu Zhang                  
**Description**     : Transformer models were provided for brain extraction and tissue segmentation in macaque T1w images. The models were trained on a large macaque samples from different sites and have been validated on data from different sites and perform well. We hoped these models could help more researchers in this field and thus benefit the neuroscience community in biomedical studies of non-human primates.          
**Documentation**   : [Github](https://github.com/TaoZhong11/BrainExtraction-TissueSegmentation-Macaque)     
**Link**            : [Github repo](https://github.com/TaoZhong11/BrainExtraction-TissueSegmentation-Macaque)       
**Language**        : Python                                                                         
**Publication**     : [Zhong et al. (2022) Neuroimage](https://www.sciencedirect.com/science/article/pii/S1053811921010703)                                      
**Communication**   : [email](mailto:taozh2315@gmail.com)        
**Restrictions**    : None    
  
### BrainBox       
<div class="rw-ui-container" data-title="BrainBox rating"></div>    
**Authors**         : Katja Heuer & Roberto Toro                  
**Description**     : A Web application for visualising, annotating & segmenting 3D brain imaging data in real time, collaboratively.   
**Documentation**   : [3 min video](https://www.youtube.com/watch?v=kwsLoVKnw24)     
**Link**            : [https://brainbox.pasteur.fr](https://brainbox.pasteur.fr)       
**Language**        : JavaScript, HTML, CSS                                                                         
**Publication**     : [Open Neuroimaging Laboratory](https://doi.org/10.3897/rio.2.e9113)                                      
**Communication**   : [Mattermost](https://mattermost.brainhack.org/brainhack/channels/brainbox) or [GitHub issues](https://github.com/neuroanatomy/BrainBox/issues)    
**Restrictions**    : Developed and tested in Chrome Browser         

### CIVET-macaque       
<div class="rw-ui-container" data-title="CIVET-macaque rating"></div>    
**Authors**         : Claude Lepage, Konrad Wagstyl, Ben Jung, Jakob Seidlitz, Caleb Sponheim, Leslie Ungerleider, Xindi Wang, Alan Evans, Adam Messinger                   
**Description**     : Fully automated structural MRI pipeline using the NIH Macaque Template (NMT). Performs registration, segmentation, and surface reconstruction of T1-weighted anatomical scans. Provides quality control images, white matter, pial and mid cortical surfaces, and surface morphometrics including cortical thickness maps.    
**Documentation**   : [Github](https://github.com/aces/CIVET_Full_Project)     
**Link**            : [Github](https://github.com/aces/CIVET_Full_Project)    
**Language**        : C, minc, NIFTI/GIFTI.  Binaries available on GitHub.                                          
**Publication**     : [Lepage et al. (submitted)](https://www.biorxiv.org/content/10.1101/2020.08.04.237149v1)         
**Communication**   : Email to [Dr. Adam Messinger](mailto:Adam.Messinger@nih.gov) or [Github](https://github.com/aces/CIVET_Full_Project/issues)                     
**Restrictions**    : Please cite the above publication          

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

### Macapype       
<div class="rw-ui-container" data-title="Macapype rating"></div>    
**Authors**         : Bastien Cagna, David Meunier, Kep kee Loh, Julien Sein, & Régis Trapeau                 
**Description**     : Python package for NHP anatomical MRI segmentation using Nipype.                               
**Documentation**   : [Online doc](https://macatools.github.io/macapype/index.html)     
**Link**            : [https://github.com/Macatools/macapype](https://github.com/Macatools/macapype)    
**Language**        : Python                                                                                  
**Publication**     : -                                                                                       
**Communication**   : [Post issue on GitHub website](https://github.com/Macatools/macapype/issues/new)               
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

### NHP-Freesurfer     
<div class="rw-ui-container" data-title="NHP-Freesurfer rating"></div>    
**Authors**         : Chris Klink                                                                             
**Description**     : Segmentation and surface generation of monkey brains using Freesurfer, the NMT template, and other tools. Jupyter Notebooks with documentation on how to generate surfaces and project results to it.            
**Documentation**   : Available in Jupyter notebook on GitHub                                                 
**Link**            : [GitHub link](https://github.com/VisionandCognition/NHP-Freesurfer/tree/public)         
**Language**        : Jupyter notebooks with Shell code                                                       
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

### Precon_all     
<div class="rw-ui-container" data-title="Precon_all rating"></div>    
**Authors**         : R. Austin Benn, Ting Xu                                                                             
**Description**     : precon_all is an anatomical surface reconstruction pipeline that can be used with Non-Human Primates, and other large animals including pigs, dogs, and potentially many more. The pipeline can be easily modified to work on most species with a reasonable T1 image by simply providing 5 masks. The pipeline provides both freesurfer and HCP compatible outputs in native image space. Group average surfaces and spherical registration templates can also be created within the precon_all framework.                   
**Documentation**   : [precon_all](https://github.com/recoveringyank/precon_all)                                    
**Link**            : [GitHub Link](https://github.com/recoveringyank/precon_all)        
**Language**        : shell                                                       
**Publication**     : In preparation                                                                                       
**Communication**   : [Email](mailto:rabbenn@cnic.es)                                            
**Restrictions**    : None       

### PREEMACS     
<div class="rw-ui-container" data-title="PREEMACS rating"></div>    
**Authors**         : Pamela Garcia-Saldivar, Arun Garimella, Eduardo A. Garza-Villarreal, Felipe Mendez, Luis Concha and Hugo Merchant                                                                                 
**Description**     : PREEMACS (pipeline for PREprocessing and Extraction of the MACaque brain Surface) is a pipeline to process raw structural images in order to obtain brain surfaces and cortical thickness, without requiring manual editing. PREEMACS has a modular design, with three modules running independently: Preprocessing, Quality Control and Brain Surface estimation based on FreeSurfer.   To evaluate the generalizability of our method, we tested PREEMACS on three different datasets of NHP images: PRIME-DE, UNC-Wisconsin Database and INB-UNAM.  Results showed accurate and robust automatic brain surface extraction in our INB-UNAM database and precise extraction in the UNC-Wisconsin and PRIME-DE databases for images that passed the quality control segment of our pipeline.                   
**Documentation**   : [PREEMACS](https://github.com/pGarciaS/PREEMACS/wiki)                                               
**Link**            : [GitHub Link](https://github.com/pGarciaS/PREEMACS)        
**Language**        : python, shell and matlab                                                       
**Publication**     : -                                                                                       
**Communication**   : [GitHub Profile](https://github.com/pGarciaS)                                            
**Restrictions**    : None  

### Reorient     
<div class="rw-ui-container" data-title="Reorient rating"></div>    
**Authors**         : Katja Heuer & Roberto Toro                                                                                     
**Description**     : A Web tool for reorienting and cropping MRI data               
**Documentation**   : [Doc in the GitHub repo](https://neuroanatomy.github.io/reorient/doc.html)                                             
**Link**            : [Web tool](https://neuroanatomy.github.io/reorient)      
**Language**        : JavaScript, HTML, CSS                                                       
**Publication**     : [Heuer and Toro 2020](https://doi.org/10.21105/joss.02670).                                                                                      
**Communication**   : [GitHub issues](https://github.com/neuroanatomy/reorient/issues)                                                 
**Restrictions**    : Developed and tested in Chrome Browser  

### Thresholdmann     
<div class="rw-ui-container" data-title="Thresholdmann rating"></div>    
**Authors**         : Katja Heuer & Roberto Toro                                                                                     
**Description**     : A Web tool for interactively creating adaptive thresholds to segment nifti images               
**Documentation**   : [Doc in the GitHub repo](https://neuroanatomy.github.io/thresholdmann/doc.html)                                        
**Link**            : [Web tool](https://neuroanatomy.github.io/thresholdmann)      
**Language**        : JavaScript, HTML, CSS                                                       
**Publication**     : Work in progress                                                                                       
**Communication**   : [GitHub issues](https://github.com/neuroanatomy/thresholdmann/issues)                                     
**Restrictions**    : Developed and tested in Chrome Browser  

### UNet model for skull stripping and brain masks of anatomical images from PRIME-DE         
<div class="rw-ui-container" data-title="UNet rating"></div>    
**Authors**         : Xindi Wang, Ting Xu                                                                             
**Description**     : The preprocessed brain masks of T1w images for all macaque monkeys from PRIME-DE. A convolutional network - UNet model was used to generate the brain mask for T1w images. The UNet model was initially trained in a large human sample and upgraded with a few macaque data. With a small macaque training sample (N=1-2), the UNet model achieves a decent performance of brain extraction with a minimal processing time (GPU: ~20s, CPU: 2-10 min).                       
**Documentation**   : [UNet model on PRIME-DE](https://github.com/HumanBrainED/NHP-BrainExtraction)    
**Link**            : [code](https://github.com/HumanBrainED/NHP-BrainExtraction), [preprocessed brain masks](https://github.com/TingsterX/PRIME-DE/tree/master/BrainExtraction)             
**Language**        : Python                                                       
**Publication**     : [In prepartion](https://github.com/to-be-release)                                 
**Communication**   : [GitHub profile](https://github.com/TingsterX)                                                 
**Restrictions**    : GNU   



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
