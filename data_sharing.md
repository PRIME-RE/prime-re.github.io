
---

##### [Template/Atlas](templates_and_atlases.md) &nbsp;  - &nbsp;  [General](pipelines_general.md) &nbsp;  - &nbsp;  [Structural](pipelines_structural.md) &nbsp;  - &nbsp;  [fMRI](pipelines_fmri.md) &nbsp;  - &nbsp;  [Diffusion](pipelines_diffusion.md) &nbsp;  - &nbsp;  [Data](data_sharing.md) &nbsp;  - &nbsp; [Software packages](software_packages.md)  &nbsp;  - &nbsp; [Hardware](hardware.md)          
---    

# Data sharing

## Overview     
- [Neurovault.org](data_sharing.md#neurovault-org)
- [Openneuro.org](data_sharing.md#openneuro)      
- [PRIME-DE](data_sharing.md#prime-de)   

<br>     

## Details

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
