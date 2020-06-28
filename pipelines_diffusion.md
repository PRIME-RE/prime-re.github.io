
---

##### [Template/Atlas](templates_and_atlases.md) &nbsp;  - &nbsp;  [General](pipelines_general.md) &nbsp;  - &nbsp;  [Structural](pipelines_structural.md) &nbsp;  - &nbsp;  [fMRI](pipelines_fmri.md) &nbsp;  - &nbsp;  [Diffusion](pipelines_diffusion.md) &nbsp;  - &nbsp;  [Data](data_sharing.md) &nbsp;  - &nbsp; [Software packages](software_packages.md)  &nbsp;  - &nbsp; [Hardware](hardware.md)          
---    

# Diffusion

## Overview
- [Diffusion-MRI by Rakshit](pipelines_diffusion.md#diffusion-mri-by-rakshit) 
- [MR Comparative Anatomy Toolbox (MrCat)](pipelines_diffusion.md#mr-comparative-anatomy-toolbox-mrcat)
    
<br>    

## Details

### Diffusion-MRI by Rakshit     
<div class="rw-ui-container" data-title="Rakshit rating"></div>     
**Authors**         : Rakshit Dadarwal                                                                             
**Description**     : These Jupyter notebooks showcase  an example of diffusion MRI preprocessing and analysis with python. They include steps for basic preprocessing (denoising, susceptibility-induced distortion correction, eddy current-induced distortion and motion correction), model fitting (DTI, DKI, NODDI) and calculation of parametric maps. These steps use functions from [DIPY](https://dipy.org/), [FSL](https://fsl.fmrib.ox.ac.uk/fsl/fslwiki/), and [AMICO](https://github.com/daducci/AMICO).                  
**Documentation**   : [Jupyter notebooks on GitHub](https://github.com/RDadarwal/Diffusion-MRI)                                     
**Link**            : [GitHub link](https://github.com/RDadarwal/Diffusion-MRI)         
**Language**        : Python                                                  
**Publication**     : -                                                                                       
**Communication**   : [GitHub profile](https://github.com/RDadarwal)                                            
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
