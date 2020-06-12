---
layout: post
title:  "3D capabilities of Oskari with videos"
excerpt : "3D view and terrain height profile tool"
date:   2020-06-10 13:00:00 +0300
categories: [news]
---

# Testing Oskari 3D-possibilities 

Oskari Joint Development Forum has created a video how to use 3D datasets.

## Spin the world with the Oskari demo website

If you have not tried yet, test Oskari 3D possibilities with the demo website. 

[See the whole video about 3D in demo Oskari.](https://youtu.be/ISKkL1_-svc)

1. First test the "Blue Marble" as background map and switch to 3D view [go to demo Oskari from here](https://demo.oskari.org/)
2. You can spin the globe with shift pressed down

<img src="/img/demo_bluemarble.png" class="img-responsive"/>

3. There are 2 datasets currently available with 3D data in the demo website, so let's check them out. Zoom to Helsinki (Finland). 
4. If the background map gets blurry, change the background map to e.g. "NLS-FI Background map"
5. Test the mesh dataset (Helsinki city 3D) from Helsinki and the city GML model (Helsinki city 3D buildings with textures). See how the buildings float on top of the map.

<img src="/img/helsinki_3D.png" class="img-responsive"/>


# Testing the Terrain Height Profile tool with Paikkatietoikkuna

The Finnish National Land Survey has tested the possibilities of WCS (Web Coverage Service) and created an addition to their Oskari installation called Terrain Height Profile.
It is not a core element for Oskari, but there is some documentation available [here](https://github.com/nls-oskari/kartta.paikkatietoikkuna.fi/tree/develop/service-terrain-profile). 
If you want to have similar, it depends on the data available. This is just one example on how WCS could be used. 

In Paikkatietoikkuna there is also a digital elevation model available (data comes from Cesium), so we can test how the 3D buildings go on top of the terrain model nicely.

[See the video about using Terrain profile tool](https://youtu.be/CO9tqsSHe60)


1. Open [Paikkatietoikkuna](https://kartta.paikkatietoikkuna.fi/) and switch to 3D view and zoom to Helsinki
2. Add e.g. orthophotograph and 3D model to the map view. 
You can see that the buildings are not floating on top of the terrain, due to digital elevation model provided by Cesium in the background.
3. Choose a place where you want to measure the terrain.
4. Click the terrain profile tool and start measuring.  The tool switches to 2D mode, so the measuring is more easy to do. 
End the measurement with double click. You get a profile for the terrain in a graph.
5. You can check the actual height of the terrain with following the graphs profile.

<img src="/img/3D_paikkatietoikkuna.png" class="img-responsive"/>

<img src="/img/terrainheightprofile.png" class="img-responsive"/>

An example of the [WCS Get Capabilities query used in here](https://beta-karttakuva.maanmittauslaitos.fi/wcs/service/ows?service=WCS&AcceptVersions=2.0.1&request=GetCapabilities).


