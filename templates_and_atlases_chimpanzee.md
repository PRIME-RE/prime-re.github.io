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
# Chimpanzee templates and atlases

[<< Back to main templates & atlases page](templates_and_atlases.md)


## Overview       
- [Juna.Chimp Templates & Davi130 parcellation](templates_and_atlases_marmoset.md#juna)        
- [National Chimpanzee Brain Resource](templates_and_atlases_marmoset.md#ncbr)        


## Details

<a name="JUNA"></a>
### Juna.Chimp Templates & Davi130 parcellation            
<div class="rw-ui-container" data-title="junachimp rating"></div>    
**Authors**         : Sam Vickery, William D Hopkins, Chet C Sherwood, Steven J Schapiro, Jona Fischer , Robert D Latzman, Svenja Caspers, Christian Gaser, Simon B Eickhoff, Robert Dahnke , Felix Hoffstaedter         	     
**Description**     : We provide a chimpanzee structural T1w template, chimpanzee tissue probability maps (TPM), and a manual macroanatomical parcellation of the chimpanzee brain which can be interactively viewed through a web viewer. Additionally, we supply an exemplar preprocessing pipeline using CAT12 with the required templates including a chimpanzee geodesic shooting template.                   
**Documentation**   : [GitHub](https://github.com/viko18/JunaChimp)     
**Link**            : [http://junachimp.inm7.de](http://junachimp.inm7.de/)    
**Language**        : Volumetric files are in NIFTI (.nii) format, matlab                    
**Publication**     : [Vickery et al. (2020)](https://elifesciences.org/articles/60136)                     
**Communication**   : [email](mailto:s.vickery@fz-juelich.de) or [open an issue](issue at https://github.com/viko18/JunaChimp)           
**Restrictions**    : Please cite our publication if you use this resource.     

<a name="NCBR"></a>
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

