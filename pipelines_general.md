
---

##### [Template/Atlas](templates_and_atlases.md) &nbsp;  - &nbsp;  [General](pipelines_general.md) &nbsp;  - &nbsp;  [Structural](pipelines_structural.md) &nbsp;  - &nbsp;  [fMRI](pipelines_fmri.md) &nbsp;  - &nbsp;  [Diffusion](pipelines_diffusion.md) &nbsp;  - &nbsp;  [Data](data_sharing.md) &nbsp;  - &nbsp; [Software packages](software_packages.md)  &nbsp;  - &nbsp; [Hardware](hardware.md)          
---    

# General tools

## Overview
- [C-PAC](pipelines_general.md#c-pac-the-configurable-pipeline-for-the-analysis-of-connectomes) 
- [NeuroElf](pipelines_general.md#neuroelf) 
    
<br>    

## Details

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
