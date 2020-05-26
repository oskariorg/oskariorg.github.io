---
layout: post
title:  "Testing Oskari embedded maps and API"
excerpt : "How easy it is to create your own Oskari API based map?"
date:   2020-05-26 13:00:00 +0300
categories: [news]
---

# How easy it is to create your own Oskari API based map?

Jan Lindbom, the CPO/CTO in Sitowise Ltd explains to how to create a light weight map service with Oskari RPC.

## 1.  Access to Oskari

“You have to have access to a Oskari platform that offers this possibility,” he starts. 

So go to a service like [Paikkatietoikkuna](https://kartta.paikkatietoikkuna.fi/?lang=en), Suomi.fi-maps or similar. 

You can also try with [demo-site](https://demo.oskari.org/), but remember it will erase all saved information every day.

## 2. Sign in and add data or map layers

“You need to publish a map with Oskari's ready to use functionality with an easy to use web interface.” 

This can be done with signing in as a user, choosing a background maps or other available map layers. In this example we are using the Finnish national geoportal called Paikkatietoikkuna and some data fetched from OpenStreetMap.

- Sign in to your Oskari instance
- Add existing map layers to your map
- Add own datasets if you want (you can adjust the style also afterwards from My data-section). Notice, this is possible only if it is allowed in the used Oskari instance. 

We used QGIS and QuickOSM tool to fetch coffeeshops in the city centre of Turku), at the moment Oskari allows datasets in zip-format (ESRI shp, GPX, Mapinfo mif and Google KML). 

<img src="/img/owndatasets.png" width="500" class="img-responsive"/>

<img src="/img/edit_owndata.png" width="500" class="img-responsive"/>

## Publish the map

- Click on Map Publishing and give the map a name and the URL where you want to post it

<img src="/img/publishing.png" width="500" class="img-responsive"/>

- Adjust the needed elements and tools to the map
- Click publish and copy paste the iframe code to your website. 

<img src="/img/embedded_maps_create.png" width="500" class="img-responsive"/>

<iframe src="https://kartta.paikkatietoikkuna.fi/published/en/4fc5a1ea-6374-4ecb-a40f-3aa2f665732d" allow="geolocation" style="border: none; width: 500px; height: 500px;"></iframe>
 
## 3. If you want to tailor it to your own needs

“And the last and most important part, you need to have application developer knowledge to be able to develop the integration to the other system by RPC. You need to know the system to which you are integrating at the technical level also.”

“ The advantage of using RPC is that the map interface can be easily integrated into a part of another system and make it work interactively”, Jan explains.

Reviewed and rewritten in 2020-05-26, original story written in 2019-01-07.
