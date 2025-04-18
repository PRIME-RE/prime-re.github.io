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
# General analysis

## Overview
- [C-PAC](pipelines_general.md#c-pac-the-configurable-pipeline-for-the-analysis-of-connectomes)
- [MacqD](pipelines_general.md#macqd) 
- [NeuroElf](pipelines_general.md#neuroelf) 
     

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

### MacqD
<div class="rw-ui-container" data-title="maqd rating"></div>    
**Authors**         : Genevieve Jiawei Moat, Maxime Gaudet-Trafit, Julian Paul, Jaume Bacardit, Suliann Ben Hamed & Colline Poirier                                                                  
**Description**     : Deep-learning-based model for automatic detection of socially housed laboratory macaques.                       
**Documentation**   : [https://github.com/C-Poirier-Lab/MacqD.git](https://github.com/C-Poirier-Lab/MacqD.git)                                      
**Link**            : [https://github.com/C-Poirier-Lab/MacqD.git](https://github.com/C-Poirier-Lab/MacqD.git)               
**Language**        : Python: 3.7.13                                                       
**Publication**     : [Moat GJ et al. (2025)](https://rdcu.be/egK32)         
**Communication**   : [E-mail Colline](mailto:colline.poirier@ncl.ac.uk)                                             
**Restrictions**    : citation required  

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
