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
# Electrical stimulation and neuroimaging    
We are currently working on a paper on the combination of brain perturbation approaches and neuroimaging in NHP and will update these papers with collected information later.

Some additional information:

### Electrical stimulation and neuroimaging: humans and macaques         
<div class="rw-ui-container" data-title="estim_humanmacaque rating"></div>     
**Authors**         : F Rocchi\*, H Oya\*, F Balezeau, AJ Billig, Z Kocsis, RL Jenison, KV Nourski, CK Kovach, M Steinschneider, Y Kikuchi, AE Rhone, BJ Dlouhy, H Kawasaki, R Adolphs, JDW Greenlee, TD Griffiths, MA Howard III, CI Petkov 	             
**Description**     : Comparative human and monkey combined electrical stimulation and fMRI.                 
**Documentation**   : Common Fronto-temporal Effective Connectivity in Humans and Monkeys: This paper and resource establishes a comparative es-fMRI resource in human neurosurgery patients and monkeys. The work also establishes considerable correspondence between fronto-temporal auditory cognitive systems involving ventro-lateral prefrontal cortex and the hippocampus. The data in monkeys are shared via [PRIME-DE](https://fcon_1000.projects.nitrc.org/indi/indiPRIME.html) and the human data via [OpenNeuro](https://openneuro.org/). The data are also available in the [Open Science Framework](https://osf.io/arqp8). Human datasets also include the electrical tractography data.     
**Link**            : [OSF](https://osf.io/arqp8;)    
**Publication**     : Pre-accepted in Neuron             
**Communication**   : E-mail [Chris Petkov](mailto:chris.petkov@ncl.ac.uk) or [Fabien Balezeau](mailto:fabien.balezeau@ncl.ac.uk)                
**Restrictions**    : No restrictions 


Submit new content through [this issue template](https://github.com/PRIME-RE/prime-re.github.io/issues/new?assignees=&labels=new-resource&template=new-resource.md&title=%3CResource+Name%3E). 
You can also join the [PRIME-RE Mattermost-channel](https://mattermost.brainhack.org/brainhack/channels/compmri_resourcehub).
