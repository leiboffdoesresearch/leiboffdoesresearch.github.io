---
layout: page
title: The Leiboff Lab
permalink: /thelab/
---

People
==================
<div>
  {% for current_people in site.current_people %}
      <div style="overflow: hidden;">
        {% if current_people.profile-image %}
        {% include people-profile-image.html image=current_people.profile-image alt=current_peopleprofile-image-alt %}
        {% endif %}
      <h2><a href="{{ current_people.url }}">{{ current_people.name }}</a></h2>
      <h3>{{ current_people.position }}</h3>
      <p>{{ current_people.content | markdownify }}</p></div>
  {% endfor %}
</div>

<br>

***

<br>

Places
==================

The Lab @ [RWLB][rwlb]{:target="_blank"}
------------------
![alt text][lab]{:style="float: right;padding: 10px" height="50%" width="50%"} The Leiboff Lab consists of 3200+ sqft of collaborative research space, shared with the labs of [Dr. Molly Megraw][megrawlab_website]{:target="_blank"} and [Dr. John Fowler][fowlerlab_website]{:target="_blank"}s within the Oregon State University, College of Agricultural Sciences, Department of Botany and Plant Pathology. We anticipate moving back to the OSU main campus Summer 2022.  

To examine development at the cellular level, we have a Leica DMi8 THUNDER inverted microscope and a Leica M205 FCA THUNDER stereoscope, which enables studies of entire tissues and live plant dissections. Both scopes are equipped with epifluorescence and Leica's THUNDER computational dehazing method for near-subcellular resolution. We routinely use paraffin-embeded tissue histology and the preparation of microscope slides for understanding features of plant anatomy.  

The lab has typical molecular biology equipment, including thermal cyclers, incubators, and centrifuges. Through the Botany and Plant Pathology department, we also have access to high throughput tissue homogenization tools, a liquid handling robotics platform, qRT-PCR machines, and cell sorting equipment.


[lab]: /assets/thelab.jpg "Lab space at RWLB"

[rwlb]: https://goo.gl/maps/tLe8hvsx63zKZyW96
[megrawlab_website]: http://megraw.cgrb.oregonstate.edu/
[fowlerlab_website]: https://bpp.oregonstate.edu/users/john-fowler-jr?gid=184

The Greenhouse
------------------
![alt text][gh]{:style="padding: 10px"}  The lab occupies a 700 sqft climate-controlled greenhouse where maize and other large grasses can be grown year-round. For full spectrum lighting we use [VOLT LED growlights][volt_website]{:target="_blank"}. Plant care, including watering and integrated pest management are conducted by College of Agricultural Sciences Greenhouse Operations Unit.

[gh]: /assets/gh.jpg "Leiboff Lab greenhouse"
[plants]: /assets/large_grasses.jpg "We can grow some big plants!"

[volt_website]: https://www.voltlighting.com/led-grow-lights/shop-grow-lights

The Nursery @ [the OSU BPP Farm][farm]{:target="_blank"}
------------------
![alt text][field]{:style="float: left;padding: 10px" height="50%" width="50%"}  The lab plants a 1-acre summer nursery at the [OSU Botany and Plant Pathology Farm][BPP_farm_website]{:target="_blank"}. Field preparation, treatment, and watering are managed by the awesome Botany Field Lab manager and staff. Most NA-adapted maize and sorghum germplasm grows well during our mild, dry summers. Our field season is typically June - October, with our spooky corn collected in time for Halloween.

[field]: /assets/field.jpg "Leiboff Lab summer nursery"

[BPP_farm_website]: https://agsci.oregonstate.edu/botany-field-lab/botany-field-lab
[farm]: https://goo.gl/maps/yjeQgn78sH1FsKA56
