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
# Marmoset templates and atlases

[<< Back to main templates & atlases page](templates_and_atlases.md)


## Overview       
- [Marmoset Brain Connectivity Atlas](templates_and_atlases_marmoset.md#marmoset-brain-connectivity-atlas)        
- [Marmoset Brain Mapping Atlas and Template](templates_and_atlases_marmoset.md#marmoset-brain-mapping-atlas-and-template)   
- [Nencki-Monash Template](templates_and_atlases_marmoset.md#nencki-monash-template)


## Details

### Marmoset Brain Connectivity Atlas            
<div class="rw-ui-container" data-title="mbca rating"></div>    
**Authors**         : The project is lead by Piotr Majka of the Laboratory of Neuroinformatics at the Nencki Institute of Experimental Biology (Poland) and prof. Marcello Rosa at Monash University (Australia). [Full list of contributors](http://www.marmosetbrain.org/about).         	     
**Description**     : The Marmoset Brain Connectivity Atlas allows for the exploration of a growing collection of retrograde tracer injections in the marmoset neocortex. Data obtained in different animals are registered to a [common stereotaxic space](http://www.marmosetbrain.org/reference) of Paxinos et al. (2012) atlas, and the resource incorporates tools for quantitative analyses. In particular, the results can be downloaded in 3D volume format in a template space which allows for ready comparisons to topologies acquired by MRI.                   
**Documentation**   : Portal’s application programming interface are available [here](http://analytics.marmosetbrain.org/wiki/api) and [here](http://analytics.marmosetbrain.org/wiki/database).     
**Link**            : [http://www.marmosetbrain.org](http://www.marmosetbrain.org)    
**Language**        : The portal is implemented in JavaScript, Python, and CSS / HTML. The source code of both components of the [http://marmosetbrain.org](http://marmosetbrain.org) is released under the GPL license (see: [here](https://github.com/Neuroinflab/marmosetbrain.org) and [here](https://github.com/Neuroinflab/analysis.Marmosetbrain.org).           
**Publication**     : [Majka et al. (2020)](http://doi.org/10.1038/s41467-020-14858-0) and [Majka et al. (2016)](http://doi.org/10.1002/cne.24023).                     
**Communication**   : [Piotr Majka](mailto:p.majka@nencki.edu.pl)    
**Restrictions**    : Material made public on the Marmoset Brain Connectivity Atlas is licensed under Creative Commons Attribution-ShareAlike 4.0 (CC-BY-SA) License. You are free to share (copy and redistribute) and adapt (remix, transform, and build upon) the marmoset-related material in any medium or format as long as you attribute the Marmoset Brain Connectivity Atlas and provide a link to the two URLs the Marmoset Brain Connectivity Atlas and the CC license). If you adapt the material, you must distribute your contributions under the same license as the original.     

### Marmoset Brain Mapping Atlas and Template       
<div class="rw-ui-container" data-title="mbmat rating"></div>    
**Authors**         : Cirong Liu, Daniel Glen, Frank Ye, John Newman, Cecil Yen, Diego Szczupak, Xiaoguang Tian, Piotr Majka, Marcello Rosa, David Leopold, Afonso Silva        	     
**Description**     : The Marmoset Brain Mapping Atlas (previously NIH Marmoset Brain Atlas) aims at building comprehensive MRI-based marmoset brain atlases and tools to facilitate neuroimaging and connectome studies of marmosets.                   
**Documentation**   : [Marmoset Brain Mapping site](https://marmosetbrainmapping.org/atlas.html)     
**Link**            : [Marmoset Brain Mapping site](https://marmosetbrainmapping.org/atlas.html)    
**Language**        : shell, matlab, etc.          
**Publication**     : [Liu et al. (2018)](https://doi.org/10.1016/j.neuroimage.2017.12.004), [Liu et al. (2020)](https://doi.org/10.1038/s41593-019-0575-0)                     
**Communication**   : [email](mailto:info@marmosetbrainmapping.org)    
**Restrictions**    : Creative Commons Attribution-NonCommercial-ShareAlike (CC BY-NC-SA 4.0)    

### Nencki-Monash Template       
<div class="rw-ui-container" data-title="Nencki-Monash rating"></div>    
**Authors**         : The template has been created in collaboration between the Laboratory of Neuroinformatics at the Nencki Institute of Experimental Biology (Poland) and prof. Marcello Rosa Laboratory at Monash University (Australia).        	     
**Description**     : The Nencki-Monash (NM) template represents a morphological average of 20 brains of young adult individuals, obtained by 3D reconstructions generated from Nissl-stained serial sections. The template combines combines the main advantages of histology-based atlases with features associated with MRI-based templates. It is also accompanied with spatial transformations to other popular marmoset brain templates, thus enabling integration with magnetic resonance imaging (MRI) and tracer-based connectivity data.                   
**Documentation**   : The documentation and examples are available within individual datasets [here](http://www.marmosetbrain.org/nencki_monash_template)     
**Link**            : [nencki_monash_templatee](http://www.marmosetbrain.org/nencki_monash_template)    
**Language**        : N/A          
**Publication**     : [Preprint](https://doi.org/10.1101/2020.04.10.036632)                     
**Communication**   : [Piotr Majka](mailto:p.majka@nencki.edu.pl)    
**Restrictions**    : Nencki-Monash Template is licensed under Creative Commons Attribution-ShareAlike 4.0 (CC-BY-SA) License. You are free to share (copy and redistribute) and adapt (remix, transform, and build upon) the marmoset-related material in any medium or format as long as you attribute the Nencki-Monash Template and cite the relevant publication. If you adapt the material, you must distribute your contributions under the same license as the original.   



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

