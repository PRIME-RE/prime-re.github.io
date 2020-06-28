
---

##### [Template/Atlas](templates_and_atlases.md) &nbsp;  - &nbsp;  [General](pipelines_general.md) &nbsp;  - &nbsp;  [Structural](pipelines_structural.md) &nbsp;  - &nbsp;  [fMRI](pipelines_fmri.md) &nbsp;  - &nbsp;  [Diffusion](pipelines_diffusion.md) &nbsp;  - &nbsp;  [Data](data_sharing.md) &nbsp;  - &nbsp; [Software packages](software_packages.md)  &nbsp;  - &nbsp; [Hardware](hardware.md)          
---    

# Macaque templates and atlases

Jump to:
- [macaque](templates_and_atlases_macaque.md)
- [marmoset](templates_and_atlases_marmoset.md)  

<br>     

## Overview     
- [D99](templates_and_atlases_macaque.md#D99)     
- [NMT v1.3](templates_and_atlases_macaque.md#NMTv1.3)     
- [NMT v2.0](templates_and_atlases_macaque.md#NMTv2.0)

<br>     

## Details

<a name="D99"></a>
### D99 Template and Atlas       
<div class="rw-ui-container" data-title="d99 rating"></div>    
**Authors**         : Saleem KS, Reveley C, Gruslys A, Ye FQ, Glen D, Samaha J, Russ BE, Saad Z, Seth AK, Leopold DA	     
**Description**     : Digital version of the Saleem and Logothetis atlas with a newer, higher quality D99 surrogate MRI template. Integrated into AFNI/SUMA software.                                         
**Documentation**   : [AFNI site](https://afni.nimh.nih.gov/Macaque)     
**Link**            : [https://afni.nimh.nih.gov/pub/dist/atlases/macaque](https://afni.nimh.nih.gov/pub/dist/atlases/macaque/)    
**Language**        : NIFTI format     
**Publication**     : [Reveley et al. (2016)](https://doi.org/10.1093/cercor/bhw248)                     
**Communication**   : [email](mailto:kadharbatcha.saleem.ctr@usuhs.edu), [AFNI message board](https://afni.nimh.nih.gov/afni/community/board/list.php?1)    
**Restrictions**    : None

<a name="NMTv1.3"></a>
### NMT v1.3 (NIMH Macaque Template - version 1.3)       
<div class="rw-ui-container" data-title="nmt1 rating"></div>    
**Authors**         : Adam Messinger, Benjamin Jung, Jakob Seidlitz, Paul Taylor, Daniel Glen	             
**Description**     : A volumetric template of the rhesus macaque created by nonlinear averaging of T1-weighted anatomical MRIs from multiple adult monkeys. Surface files are included. Version 1.3 updates include: an improved mapping of the D99 atlas, improved brain masking and normalization, and files that are defined in a common template space (NMT space), using the short data type for improved storage efficiency.                                   
**Documentation**   : [Github](https://github.com/jms290/NMT/blob/master/NMT_v1.3/README.md)     
**Link**            : [Github](https://github.com/jms290/NMT/tree/master/NMT_v1.3)    
**Language**        : Volumetric files are in NIFTI (.nii) format, while surface files are in GIFTI (.gii) format. Scripts for processing single subjects rely on bash shell and AFNI. Some scripts also require ANTs.                        
**Publication**     : Seidlitz, J., Sponheim, C., Glen, D., Ye, F.Q., Saleem, K.S., Leopold, D.A., Ungerleider, L., Messinger, A. A population MRI brain template and analysis tools for the macaque. NeuroImage 170:121-131 (2018). [https://doi.org/10.1016/j.neuroimage.2017.04.063](https://doi.org/10.1016/j.neuroimage.2017.04.063)                       
**Communication**   : Through the GitHub repo or via email to [Dr. Adam Messinger](mailto:Adam.Messinger@nih.gov)                       
**Restrictions**    : To use the NMT_v1.3 cite the above article:  [Seidlitz et al., (2018)](https://doi.org/10.1016/j.neuroimage.2017.04.063). To use the D99 atlas cite [Reveley et al. (2016)](https://doi.org/10.1093/cercor/bhw248).

<a name="NMTv2.0"></a>
### NMT 2.0 Templates (NIMH Macaque Template - version 2.0)   
<div class="rw-ui-container" data-title="nmt2 rating"></div>    
**Authors**         : Adam Messinger, Benjamin Jung, Jakob Seidlitz, Paul Taylor, Daniel Glen    	             
**Description**     : A collection of volumetric templates of the rhesus macaque created by nonlinear averaging of T1-weighted anatomical MRIs from multiple adult monkeys.  Surface files are included. The NMT 2.0 provides increased flexibility in macaque group analysis by providing symmetric and asymmetric templates. Both templates are available with an expanded, full head field of view.  The templates are available in both AC-PC orientation and in Horsley-Clarke stereotaxic orientation. Updates to the templates include:  an improved mapping of the D99 atlas, improved brain masking and normalization, and files that are defined in a common template space (NMT space), using the short data type for improved storage efficiency.                                   
**Documentation**   : TBD     
**Link**            : TBD    
**Language**        : Volumetric files are in NIFTI (.nii) format, while surface files are in GIFTI (.gii) format. Scripts for processing single subjects rely on bash shell and AFNI. Some scripts also require ANTs.                        
**Publication**     : TBD                       
**Communication**   : Through the GitHub repo or via email to [Dr. Adam Messinger](mailto:Adam.Messinger@nih.gov)         
**Restrictions**    : Usage requires citation of this article: TBD



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
