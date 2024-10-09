---
title: Vignettes_3
layout: about
permalink: /vignettes_3.html
---
<div class="container text-center">
  {% include feature/image.html objectid="https://blackiowa.org/wp-content/uploads/2020/11/AAMI_horiz_fullcolor.png" width="75" alt="Welcome to AAMI's Collection of Vignettes" %}

  <h2>Welcome to AAMI's Collection of Vignettes</h2>

{% include feature/nav-menu.html sections="Explore by Subject;Explore by Location;Browse Items" %}

<h3> Explore by Subject </h3>

Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.


<div class="col-md-12"> <!-- Changed to col-md-12 for full width -->
     {% include index/carousel.html %}
    
    {% comment %}
        Filter carousel items based on specific parentid
    {% endcomment %}

{%- assign specific_parentid = "institutionid" -%}  <!-- Replace with the actual parentid you want to filter by -->

    {%- assign carousel-items = site.data[site.metadata] | where_exp: 'item','item.objectid and item.parentid == institutionid' | where_exp: "item","item.image_small != nil or item.image_thumb != nil" -%}



<h3> Explore by Location </h3>

  <div class="col-md-12 p-3">
            {% include item/mini-map.html map-zoom=20 %}
            <p><strong>Geographic Coordinates:</strong> {{ page.latitude }}, {{ page.longitude }}</p>
            {% if page.location_description %}
            <p><strong>Location:</strong> {{ page.location_description }}</p>
            {% endif %}

            
        </div>

<h3> Browse Items </h3>

