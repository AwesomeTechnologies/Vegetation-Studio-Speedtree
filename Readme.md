# Vegetation-Studio-Speedtree
This includes modified versions of the Unity Speedtree files. The shader supports Vegetation Studios implementation of instanced indirect rendering.

<b>SETTING UP SPEEDTREE GRASS WITH THIS SHADER</b>

This version is based on the 5.6 version of Unity. Look at the other branches for newer versions. Select the version closest (bellow) your current Unity version.

Vegetation Studio can use instanced indirect rendering on vegetation. This allows the vegetation instanced to be rendered direct from a compute buffer on the GPU allowing for larger batches than the 1023 max of normal rendering. In addition to this there is a final compute shader pass before rendering that does GPU fristum culling and LOD selection.

To set up download the files from github to your Unity project. 
Make a prefab of the Speedtree grass and change the shader on all LODs like in the image. 

<p align="center">
  <img src="https://www.awesometech.no/wp-content/uploads/2017/12/Image-397.png" width="350"/>
</p>

Then add the prefab as normal to Vegetation Studio and set the render mode to Instanced Indirect.

<p align="center">
  <img src="https://www.awesometech.no/wp-content/uploads/2017/12/Image-398.png" width="350"/>
</p>

Go to the Render tab of the Vegetation System component and make sure compute shaders and GPU culling is enabled.

<p align="center">
  <img src="https://www.awesometech.no/wp-content/uploads/2017/12/Image-399.png" width="350"/>
</p>

The speedtree grass should now work with instanced indirect. 

See branches for shaders based on other unity releases. 
