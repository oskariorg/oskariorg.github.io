---
layout: post
title:  "What is Oskari RPC?"
excerpt : "Oskari API is a really nice option for creating light weight map services"
date:   2019-01-09 13:00:00 +0300
categories: [news]
---

# Why choose Oskari API over Oskari installation?

In 2018 I requested Marko Kauppi from Ubigu Ltd to describe where he sees Oskari should be going in the future and he replied:

_"It would be interesting to see more services that utilizes Oskari’s API which is created with RPC technology."_

So let’s go into the realm of the elusive RPC a little bit. 
Oskari setups are usually quite extensive with lots of different datasets and tools (check out for example [Liiteri - service for environmental information](https://liiteri.ymparisto.fi/) or [Regional information service in SW Finland](http://karttapalvelu.lounaistieto.fi/)).

But then there are services focusing on only one theme, like for example [Fishing restrictions](https://kalastusrajoitus.fi/) which 
offers the possibility for their users to check what are the fishing limitations in a requested area. 
City of Tampere offers a [feedback service for tram planning](https://kartat.tampere.fi/raitiotieallianssi/) and National Land Survey of Finland has their own lean client interface called [Mapsite](https://asiointi.maanmittauslaitos.fi/karttapaikka/?lang=en). As we have told you before, Kela (Social Insurance Institute) recently opened their service for [finding your nearest social service point](https://oskari.org/gallery/kela) and GI learning portal [PaikkaOppi was renewed](https://oskari.org/gallery/paikkaoppi).

They are all examples of utilizing Oskari API.

## If you do not have the resources to setup your own Oskari instance 

Take ruthlessly advantage of those offering the published maps functionality. You can use the service provided by say [Suomi.fi maps](https://verkosto.oskari.org/en/suomi_fi/) or [Paikkatietoikkuna](http://www.paikkatietoikkuna.fi/) and create an embedded map and customize it with available RPC tools. This way you can enhance and modify the map service and make it talk to your own site.

RPC actually means [Remote Procedure Call](https://en.wikipedia.org/wiki/Remote_procedure_call) - so retrieving tools to a client from a service providing this technology. 
The map in the examples are created with some already existing Oskari installation and RPC is a way for the website to talk with the embedded map 
and request needed functionalities from the master Oskari installation.

RPC tech is now being tested in several other services as well; 
Finnish Heritage Agency has stated that they are currently developing a map service for [reporting archeological findings](https://verkosto.oskari.org/en/reporting-archaeological-findings-with-rpc/) with 
RPC and Helsinki Region Environmental Services Authority (HSY) are creating a climate atlas with Oskari API.

## RPC use is spreading

This is something that also Ubigu Ltd is looking for.

_"I hope that Oskari could be easily tailored to different map needs from functionality to visual appearance"_, continues Kauppi.

Maybe RPC could be the solution?

Here are some tips [for developers](https://github.com/oskariorg/rpc-client) to use RPC technology and the [request examples](http://oskari.org/examples/rpc-api/rpc_example.html).

Thanks for the comments Marko, and let's hope that we will see more Oskari API examples this spring!

Story by Sanna Jokela,
Oskari communication coordinator
