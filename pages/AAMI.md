---
title: African American Museum Of Iowa
layout: about
permalink: /aami.html
# include CollectionBuilder info at bottom
credits: true
# Edit the markdown on in this file to describe your collection
# Look in _includes/feature for options to easily add features to the page
---

{% include feature/jumbotron.html objectid="https://blackiowa.org/wp-content/uploads/2020/11/AAMI_horiz_fullcolor.png" %} 

{% include feature/nav-menu.html sections="Collections;AAMI" %}

#Collections from the African American Museum of Iowa

The collections donated by the African American Museum of Iowa for the Amplifying Black Voices in Iowa Grant.

{%- assign items = site.data[site.metadata] | where_exp: 'item','item.objectid' -%}

<div class="row">

  <div class="col-md-8">

    {% include index/carousel.html title="Items" %}
    {% if site.data.theme.carousel-child-objects == true %}
    {% endif %}

  </div>
  <div class="col-md-4">  
        
</div>

## Collection 1

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nunc ut feugiat diam. Aenean hendrerit facilisis tellus, id viverra magna mollis tristique. Proin condimentum facilisis elit, aliquet euismod lacus pulvinar quis. Nullam et mattis libero. Sed interdum semper convallis. Curabitur auctor, ligula ut tempor lacinia, metus orci tempor purus, nec mollis ligula justo at velit. Nulla faucibus ipsum eget arcu semper rhoncus.
## Collection 2
Proin ut semper neque. Sed semper quis risus non malesuada. Etiam urna velit, finibus eu sapien at, fringilla tempor ipsum. Morbi tortor dolor, feugiat quis semper quis, tempor in diam. Fusce blandit dui in arcu finibus, non maximus dolor dignissim. Quisque id nunc ante. Aenean eu mollis leo. Donec luctus sapien sed massa pharetra, eget fermentum nulla volutpat. Praesent quis augue non sapien ullamcorper posuere ac non felis.