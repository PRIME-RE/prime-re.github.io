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
# Data sharing

## Overview     
- [BigMac Dataset](templates_and_atlases_chimpanzee.md#bigmac)        
- [National Chimpanzee Brain Resource](templates_and_atlases_chimpanzee.md#national-chimpanzee-brain-resource)        
- [Neurovault.org](data_sharing.md#neurovault-org)
- [Openneuro.org](data_sharing.md#openneuro)      
- [PRIME-DE](data_sharing.md#prime-de)   
- [Structural, diffusion and rs-functional MRI in Macaque Monkeys](data_sharing.md#structural-diffusion-and-rs-functional-mri-in-macaque-monkeys)

## Details

### The BigMac dataset	            
<div class="rw-ui-container" data-title="NCBR rating"></div>    
**Authors**         : Amy FD Howard, Istvan N Huszar, Adele Smart, Michiel Cottaar, Greg Daubney, Taylor Hanayik, Alexandre A Khrapitchev, Rogier B Mars, Jeroen Mollink, Connor Scott, Nicola R Sibson, Jerome Sallet, Saad Jbabdi, Karla L Miller            
**Description**     : An open dataset combining in vivo MRI, postmortem MRI and multi-contrast microscopy in a single, rhesus macaque brain. The in vivo data includes functional, structural and diffusion MRI. The postmortem MRI includes structural MRI, a T1 map and an extensive diffusion protocol (two resolutions, multi-shell, ultra-HARDI + spherical tensor encoding). The microscopy includes polarised light imaging and histology acquired throughout the brain. The MRI and microscopy have been coregistered and warpfields are provided.                         
**Documentation**   : [Documentation](https://open.win.ox.ac.uk/pages/amyh/bigmacdocumentation/ )     
**Link**            : [Link](https://open.win.ox.ac.uk/DigitalBrainBank/#/datasets/anatomist)    
**Language**        : bash, matlab, python                    
**Publication**     : [Publication](https://open.win.ox.ac.uk/DigitalBrainBank/#/datasets/anatomist)                     
**Communication**   : [Email](mailto:amy.howard@ndcn.ox.ac.uk)               
**Restrictions**    : Data access requires a data sharing agreement to be signed between institutions. This stipulates the data can only be used for scientific research and that future publications acknowledge the original manuscript and funding body.   

### National Chimpanzee Brain Resource	            
<div class="rw-ui-container" data-title="NCBR rating"></div>    
**Authors**         : [NCBR Team](https://www.chimpanzeebrain.org/our-team-and-partners)            
**Description**     : The National Chimpanzee Brain Resource (NCBR) has the aim of facilitating research advancement through the collection and distribution of chimpanzee neuroimaging data and postmortem brain tissue. The NCBR also serves as a portal to access chimpanzee brain atlas tools, data repository, bibliography of publications, educational information, and links to other chimpanzee brain resources and datasets on the Internet.                         
**Documentation**   : [NCBR](https://www.chimpanzeebrain.org)     
**Link**            : [NCBR](https://www.chimpanzeebrain.org)    
**Language**        : Website in English                    
**Publication**     : [NCBR related publications](https://www.chimpanzeebrain.org/fixed-tissue-research)                     
**Communication**   : [NCBR Team](https://www.chimpanzeebrain.org/our-team-and-partners)               
**Restrictions**    : None indicated.     

### Neurovault.org       
<div class="rw-ui-container" data-title="neurovault rating"></div>    
**Authors**         : Fox AS & Gorgolewski KJ                  
**Description**     : The method for optimally sharing voxelwise data from NHP neuroimaging studies remains unclear. To address this issue, Fox and colleagues have adapted the Neurovault.org resource (Gorgolewski et al., 2015), which is commonly used to share human neuroimaging data, to other species, including rhesus monkeys. To complement within-manuscript reporting (e.g. location of peak-activations), researchers can now upload any voxelwise images aligned to NMT-template space, including unthresohlded statistical maps, atlases, and ROIs to Neurovault.org by specifying their species-specific template. Collections of voxelwise analyses can be linked to publication DOIs to appropriately credit researchers, and will ultimately facilitate meta-analyses, and other large-scale data-scientific efforts, such as cross-species comparisons.                                         
**Documentation**   : [FAQ](https://neurovault.org/FAQ)     
**Link**            : [Neurovault.org](https://neurovault.org/)    
**Publication**     : [Gorgolewski et al. (2015)](https://www.frontiersin.org/articles/10.3389/fninf.2015.00008/full)                   
**Communication**   : [Email](mailto:dfox@ucdavis.edu) 

### Openneuro     
<div class="rw-ui-container" data-title="openneuro rating"></div>    
**Authors**         : Stanford Center For Reproducible Neuroscience               
**Description**     : A free and open platform for sharing MRI, MEG, EEG, iEEG, and ECoG data. It was formerly known as Open fMRI, but has been updated to include more types of data. The hundreds of public datasets available there are organized according to the [BIDS format](https://bids.neuroimaging.io). Openneuro datasets can be also accessed via [Datalad](https://www.datalad.org). Though Open Neuro primarily contains data from human participants, several NHP datasets are also available through the platform.                                            
**Documentation**   : [Openneuro FAQ](https://openneuro.org/faq)  
**Link**            : [Openneuro.org](https://openneuro.org)    
**Publication**     : [Poldrack et al. (2013)](https://www.frontiersin.org/articles/10.3389/fninf.2013.00012/full)                   
**Communication**   : [Openneuro Support](https://openneuro.org) 

### PRIME-DE       
<div class="rw-ui-container" data-title="prime-de rating"></div>    
**Authors**         : PRIME-DE consortium                  
**Description**     : The overarching goal of PRIMatE Data Exchange (PRIME-DE) is to create an open science resource for the neuroimaging community that will facilitate the mapping of the non-human primate connectome. To accomplish this, we will aggregate a combination of functional, diffusion and morphometric magnetic resonance imaging (MRI) datasets across laboratories around the world, and share the data with the larger scientific community.                                         
**Documentation**   : [PRIME-DE](http://fcon_1000.projects.nitrc.org/indi/indiPRIME.html)   
**Link**            : [PRIME-DE](http://fcon_1000.projects.nitrc.org/indi/indiPRIME.html)    
**Publication**     : [Milham et al. (2018)](https://doi.org/10.1016/j.neuron.2018.08.039)                   
**Communication**   : [Email](mailto:Michael.Milham@childmind.org) 

### Structural, diffusion and rs-functional MRI in Macaque Monkeys    
<div class="rw-ui-container" data-title="sdrsfmri rating"></div>    
**Name**            : Structural, diffusion and rs-functional MRI in Macaque Monkeys                                             
**Authors**         : Vanessa De Castro, Benoit Cottereau and Jean-Baptiste Durand                                                    
**Description**     : This dataset contains unprocessed structural, diffusion and rs-functional MRI data acquired in 3 female rhesus macaques. Each monkey underwent multiple sessions. For each session they were lightly anesthetized. The animals were installed in sphinx position with their head restrained by a head-post. Whole-brain images were acquired on a 3 Tesla clinical MR scanner (Philips Achieva).                       
**Link**            : [openneuro](https://openneuro.org/datasets/ds003989/versions/1.0.0)        
**Publication**     : [De Castro et al. (2021)](https://doi.org/10.1093/cercor/bhaa301)     
**Communication**   : [Email De Castro](mailto:vanessa.decastro@cnrs.fr) or [Email Durand](mailto:jbdurand@cnrs.fr)                              
**Restrictions**    : citation required                                  
       
     
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
