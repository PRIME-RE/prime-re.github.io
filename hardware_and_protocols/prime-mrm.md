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

### PRIME-MRM: MRI monitoring of monkeys in neuroscience    
<div class="rw-ui-container" data-title="PRIME-MRM rating"></div>    
**Authors**         : F Balezeau, J Nacef, Y Kikuchi, F Schneider, F Rocchi, RS Muers, R Fernandez-Palacios O’Connor, C Blau, B Wilson, RC Saunders, M Howard III, A Thiele, TD Griffiths, *CI Petkov & *K Murphy (* joint senior authors)                                                                    
**Description**     : Information from Magnetic Resonance Imaging (MRI) is useful for diagnosis and treatment management of human neurological patients. MRI monitoring might also prove useful for non-human animals involved in neuroscience research provided that MRI is available and feasible and that there are no MRI contra-indications precluding scanning. We establish an MRI Monitoring (PRIME-MRM) resource within the PRIMatE Data Exchange (PRIME-DE) and encourage submissions by the scientific community to grow the resource and the evidence base on MRI monitoring. The community is also encouraged to contribute to PRIME-RE to gow the resource exchange linked to PRIME-MRM.      
**Documentation**   : For more information, please see the PRIME-DE contributions linked under PRIME-MRM for the data. The forthcoming paper (Balezeau et al.) provides further information on how to contribute, how MRI monitoring could be useful and how to grow the evidence base including quantification in relation to normative data on PRIME-DE. For the initial cases contributed, we show MRI quantification of internal controls in relation to treatment steps and comparisons with normative data in typical monkeys drawn from PRIME-DE. MRI monitoring can assist in precise and early diagnosis of cerebral events and can be useful for visualising, treating and quantifying treatment response. The scientific community is encouraged to grow the PRIME-MRM resource with other cases and larger samples to further assess and increase the evidence base on the benefits of MRI monitoring of primates, complementing the animals’ clinical monitoring and treatment regime. We also suggest in the paper a set of basic scans that can serve as a basic scan toolkit, as well as a more extensive set of scans as needed. We will be compiling a list of veterinary, radiology or clinicians that could be consulted or provide further guidance. We encourage a brief animal history and any diagnostic information to be included as meta data on PRIME-DE contributions.                                           
**Link**            : [PRIME-DE](https://fcon_1000.projects.nitrc.org/indi/indiPRIME.html )               
**Language**        : n/a                                                       
**Publication**     : forthcoming, currently under minor revision               
**Communication**   : Email [Chris Petkov](mailto:chris.petkov@ncl.ac.uk) or [Fabien Balezeau](mailto:fabien.balezeau@ncl.ac.uk)                                                  
**Restrictions**    : None    
