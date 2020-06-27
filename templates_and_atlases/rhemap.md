## RheMAP    

![RheMAP logo](RheMAP_logo.png)    
<div class="rw-ui-container" data-title="rhemap rating"></div>

|                     |                                                                                         |
| :------------------ | :-------------------------------------------------------------------------------------- |
| **Name**            | RheMAP                                                                                  |    
| **Authors**         | [Nikoloz Sirmpilatze](https://github.com/niksirbi) (German Primate Center)<br>[Chris Klink](https://github.com/pcklink) (Netherlands Institute for Neuroscience)      |
| **Description**     | Non-linear warps across a set of the most common rhesus macaque brain templates.        |
| **Documentation**   | [RheMAP on GitHub](https://github.com/PRIME-RE/RheMAP)                                  |
| **Link**            | [Dataset of warps and warped templates at Zenodo](https://doi.org/10.5281/zenodo.3668510) |
| **Language**        | [RheMAP on GitHub](https://github.com/PRIME-RE/RheMAP) includes Jupyter notebooks in Python |
| **Publication**     | Sirmpilatze, Nikoloz and Klink, P. Christiaan (2020). RheMAP: Non-linear warps between common rhesus macaque brain templates (Version 1)[Data set]. Zenodo. https://doi.org/10.5281/zenodo.3668510|
| **Communication**   | <p.c.klink@gmail.com>                                                                   |
| **Restrictions**    | Please cite the Zenodo dataset when you use this in your work                           |
    
[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.3668510.svg)](https://doi.org/10.5281/zenodo.3668510)

![RheMAP graphic](RheMAP_graphic.png)



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
