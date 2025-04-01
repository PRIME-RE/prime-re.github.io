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
# Software packages

This is a (non-exhaustive) list of software packages commonly used in (NHP) neuroimaging analysis. These were not submitted to PRIME-RE but are rather common in the field. Documentation will not be provided on this site, but can usually be found at the websites for the individual packages. For a similar (much better curated) list, see <a href="https://www.nitrc.org/" target="_blank">NITRC</a>.

[<img src="https://www.nitrc.org/themes/nitrc3.0/images/nitrc-logo.png" height="40">](https://www.nitrc.org/)      

If you use any of these software packages for your published work, please make sure to credit the developers. In many cases this is even a prerequisite for using the software at all. Information on how to credit a resource will usually be available on the resource's linked website. If this is not the case, and there is not an obvious methods paper you can cite, you should probably still mention the name (and url) of the tools you used when describing your methods. It increases reproducibility and recognizes the efforts of the developers that create these tools.     

If you would like to have something added to this list, please [let us know](https://github.com/PRIME-RE/prime-re.github.io/issues/new?assignees=&labels=Contact&template=contact.md&title=[Contact]:&nbsp;%3Ctopic%3E) or fill out a [new resource form](https://github.com/PRIME-RE/prime-re.github.io/issues/new?assignees=&labels=new-resource&template=new-resource.md&title=%3CResource+Name%3E).   

| **Package** &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; | **Usage** &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; | &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp;  |  
| :-- | :-- | :-: |       
| [AFNI](https://afni.nimh.nih.gov/) | Universal (f)MRI | [<img src="https://afni.nimh.nih.gov/sites/default/files/default_images/afnilogo.png" height="30" />](https://afni.nimh.nih.gov/) |         
| [ANTs](http://stnava.github.io/ANTs/) | Registration | [<img src="https://camo.githubusercontent.com/d89ec9e8fec46adc32f363c57ff5708939da8d8d/687474703a2f2f692e696d6775722e636f6d2f6d4c5a373141692e706e67" height="30" />](http://stnava.github.io/ANTs/) |        
| [BrainVISA](http://brainvisa.info/web/index.html) | Anatomy | [<img src="http://brainvisa.info/web/_static/images/brainvisa.png" height="30" />](http://brainvisa.info/web/index.html) |           
| [Brainvoyager](https://www.brainvoyager.com/) | Universal (f)MRI | [<img src="https://www.brainvoyager.com/resources/Home/BrainVoyager-v21_Snapshot1_lores.png" height="30" />](https://www.brainvoyager.com/) |     
| [CIVET](http://www.bic.mni.mcgill.ca/ServicesSoftware/CIVET) | Cortical surface analysis | [<img src="https://mcin.ca/wp-content/uploads/2017/06/gray-left-overlay-medial-clear.png" height="30" />](http://www.bic.mni.mcgill.ca/ServicesSoftware/CIVET) |         
| [Connectome Workbench](https://www.humanconnectome.org/software/connectome-workbench) | Universal MRI  | [<img src="https://www.humanconnectome.org/themes/uar_washu/assets/images/logos/ccf-logo-mobile.png" height="30" />](https://www.humanconnectome.org/software/connectome-workbench) |         
| [dcm2niix](https://www.nitrc.org/plugins/mwiki/index.php/dcm2nii:MainPage) | Convert dcm to nifti | [<img src="https://www.mccauslandcenter.sc.edu/mricrogl/sites/sc.edu.mricrogl/files/mni320_0.png" height="30" />](https://www.nitrc.org/plugins/mwiki/index.php/dcm2nii:MainPage) |         
| [DSI Studio](http://dsi-studio.labsolver.org/) | Tractography | [<img src="http://dsi-studio.labsolver.org/_/rsrc/1468760876817/config/customLogo.gif?revision=17" height="30" />](http://dsi-studio.labsolver.org/) |         
| [Freesurfer](https://surfer.nmr.mgh.harvard.edu/) | Universal MRI. Surface generation. Segmentation. | [<img src="https://surfer.nmr.mgh.harvard.edu/fscortex.png" height="30" />](https://surfer.nmr.mgh.harvard.edu/) |         
| [FSL](https://fsl.fmrib.ox.ac.uk/fsl/fslwiki) | Universal (f)MRI | [<img src="https://fsl.fmrib.ox.ac.uk/fsl/wiki_static/fsl/img/fsl-logo-x2.png" height="30" />](https://fsl.fmrib.ox.ac.uk/fsl/fslwiki) |   
| [Horos](https://horosproject.org/) | Dicom viewer. Open source OsiriX alternative | [<img src="https://horosproject.org/wp-content/uploads/2018/02/horos-blue-circle.png" height="30" />](https://horosproject.org/) |              
| [InVesalius](https://invesalius.github.io/) | 3D reconstruction | [<img src="https://d2.alternativeto.net/dist/icons/invesalius-3_88840.png?width=200&height=200&mode=crop&upscale=false" height="30" />](https://invesalius.github.io/) |                   
| [ITK-SNAP](http://www.itksnap.org/pmwiki/pmwiki.php) | Segmentation and 3D | [<img src="http://www.itksnap.org/Artwork/snaplogo3.png" height="30" />](http://www.itksnap.org/pmwiki/pmwiki.php) |         
| [JIP](http://www.nmr.mgh.harvard.edu/~jbm/jip/jip-align/) | Registration | [<img src="http://www.nmr.mgh.harvard.edu/~jbm/jip/_Media/align_med.jpeg" height="30" />](http://www.nmr.mgh.harvard.edu/~jbm/jip/jip-align/) |               
| [Lead-DBS](https://www.lead-dbs.org/) | Connectome | [<img src="https://www.lead-dbs.org/wp-content/uploads/logo_icon.png" height="30" />](https://www.lead-dbs.org/) |         
| [MedInria](https://med.inria.fr/) | Image processing and viewing | [<img src="https://avatars2.githubusercontent.com/u/2675371?s=200&v=4" height="30" />](https://med.inria.fr/) |          
| [MIPAV](https://mipav.cit.nih.gov/) | Image processing and viewing | [<img src="https://mipav.cit.nih.gov/about.asp_files/splash.gif" height="30" />](https://mipav.cit.nih.gov/) |         
| [MRIcro(GL)](https://www.mccauslandcenter.sc.edu/crnl/mricro) | Image viewing 3D | [<img src="https://www.mccauslandcenter.sc.edu/mricrogl/sites/sc.edu.mricrogl/files/mni320_0.png" height="30" />](https://www.mccauslandcenter.sc.edu/crnl/mricro) |  
| [MRtrix3](https://mrtrix.org/) | Tractography | [<img src="https://www.mrtrix.org/images/frontpage/tractography.jpg" height="30" />](https://mrtrix.org/) |                 
| [mrVista](https://web.stanford.edu/group/vista/cgi-bin/wiki/index.php/MrVista) | Universal (f)MRI | [<img src="https://vistalab.stanford.edu/wp-content/uploads/2013/01/mrMesh.png" height="30" />](https://web.stanford.edu/group/vista/cgi-bin/wiki/index.php/MrVista) |           
| [OsiriX](https://www.osirix-viewer.com/) | DICOM viewer | [<img src="https://web.stanford.edu/group/vista/wikiupload/d/dd/MeshVisualize.jpg" height="30" />](https://www.osirix-viewer.com/) |         
| [Slicer 3D](https://www.slicer.org/) | Versatile image processing 3D | [<img src="https://www.slicer.org/img/3DSlicerLogo-H-Color-218x144.png" height="30" />](https://www.slicer.org/) |         
| [SPM](https://www.fil.ion.ucl.ac.uk/spm/) | Universal fMRI | [<img src="https://www.fil.ion.ucl.ac.uk/spm/images/spm.svg" height="30" />](https://www.fil.ion.ucl.ac.uk/spm/) |         
| [TrackVis](http://trackvis.org/) | Tractography | [<img src="http://trackvis.org/images/trackvis_prospective.png" height="30" />](http://trackvis.org/) |       

### Python based solutions

| **Package** &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; | **Usage** &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; | &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp;  |  
| :-- | :-- | :-: |      
| [Pycortex](https://github.com/gallantlab/pycortex) | Volumes and surfaces | [<img src="https://gallantlab.github.io/pycortex/_images/3dhead.png" height="30" />](https://github.com/gallantlab/pycortex) |         
| [NiPype](https://nipype.readthedocs.io/en/latest/) | Pipelines | [<img src="https://nipype.readthedocs.io/en/latest/_static/nipype-banner-bg.png" height="30" />](https://nipype.readthedocs.io/en/latest/) |         
| [NiPy](https://nipy.org/) | A collection of more Python resources | [<img src="https://nipy.org/img/nipy.svg" height="30" />](https://nipy.org/) |         
| [Nilearn](https://nilearn.github.io/) | Statistical learning and plotting | [<img src="https://nilearn.github.io/_static/nilearn-logo.png" height="30" />](https://nilearn.github.io/) | 
