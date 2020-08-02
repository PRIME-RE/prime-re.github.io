<head><meta name="viewport" content="width=device-width, initial-scale=1"><style>
.dropbtn {background-color: #3498DB; color: white; padding: 16px; font-size: 1rem; border: none; cursor: pointer;}
.dropbtn:hover, .dropbtn:focus {background-color: #2980B9;}
.dropdown {position: relative; display: inline-block;}
.dropdown-content {display: none; position: absolute; background-color: #f1f1f1; min-width: 100%; overflow: auto; box-shadow: 0px 8px 16px 0px rgba(0,0,0,0.2); z-index: 1; text-align: center; font-size: 1rem;}
.dropdown-content a { color: black; padding: 12px 16px; text-decoration: none; display: block;}
.dropdown a:hover {background-color: #ddd;}
.show {display: block;}
  
.dropbtn + .dropbtn { margin-left: 1rem; }
@media screen and (min-width: 64em) { .dropbtn { padding: 0.75rem 1rem; } }
@media screen and (min-width: 42em) and (max-width: 64em) { .dropbtn { padding: 0.6rem 0.9rem; font-size: 0.9rem; } }
@media screen and (max-width: 42em) { .dropbtn { display: block; width: 100%; padding: 0.75rem; font-size: 0.9rem; }
  .dropbtn + .dropbtn { margin-top: 1rem; margin-left: 0; } }
</style></head>

<center><div class="dropdown">
  <button onclick="myFunction()" class="dropbtn">Select Resource Category</button>
  <div id="myDropdown" class="dropdown-content">
    <a href="templates_and_atlases">Template/Atlas</a>
    <a href="pipelines_general">General</a>
    <a href="pipelines_structural">Structural</a>
    <a href="pipelines_fmri">Functional</a>
    <a href="pipelines_diffusion">Diffusion</a>
    <a href="data_sharing">Data sharing</a>
    <a href="software_packages">Software packages</a>
    <a href="hardware">Hardware</a>
  </div>
</div></center>

<script>
function myFunction() {document.getElementById("myDropdown").classList.toggle("show");}
window.onclick = function(event) {
  if (!event.target.matches('.dropbtn')) {
    var dropdowns = document.getElementsByClassName("dropdown-content");
    var i;
    for (i = 0; i < dropdowns.length; i++) {
      var openDropdown = dropdowns[i];
      if (openDropdown.classList.contains('show')) {
        openDropdown.classList.remove('show');
      }
    }
  }
}
</script>


# Resources      

Resources are categorized according to the problem or task they address. The resources classified under [pipelines](pipelines.md) are not necessarily complete raw-to-result pipelines. They can also be tools specifically addressing an issue associated with the type of pipeline they are classified under. We mostly followed the category indication we received upon contribution of the tool. If you feel a resource should be classified differently, [let us know](https://github.com/PRIME-RE/prime-re.github.io/issues/new?assignees=&labels=Contact&template=contact.md&title=[Contact]:%C2%A0%3Ctopic%3E). If any of these resources have been helpful, consider leaving a [testimonial](testimonials.md).
