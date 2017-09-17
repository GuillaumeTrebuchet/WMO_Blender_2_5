
# WMO Addon for Blender 2.5

This is an addon for Blender 2.5+ that allows import/export of World of warcraft's WMO files (v3.3.5).

<img src="images/wmo_addon_preview.png">
Not all features are supported yet, mostly because the format is obviously undocumented (and some piece of data seemed unused), but also because some features are not supported by blender at the time of the project (eg. normal editing is not supported by blender). But most usefull features are present and exported files are fully functionals.
At the time I wrote this addon, it was one of the only softwares that supported creation of WMO with collisions.

The addon works as follow : 

There is 4 new panels available.
Each one contains settings used during export.

<img align="left" src="images/wmo_addon_group_panel.png">
<b>Wow WMO group</b> panel is in Object properties, it shows options relative to wmo groups.
Group name/desc are optionnal and are just referenced from inside wmo, seems to have no effect.<br/>
This panel MUST be enabled when exporting, else export will fail.
<br/><br/><br/><br/><br/><br/>

<img align="right" src="images/wmo_addon_material_panel.png">
<b>Wow material</b> panel is in Material properties, it shows options relative to wmo shader. The only options that are exported are shown in this panel (blender materials / texture are not exported)
Materials are displayed on faces assigned to this material.<br/>
If the panel is disabled, the material is not exported and assigned faces will not be visible in game (it can still collide though)
<br/><br/><br/><br/><br/>


<img align="left" src="images/wmo_addon_collision_panel.png">
<b>Wow collision</b> panel is in Data properties and are only visible when selecting a mesh. It shows options relative to wmo collisions. "collision vertex group" specifies the vertex group whose faces will be allowed to collide.
<br/><br/><br/><br/><br/><br/><br/><br/><br/><br/>

<img align="right" src="images/wmo_addon_light_panel.png">
<b>Wow light</b> panel is in Data properties and are only visible when selecting a lamp. It shows options relative to wmo lights. This panel will probably change later.
Lights are not exported for now.
<br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/>

<b>UV</b><br/>
Only the active UV layer is exported. UV data imported are stored in "UVmap" layer.

<b>Vertex color</b><br/>
Only the active Vertex Color layer is exported. Vertex color data imported are stored in "Col" layer.
