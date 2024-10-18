---
title: Vignettes_2
layout: about
permalink: /vignettes_2.html
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

  <div class="row">
    <div class="col-md-3">
      <div class="card">
        <img src="https://s3.amazonaws.com/pastperfectonline/images/museum_196/010/p20121215.jpg" class="card-img-top" alt="Alice Snead Neal">
        <div class="card-body">
          <h5 class="card-title">Alice Snead Neal</h5>
          <button type="button" class="btn btn-secondary" data-toggle="modal" data-target="#modalAlice">
            Explore
          </button>
        </div>
      </div>

      <!-- Modal for Alice Snead Neal -->
      <div class="modal fade" id="modalAlice" tabindex="-1" role="dialog" aria-labelledby="modalAliceLabel" aria-hidden="true">
        <div class="modal-dialog" role="document">
          <div class="modal-content">
            <div class="modal-header">
              <h5 class="modal-title" id="modalAliceLabel">Alice Snead Neal</h5>
              <button type="button" class="close" data-dismiss="modal" aria-label="Close">
                <span aria-hidden="true">&times;</span>
              </button>
            </div>
            <div class="modal-body">
              <p>Studio portrait of Modial Alice Snead Neal Wearing Patterned Dress.</p>
            </div>
            <div class="modal-footer">
              <button type="button" class="btn btn-secondary" data-dismiss="modal">Close</button>
            </div>
          </div>
        </div>
      </div>
    </div>

    <div class="col-md-3">
      <div class="card">
        <img src="https://s3.amazonaws.com/pastperfectonline/images/museum_196/010/p20121220.jpg" class="card-img-top" alt="Nathanial Waites">
        <div class="card-body">
          <h5 class="card-title">Nathanial Waites</h5>
          <button type="button" class="btn btn-secondary" data-toggle="modal" data-target="#modalNathanial">
            Explore
          </button>
        </div>
      </div>

      <!-- Modal for Nathanial Waites -->
      <div class="modal fade" id="modalNathanial" tabindex="-1" role="dialog" aria-labelledby="modalNathanialLabel" aria-hidden="true">
        <div class="modal-dialog" role="document">
          <div class="modal-content">
            <div class="modal-header">
              <h5 class="modal-title" id="modalNathanialLabel">Nathanial Waites</h5>
              <button type="button" class="close" data-dismiss="modal" aria-label="Close">
                <span aria-hidden="true">&times;</span>
              </button>
            </div>
            <div class="modal-body">
              <p>Studio portrait of Nathanial Waites wearing a dark suit, seated in ornate chair against backdrop.</p>
            </div>
            <div class="modal-footer">
              <button type="button" class="btn btn-secondary" data-dismiss="modal">Close</button>
            </div>
          </div>
        </div>
      </div>
    </div>

    <div class="col-md-3">
      <div class="card">
        <img src="https://s3.amazonaws.com/pastperfectonline/images/museum_196/018/p20127618.jpg" class="card-img-top" alt="Woman in Quarter-Sleeve Dress">
        <div class="card-body">
          <h5 class="card-title">Woman in Quarter-Sleeve Dress</h5>
          <button type="button" class="btn btn-secondary" data-toggle="modal" data-target="#modalWoman">
            Explore
          </button>
        </div>
      </div>

      <!-- Modal for Woman in Quarter-Sleeve Dress -->
      <div class="modal fade" id="modalWoman" tabindex="-1" role="dialog" aria-labelledby="modalWomanLabel" aria-hidden="true">
        <div class="modal-dialog" role="document">
          <div class="modal-content">
            <div class="modal-header">
              <h5 class="modal-title" id="modalWomanLabel">Woman in Quarter-Sleeve Dress</h5>
              <button type="button" class="close" data-dismiss="modal" aria-label="Close">
                <span aria-hidden="true">&times;</span>
              </button>
            </div>
            <div class="modal-body">
              <p>Woman wearing a quarter-sleeve button-up dress seated next to a window with two embroidered pillows.</p>
            </div>
            <div class="modal-footer">
              <button type="button" class="btn btn-secondary" data-dismiss="modal">Close</button>
            </div>
          </div>
        </div>
      </div>
    </div>

    <div class="col-md-3">
      <div class="card">
        <img src="https://s3.amazonaws.com/pastperfectonline/images/museum_196/008/p2011066.jpg" class="card-img-top" alt="Cecil Reed">
        <div class="card-body">
          <h5 class="card-title">Cecil Reed</h5>
          <button type="button" class="btn btn-secondary" data-toggle="modal" data-target="#modalCecil">
            Explore
          </button>
        </div>
      </div>

      <!-- Modal for Cecil Reed -->
      <div class="modal fade" id="modalCecil" tabindex="-1" role="dialog" aria-labelledby="modalCecilLabel" aria-hidden="true">
        <div class="modal-dialog" role="document">
          <div class="modal-content">
            <div class="modal-header">
              <h5 class="modal-title" id="modalCecilLabel">Cecil Reed</h5>
              <button type="button" class="close" data-dismiss="modal" aria-label="Close">
                <span aria-hidden="true">&times;</span>
              </button>
            </div>
            <div class="modal-body">
              <p>Black and white photograph of Cecil Reed, a prominent African American politician and businessman in Iowa.</p>
            </div>
            <div class="modal-footer">
              <button type="button" class="btn btn-secondary" data-dismiss="modal">Close</button>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</div>
