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
    <a href="templates_and_atlases">Template/Atlas</a>
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
# Resources      

Resources are categorized according to the problem or task they address. You can quickly navigate through resource categories with the button above. The analysis resources are not necessarily complete raw-to-result pipelines. They can also be tools specifically addressing an issue associated with the type of analysis they are classified under. We mostly followed the category indication we received upon contribution of the tool. If you feel a resource should be classified differently, [let us know](https://github.com/PRIME-RE/prime-re.github.io/issues/new?assignees=&labels=Contact&template=contact.md&title=[Contact]:%C2%A0%3Ctopic%3E). If any of these resources have been helpful, consider leaving a [testimonial](testimonials.md).

## Overview of resources          
### **[Templates and Atlases](templates_and_atlases.md)**
[Macaque](templates_and_atlases.md#macaque_atlases)
- [Details](templates_and_atlases_macaque.md)      
  - [D99](templates_and_atlases_macaque.md#D99)     
  - [NMT v1.3](templates_and_atlases_macaque.md#NMTv1.3)       
  - [NMT v2.0](templates_and_atlases_macaque.md#NMTv2.0)       
- [Warps between macaque templates](templates_and_atlases.md#macaque_warps)     
  - [RheMAP](templates_and_atlases/rhemap.md)    
  
[Marmoset](templates_and_atlases.md#marmoset_atlases)       
- [Details](templates_and_atlases_marmoset.md)    
  - [Marmoset Brain Connectivity Atlas](templates_and_atlases_marmoset.md#marmoset-brain-connectivity-atlas)        
  - [Marmoset Brain Mapping Atlas and Template](templates_and_atlases_marmoset.md#marmoset-brain-mapping-atlas-and-template)        
  - [Nencki-Monash Template](templates_and_atlases_marmoset.md#nencki-monash-template)

[Other species](templates_and_atlases.md#other_atlases)    


### **[General analysis](pipelines_general.md)**  
- [C-PAC](pipelines_general.md#c-pac-the-configurable-pipeline-for-the-analysis-of-connectomes) 
- [NeuroElf](pipelines_general.md#neuroelf)   

### **[Structural analysis](pipelines_structural.md)**            
- [AFNI @animal_warper](pipelines_structural.md#afni-animal_warper)   
- [BrainBox](pipelines_structural.md#brainbox)    
- [CIVET-macaque](pipelines_structural.md#civet-macaque)     
- [C-PAC](pipelines_structural.md#c-pac-the-configurable-pipeline-for-the-analysis-of-connectomes) 
- [MR Comparative Anatomy Toolbox (MrCat)](pipelines_structural.md#mr-comparative-anatomy-toolbox-mrcat)
- [Macapype](pipelines_structural.md#macapype)    
- [NHP-Freesurfer](pipelines_structural.md#nhp-freesurfer)     
- [NHP-pycortex](pipelines_structural.md#nhp-pycortex)  
- [Precon_all](pipelines_structural.md#precon_all)
- [PREEMACS](pipelines_structural.md#preemacs)
- [Reorient](pipelines_structural.md#reorient)
- [Thresholdmann](pipelines_structural.md#thresholdmann)     
- [UNet model for skull stripping and brain masks of anatomical images from PRIME-DE](pipelines_structural.md#unet-model-for-skull-stripping-and-brain-masks-of-anatomical-images-from-prime-de)     

### **[Functional analysis](pipelines_fmri.md)**
- [afni_proc.py](pipelines_fmri.md#afni_procpy)   
- [C-PAC](pipelines_fmri.md#c-pac-the-configurable-pipeline-for-the-analysis-of-connectomes) 
- [MR Comparative Anatomy Toolbox (MrCat)](pipelines_fmri.md#mr-comparative-anatomy-toolbox-mrcat)
- [NeuroElf](pipelines_general.md#neuroelf)     
- [NHP-BIDS](pipelines_fmri.md#nhp-bids)
- [NHP-pycortex](pipelines_fmri.md#nhp-pycortex)
- [Pypreclin](pipelines_fmri.md#pypreclin)     

### **[Diffusion analysis](pipelines_diffusion.md)**
- [Diffusion-MRI by Rakshit](pipelines_diffusion.md#diffusion-mri-by-rakshit) 
- [MR Comparative Anatomy Toolbox (MrCat)](pipelines_diffusion.md#mr-comparative-anatomy-toolbox-mrcat)


### **[Data sharing](data_sharing.md)**       
- [Neurovault](data_sharing.md#neurovault) 
- [Openneuro](data_sharing.md#openneuro)     
- [PRIME-DE](data_sharing.md#prime-de)       


### **[Software packages](software_packages.md)**


### **[Hardware & protocols](hardware.md)**
