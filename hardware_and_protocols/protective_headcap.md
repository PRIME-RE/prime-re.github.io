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
# Protective cranial implant caps for macaques     

<img src="https://ars.els-cdn.com/content/image/1-s2.0-S0165027020304155-gr1_lrg.jpg" alt="headcap" width="500"/>

### Background     
Neuroscience studies with macaque monkeys may require cranial implants to stabilize the head or gain access to the brain for scientific purposes. Wound management that promotes healing after the cranial implant surgery in non-human primates can be difficult as it is not necessarily possible to cover the wound margins.

### New Method    
Here, we developed an easily modifiable head cap that protects the sutured skin margins after cranial implant surgery and contributes to wound healing. The protective head cap was developed in response to monkeys picking at sutured skin margins around an implant, complicating healing. The user-friendly protective cap, made from Klarity- R™ Sheet (3.2 mm thick with 36% or 42% perforation) is affixed to the implant post-surgically. Once secured and while the monkey is still anesthetized, the plastic sheeting is molded around the implant. The protective head cap restricts the monkey’s finger access to its’ wound margins while allowing air to circulate to promote wound healing.

### Results and comparison with existing methods    
Across two UK primate facilities, the protective head cap promoted wound healing. In monkeys that did not wear the head cap, re-suturing was necessary in ∼30% of cases. In contrast, none of the monkeys that wore the head cap required re-suturing. The monkeys wearing the head cap also had reduced numbers of days of prescribed antibiotics and analgesia.

### Conclusion    
This bespoken, easily adaptable, protective head cap supports postoperative wound healing, and enhances the welfare of monkeys involved in neuroscience research.         

### Reference & link     
Perry, Mason, Nacef, Waddle, Hynes, Bergmann, Schmid, Petkov, Thiele, & Mitchell (2020). Protective cranial implant caps for macaques, *Journal of Neuroscience Methods*, <a href="https://doi.org/10.1016/j.jneumeth.2020.108992" target="_blank">https://doi.org/10.1016/j.jneumeth.2020.108992</a>
