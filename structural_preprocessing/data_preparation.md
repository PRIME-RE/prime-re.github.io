
# 1. Structural preprocessing

## Description
Several steps to obtain a segmented brain with possibility to create surfaces

<a name="issues"></a> 
## Issues linked to NHP imaging
- non standard orientation: sphinx position, oblique orientation
<div style="text-align:center">
<img src="../images/misorientation.png" style="position:absolute; top:-10px; left:-30px; width:80px; height:80px; border:none;"  width="400" align="middle">
</div>
- strong intensity bias due to a huge variety of coils used
<img src="../images/bias.png" width="300" align="middle">
- large FOV / non brain tissue
<img src="../images/non_brain.png" width="400" align="middle">

<a name="steps"></a> 
## Steps
<a name="steps"></a> 
### Preparation of data (Cropping, deoblique…)

- **What is is about?**

- **Solutions**
<a name="registration"></a>  
### Registration to template
<a name="extraction"></a> 
### Brain extraction / skull stripping
<a name="segmentation"></a> 
### Segmentation (GM, WM, CSF? Subcortical?bone, non brain soft tissue? air?)
<a name="surf"></a> 
### Surface generation
<a name="measures"></a> 
### Morphometry measures (thickness, curvature etc)

<a name="links"></a> 
## Links to pipelines

<a name="communication"></a> 
## Communication
Link to the communication channel for your project. You can, for example, create a [slack channel](https://brainhack-slack-invite.herokuapp.com/) for your project inside the Brainhack slack community, and include a slack badge [![slack_brainhack_3](https://user-images.githubusercontent.com/6297454/47951457-5b37b780-df61-11e8-9d77-7b5a4c7af875.png)](https://brainhack-slack-invite.herokuapp.com/) to invite people to Brainhack slack, where they can then find and join your channel.  
Or create a community on [gitter](https://gitter.im/) and link to the chat by including a Gitter badge linking to your community 
[![Gitter chat](https://badges.gitter.im/gitterHQ/gitter.png)](https://gitter.im/yourRoom/Lobby#)







