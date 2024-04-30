# Export_Crowds
!!!!!IMPORTANT!!!!!!!!!

You need to have installed the "FxLabs" plugins from "sideFxLabs".


OBJ-HDA to export crowds generated in Houdini to export them to Unreal Engine or other software 
with FBX and VAT ("vertex animation texture") format.




https://github.com/AdriDevVfx/Export_Crowds/assets/54435704/a579e81a-a143-4780-8200-b7aba5ad8a77




Save the Export_crowd.otls file in the OTL folder:
.\Documents\houdinixx.x\otls

The node will appear in the OBJ context of Houdini.

== Help on how to use it ==

Select Nodes -> Select the node to export the crowds to.
Choose your way to export FBX or VAT.


#### FBX ####

-Create a network of top nodes inside a geo node("RND_FBX")
![TOPS](https://github.com/AdriDevVfx/Export_Crowds/assets/54435704/91d3da31-00e5-48a3-9d3f-0c05dacf35d8)

-Exports each character with the label of the name attribute in the folder ("$HIP")



#### VAT ####

-Create an "Export" folder in the folder ("$HIP") and each character folder contains the "geo" and "textures".

![export](https://github.com/AdriDevVfx/Export_Crowds/assets/54435704/6d7e3ec2-25de-4701-90a7-4da13ec86ee0)

-When running Render Vat creates a "geo"/"RND_VAT" node runs the node labs::vertex_animation_textures::3.0 ("side FX labs must be installed"). 
