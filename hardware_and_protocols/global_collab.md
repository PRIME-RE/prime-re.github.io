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
# A framework and resource for global collaboration in NHP neuroscience

### Description
As science and technology evolve, there is an increasing need for promotion of international scientific exchange. Collaborations, while offering substantial opportunities for scientists and benefit to society, also present challenges for those working with animal models, such as non-human primates (NHPs). Diversity in regulation of animal research is sometimes mistaken for the absence of common international welfare standards. Here, the ethical and regulatory protocols for 13 countries that have guidelines in place for biomedical and/or neuroscience research involving NHPs were assessed with a focus on neuroscience. Review of the variability and similarity in trans-national NHP welfare regulations extended to countries in Asia, Europe and North America. A tabulated resource is established to advance solution-oriented discussions and scientific collaborations across borders. Our aim is to better inform the public and other stakeholders. Through cooperative efforts to identify and analyze information with reference to evidence-based discussion, the proposed key ingredients may help to shape and support a more informed, open framework. This framework and resource can be expanded further for biomedical research in other countries.

![image](/images/GlobalNHP.png)

  
### Reference & link
Hartig,R., Klink, P.C., Polyakova, Z., Dehaqani, M-R.A., Bondar, I., Merchant, H., Vanduffel, W., Roe, A.W., Nambu, A., Thirumala, M., Shmuel, A., Kapoor, V., Gothard, K.M., Evrard, H.C., Basso, M.A., Petkov, C.I., & Mitchell A.S (2023) A framework and resource for global collaboration in non-human primate neuroscience. *[Current Research in Neurobiology](https://doi.org/10.1016/j.crneur.2023.100079)*    
  
  
### Information tables     
The paper contains (and links) extensive information tables that can be expanded and/or corrected when additional information becomes available. This resource can be viewed as a google spreadsheet <a href="https://docs.google.com/spreadsheets/d/1hKLikEDP-x3k0fI97m_TYrXCIhaMzDhSKLTHDPMsRWk/edit?usp=sharing" target="_blank">here</a>. For suggested edits and/or additions, please use one of our [contact options](https://prime-re.github.io/contact). 
  
[![Global Tables](/images/GlobalTables.png)](https://docs.google.com/spreadsheets/d/1hKLikEDP-x3k0fI97m_TYrXCIhaMzDhSKLTHDPMsRWk/edit?usp=sharing)
  
