# Export_Crowds
!!!!!IMPORTANTE!!!!!!!!!

Es necesario tener instalado el plugins "FxLabs" de "sideFxLabs"


OBJ-HDA para exportar crowds generados en Houdini exportarlos a Unreal Engine u otro software 
con formato FBX y VAT ("vertex animation texture")




https://github.com/AdriDevVfx/Export_Crowds/assets/54435704/a579e81a-a143-4780-8200-b7aba5ad8a77




Guarda el archivo Export_crowd.hda en la carpeta OTL:
.\Documents\houdinixx.x\otls

El nodo aparecera en el contexto OBJ de Houdini

== Ayuda de uso ==

Select Nodes -> Selecciona el nodo para exportar los crowds
Elige tu forma de exportar FBX o VAT.


#### FBX ####

-Crea una red de nodos top dentro de un nodo geo("RND_FBX")
![TOPS](https://github.com/AdriDevVfx/Export_Crowds/assets/54435704/91d3da31-00e5-48a3-9d3f-0c05dacf35d8)

-Exporta cada character con el label del atributo name en la carpeta ("$HIP")



#### VAT ####

-Crea una carpeta "Export" en la carpeta ("$HIP")  y cada carpeta character  contiene la "geo" y "textures"

![export](https://github.com/AdriDevVfx/Export_Crowds/assets/54435704/6d7e3ec2-25de-4701-90a7-4da13ec86ee0)

-Al ejecutar Render Vat crea un nodo "geo"/"RND_VAT" ejecuta el nodo labs::vertex_animation_textures::3.0 ("es necesario tener side FX labs instalado ") 
