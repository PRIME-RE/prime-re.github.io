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

# MRI monitoring of NHPs  

### Description     
Information from Magnetic Resonance Imaging (MRI) is useful for diagnosis and treatment management of human neurological patients. MRI monitoring might also prove useful for non-human animals involved in neuroscience research provided that MRI is available and feasible and that there are no MRI contra-indications precluding scanning. However, MRI monitoring is not established in macaques and a resource is urgently needed that could grow with scientific community contributions. Here we show the utility and potential benefits of MRI-based monitoring in a few diverse cases with macaque monkeys. We also establish a PRIMatE MRI Monitoring (PRIME-MRM) resource within the PRIMatE Data Exchange (PRIME-DE) and quantitatively compare the cases to normative information drawn from MRI data from typical macaques in PRIME-DE. In the cases, the monkeys presented with no or mild/moderate clinical signs, were well otherwise and MRI scanning did not present a significant increase in welfare impact. Therefore, they were identified as suitable candidates for clinical investigation, MRI-based monitoring and treatment. For each case, we show MRI quantification of internal controls in relation to treatment steps and comparisons with normative data in typical monkeys drawn from PRIME-DE. We found that MRI assists in precise and early diagnosis of cerebral events and can be useful for visualising, treating and quantifying treatment response. The scientific community could now grow the PRIME-MRM resource with other cases and larger samples to further assess and increase the evidence base on the benefits of MRI monitoring of primates, complementing the animals’ clinical monitoring and treatment regime.

### Reference & link
Balezeau, F. et al. MRI monitoring of macaque monkeys in neuroscience: Case studies, resource and normative data comparisons. *Neuroimage* 230, 117778 (2021). [https://doi.org/10.1016/j.neuroimage.2021.117778](https://doi.org/10.1016/j.neuroimage.2021.117778)    
