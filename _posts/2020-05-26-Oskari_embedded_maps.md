---
layout: post
title:  "Testing Oskari embedded maps"
excerpt : "How easy it is to create your own embedded map to your web site? So easy!"
date:   2020-05-26 13:00:00 +0300
categories: [news]
---

# How easy it is to create your own Oskari based map?

In this blog post Jan Lindbom, the CPO/CTO in Sitowise Ltd explains to how to create a light weight map service with Oskari. We shall try to do what he instructs.

## 1.  Access to Oskari

_“You have to have an access to a Oskari platform that offers the possibility to publish maps,”_ he starts. 

So go to a service like [Paikkatietoikkuna](https://kartta.paikkatietoikkuna.fi/?lang=en), [Suomi.fi-maps](https://www.maanmittauslaitos.fi/asioi-verkossa/suomifi-kartat) or similar. 

You can also try this with [Oskari demo](https://demo.oskari.org/), but remember it will erase all saved information every day.

## 2. Sign in and add data or map layers

_“You need to publish a map with Oskari's ready to use functionality with an easy to use web interface.”_

This can be done with signing in as a user, choosing a background maps or other available map layers. In this example we are using the Finnish national geoportal called Paikkatietoikkuna and some data fetched from [OpenStreetMap](https://www.openstreetmap.org/).

- **Sign in** to your Oskari instance
- Add existing map layers to your map if needed
- Add own datasets if you want and select a suitable style for your points, lines or polygons. 

The styling abilities are a bit limited. But you can adjust the style also afterwards from **My data**-section. Notice, that adding own data is possible only if it is allowed in the used Oskari instance. The abilities of Oskari can vary according to the service provider. But adding own data and publishing maps is a core element of Oskari. 

We used QGIS and QuickOSM tool to fetch coffeeshops from the city centre of Turku. At the moment Oskari allows datasets to be imported in zip-format and it supports ESRI .shp, .GPX, Mapinfo .mif and Google .KML-formats. 

<img src="/img/owndatasets.png" width="500" class="img-responsive"/>

<img src="/img/edit_owndata.png" width="500" class="img-responsive"/>

## 3. Publish the map

- Click on **Map Publishing** and give the map a name and the URL where you want to post it

<img src="/img/publishing.png" width="500" class="img-responsive"/>

<img src="/img/embedded_maps_create.png" width="500" class="img-responsive"/>

- Adjust the needed elements and tools to the map
- Click publish and copy paste the iframe code to your website. 

<iframe src="https://kartta.paikkatietoikkuna.fi/published/en/4fc5a1ea-6374-4ecb-a40f-3aa2f665732d" allow="geolocation" style="border: none; width: 500px; height: 500px;"></iframe>
 
## 4. If you want to tailor the embedded map to your own needs, learn RPC

Oskari's published maps can be tailored to make them look exactly as you like. This is done by using Oskari RPC (Remote Procedure Call).

_“And the last and most important part, you need to have application developer knowledge to be able to develop the integration to the other system by RPC. You need to know the system to which you are integrating at the technical level also.”_

_“The advantage of using RPC is that the map interface can be easily integrated into a part of another system and make it work interactively”,_ Jan explains.

- [Examples of Oskari RPC](https://oskari.org/examples/rpc-api/rpc_example.html) to tailor the embedded maps
- [Guide](https://oskari.org/guides/rpc-step-by-step)
- Check the gallery of some examples, like [Fishing restrictions](https://www.oskari.org/gallery/fishing_restrictions) and [Social insurance service search](https://www.oskari.org/gallery/kela)
- [Test the workshop material created for FOSS4G 2019](https://www.oskari.org/documentation/examples/FOSS4G_2019/workshop)

_Reviewed and rewritten in 2020-05-26, original story written in 2019-01-07._
