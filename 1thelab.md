---
layout: page
title: The Leiboff Lab
permalink: /thelab/
---

Current People
==================
<div>
  {% for current_people in site.current_people %}
      <div style="overflow: hidden;">
        <table style="width:100%">
          <tr>
            <td style="width:40%">
              <div>
                {% if current_people.profile-image %}
                {% include people-profile-image.html image=current_people.profile-image alt=current_people.profile-image-alt %}
                {% endif %}
              </div>
            </td>
            <td>
              <div>
                <h2><a href="{{ current_people.url }}">{{ current_people.name }}</a></h2>
                <h3>{{ current_people.position }}</h3>
                <p>{{ current_people.content | markdownify }}</p>
              </div>
            </td>
          </tr>
        </table>
      </div>
  {% endfor %}
</div>

***  

<br>

Places
==================

The Lab @ [3618 Cordley Hall][cord]{:target="_blank"}
------------------
![alt text][lab]{:style="float: right;padding: 10px" height="50%" width="50%"} The Leiboff Lab consists of 2400+ sqft of collaborative research space, shared with the labs of [Dr. Molly Megraw][megrawlab_website]{:target="_blank"} and [Dr. John Fowler][fowlerlab_website]{:target="_blank"} within the Oregon State University, College of Agricultural Sciences, Department of Botany and Plant Pathology. Our remodeled space was opened in Summer 2022 and provides a modern lab environment.  

To examine development at the cellular level, we have a Leica DMi8 THUNDER inverted microscope and a Leica M205 FCA THUNDER stereoscope, which enables studies of entire tissues and live plant dissections. Both scopes are equipped with epifluorescence and Leica's THUNDER computational dehazing method for near-subcellular resolution. We routinely use paraffin-embeded tissue histology and the preparation of microscope slides for plant anatomy.

![alt text][dmi8]{:style="float: center;padding: 5px" height="95%" width="95%"} | ![alt text][fca205]{:style="float: center;padding: 5px" height="95%" width="95%"}

The lab has typical molecular biology equipment, including thermal cyclers, incubators, and centrifuges. Through the Botany and Plant Pathology department, we also have access to high throughput tissue homogenization tools, a liquid handling robotics platform, qRT-PCR machines, cell sorting equipment, and a walk in seed storage room. Through the OSU [Center for Quantitative Life Sciences][cqls_website]{:target="_blank"}, we have access to confocal microscopy, genomic library preparation / sequencing, and priority queing for high performance computing.

[lab]: /assets/thelab.jpg "Lab space at Cordley Hall"

[dmi8]: /assets/tamara.jpg "Inverted epifluorescence miscroscope"
[fca205]: /assets/tia.jpg "Epifluorescence stereoscope"

[cord]: https://goo.gl/maps/StWsL3s41pgCmgjV6
[megrawlab_website]: http://megraw.cgrb.oregonstate.edu/
[fowlerlab_website]: https://bpp.oregonstate.edu/users/john-fowler-jr?gid=184

[cqls_website]: https://cqls.oregonstate.edu/core

The Greenhouse
------------------

The lab occupies a 700 sqft climate-controlled greenhouse where maize and other large grasses can be grown year-round. Plant care, including watering and integrated pest management are conducted by College of Agricultural Sciences Greenhouse Operations Unit.

![alt text][gh]{:style="float:center"} | ![alt text][plants]{:style="float:center"}

[gh]: /assets/gh.jpg "Leiboff Lab greenhouse"
[plants]: /assets/large_grasses.jpg "We can grow some big plants!"

The Nursery @ [the OSU BPP Farm][farm]{:target="_blank"}
------------------
![alt text][field]{:style="float: right;padding: 10px" height="40%" width="40%"}  The lab plants a 1-acre summer nursery at the [OSU Botany and Plant Pathology Farm][BPP_farm_website]{:target="_blank"}. Field preparation, treatment, and watering are managed by the Botany Field Lab manager and staff. Most North America-adapted maize and sorghum germplasm grows well during our mild, dry summers. Our field season is typically June - October, with our spooky corn collected in time for Halloween.

[field]: /assets/field.jpg "Leiboff Lab summer nursery"

[BPP_farm_website]: https://agsci.oregonstate.edu/botany-field-lab/botany-field-lab
[farm]: https://goo.gl/maps/yjeQgn78sH1FsKA56

<br>

***

*Past People*
==================
<div class="grid-container">
  {% for past_people in site.past_people %}
      <div class="grid-item">
        <h2><a href="{{ past_people.url }}">{{ past_people.name }}</a></h2>
        <h3>{{ past_people.position }}</h3>
        <div style="overflow: hidden; width:50%">
        {% if past_people.profile-image %}
        {% include people-profile-image.html image=past_people.profile-image alt=past_peopleprofile-image-alt %}
        {% endif %}
        </div>
      </div>
  {% endfor %}
</div>
