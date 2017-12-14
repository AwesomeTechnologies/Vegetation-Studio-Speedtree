# Vegetation-Studio-Speedtree
This includes modified versions of the Unity Speedtree files. The shader supports Vegetation Studios implementation of instanced indirect rendering.

<b>SETTING UP SPEEDTREE GRASS WITH THIS SHADER</b>

Vegetation Studio can use instanced indirect rendering on vegetation. This allows the vegetation instanced to be rendered direct from a compute buffer on the GPU allowing for larger batches than the 1023 max of normal rendering. In addition to this there is a final compute shader pass before rendering that does GPU fristum culling and LOD selection.

<p align="center">
  <img src="https://www.awesometech.no/wp-content/uploads/2017/12/Image-397.png" width="350"/>
</p>

<p align="center">
  <img src="https://www.awesometech.no/wp-content/uploads/2017/12/Image-398.png" width="350"/>
</p>

<p align="center">
  <img src="https://www.awesometech.no/wp-content/uploads/2017/11/Image-399.png" width="350"/>
</p>
