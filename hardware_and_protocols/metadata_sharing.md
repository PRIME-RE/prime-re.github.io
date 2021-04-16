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
    <a href="https://prime-re.github.io/templates_and_atlases">Template/Atlas</a>
    <a href="https://prime-re.github.io/pipelines_general">General analysis</a>
    <a href="https://prime-re.github.io/pipelines_structural">Structural analysis</a>
    <a href="https://prime-re.github.io/pipelines_fmri">Functional analysis</a>
    <a href="https://prime-re.github.io/pipelines_diffusion">Diffusion analysis</a>
    <a href="https://prime-re.github.io/pipelines_cross-species">Cross-species analysis</a>
    <a href="https://prime-re.github.io/data_sharing">Data sharing</a>
    <a href="https://prime-re.github.io/software_packages">Software packages</a>
    <a href="https://prime-re.github.io/hardware">Hardware & protocols</a>
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
# Metadata sharing

### Description
Sharing and pooling large amounts of non-human primate neuroimaging data offer new exciting opportunities to understand the primate brain. The potential of big data in non-human primate neuroimaging could however be tremendously enhanced by combining such neuroimaging data with other types of information. Here we describe metadata that have been identified as particularly valuable by the non-human primate neuroimaging community, including behavioural, genetic, physiological and phylogenetic data.

![image](/images/nhpbids_lrg.jpg)

### Reference & link
Poirier, C. et al. Beyond MRI: on the scientific value of combining non-human primate neuroimaging with metadata. *Neuroimage* 117679 (2021) [doi:10.1016/j.neuroimage.2020.117679](https://doi.org/10.1016/j.neuroimage.2020.117679).


  
