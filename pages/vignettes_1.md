---
title: Vignettes_1
layout: about
permalink: /vignettes_1.html
---

<h1>Sample Case Study</h1>

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



  <div class="container mt-5">
    <div class="row">
        <div class="col-md-3">
            {% include feature/card.html text="Studio portrait of Modial Alice Snead Neal Wearing Patterned Dress" header="Alice Snead Neal" objectid="https://s3.amazonaws.com/pastperfectonline/images/museum_196/010/p20121215.jpg" %}
        </div>
        
        <div class="col-md-3">
            {% include feature/card.html text="Studio portrait of Nathanial Waites wearing a dark suit, seated in ornate chair against backdrop." header="Nathanial Waites" objectid="https://s3.amazonaws.com/pastperfectonline/images/museum_196/010/p20121220.jpg" %}
        </div>
        
        <div class="col-md-3">
            {% include feature/card.html text="Woman wearing a quarter-sleeve button-up dress seated next to a window with two embroidered pillows." header="Woman in Quarter-Sleeve Dress Posed by Window" objectid="https://s3.amazonaws.com/pastperfectonline/images/museum_196/018/p20127618.jpg" %}
        </div>
        
        <div class="col-md-3">
            {% include feature/card.html text="Black and white photograph of Cecil Reed, a prominent African American politician and businessman in Iowa. He is pictured here standing at a podium looking at the camera. Later in his career he did a lot of public speaking." header="Cecil Reed" objectid="https://s3.amazonaws.com/pastperfectonline/images/museum_196/008/p2011066.jpg" %}
        </div>
    </div>
</div>
