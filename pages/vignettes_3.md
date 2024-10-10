---
title: Vignettes_3
layout: about
permalink: /vignettes_3.html
---
<div class="container text-center">
  {% include feature/image.html objectid="https://blackiowa.org/wp-content/uploads/2020/11/AAMI_horiz_fullcolor.png" width="75" alt="Welcome to AAMI's Collection of Vignettes" %}

  <h2>Welcome to AAMI's Collection of Vignettes</h2>

{% include feature/nav-menu.html sections="Churches;Explore by Location;Browse Biographies" %}

<h2> Churches </h2>

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

<h3> Browse Biographies </h3>

<div class="row mb-3 justify-content-center">
    <div class="col-md-8 text-center">
        <form role="search" id="lunrSearch" onsubmit="submitFilter(); return false;">
            <div class="input-group input-group-lg">
                <input type="text" class="form-control" id="filterTextBox" placeholder="Filter ... " aria-label="Search"> 
                <button class="btn btn-success" type="submit" title="Filter items" id="filterButton">Search</button>
                <button class="btn btn-outline-secondary filter" onclick="resetFilter(); return false;" data-filter="">Reset</button>
            </div>
        </form>
        <div class="h2" id="numberOf"></div>
    </div>
    <div class="col-md-2">
        <div class="dropdown">
            <button class="btn btn-secondary mt-1 dropdown-toggle" type="button" id="browseSortButton" data-bs-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
                Sort by <span id="sortFilter">Random</span>
            </button>
            <div class="dropdown-menu browse-sort-menu" aria-labelledby="browseSortButton">
                <button class="dropdown-item browse-sort-item active" data-filter="random">Random</button>
                <button class="dropdown-item browse-sort-item" data-filter="title">Title</button>
                <!-- Add additional sorting options if needed -->
            </div>
        </div>
    </div>
</div>

<div id="loadingIcon" class="text-center">
    <div class="spinner-border text-dark" role="status"><span class="visually-hidden">Loading...</span></div>
</div>

<div class="row" id="browseItems">
    {% assign institutionid = "aami" %}  <!-- Set the institution ID to filter by "aami" -->
    {% assign items = site.data.abvi-single-site | where: "institutionid", institution_id %}  <!-- Filter items by institution ID -->

    {% for item in items %}
        <div class="col-md-4 mb-4">
            <div class="card">
                <img class="card-img-top" src="{{ item.image_small | relative_url }}" alt="{{ item.title | escape }}">
                <div class="card-body">
                    <h5 class="card-title">{{ item.title }}</h5>
                    <p class="card-text">{{ item.description }}</p>
                    <a href="{{ '/items/' | append: item.objectid | append: '.html' | relative_url }}" class="btn btn-primary">View Item</a>
                </div>
            </div>
        </div>
    {% endfor %}
    
    {% if items.size == 0 %}
        <p>No items found for this institution.</p>
    {% endif %}
</div>
