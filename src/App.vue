<template>
  <div id="app">
    <div class="my-3 p-3 bg-white rounded shadow-sm">
      <form>
        <div class="form-group">
          <label for="exampleFormControlTextarea1">Your comment:</label>
          <textarea class="form-control"  rows="3"></textarea>
          <button type="button" class="btn btn-light">Send comment</button>
        </div>
      </form>

      <h6 class="border-bottom border-gray pb-2 mb-0">Recent comments</h6>

      <div class="media text-muted pt-3">
        <img class="mr-2 rounded" style="width: 32px; height: 32px;" src="https://dummyimage.com/32x32/007bff/007bff.png">
        <p class="media-body pb-3 mb-0 small lh-125 border-bottom border-gray">
          <strong class="d-block text-gray-dark">@troodon</strong>

          <textarea class="form-control" rows="2">Education is the best provision for old age.</textarea>
          <button type="button" class="btn btn-warning">Cancel</button>
          <button type="button" class="btn btn-light">Save</button>
        </p>
      </div>


      <div class="media text-muted pt-3">
        <img class="mr-2 rounded" style="width: 32px; height: 32px;" src="https://dummyimage.com/32x32/007bff/007bff.png">
        <p class="media-body pb-3 mb-0 small lh-125 border-bottom border-gray">
          <strong class="d-block text-gray-dark">@troodon</strong> Education is the best provision for old age.
        </p>
        <div class="dropdown">
          <button class="btn btn-secondary dropdown-toggle" type="button" id="dropdownMenuButton" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
            Actions
          </button>
          <div class="dropdown-menu" aria-labelledby="dropdownMenuButton">
            <a class="dropdown-item" href="#">Edit</a>
            <a class="dropdown-item" href="#">Delete</a>
          </div>
        </div>
      </div>

      <div class="media text-muted pt-3">
        <img alt="32x32" class="mr-2 rounded" src="https://dummyimage.com/32x32/e83e8d/e83e8d.png" style="width: 32px; height: 32px;">
        <p class="media-body pb-3 mb-0 small lh-125 border-bottom border-gray">
          <strong class="d-block text-gray-dark">@alxndrv88</strong> Pleasure in the job puts perfection in the work.
        </p>
        <div class="dropdown">
          <button class="btn btn-secondary dropdown-toggle" type="button" id="dropdownMenuButton" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
            Actions
          </button>
          <div class="dropdown-menu" aria-labelledby="dropdownMenuButton">
            <a class="dropdown-item" href="#">Edit</a>
            <a class="dropdown-item" href="#">Delete</a>
          </div>
        </div>
      </div>
      <div class="media text-muted pt-3">
        <img class="mr-2 rounded" src="https://dummyimage.com/32x32/6f42c1/6f42c1.png" style="width: 32px; height: 32px;">
        <p class="media-body pb-3 mb-0 small lh-125 border-bottom border-gray">
          <strong class="d-block text-gray-dark">@vrubel</strong> Quality is not an act, it is a habit.
        </p>
        <div class="dropdown">
          <button class="btn btn-secondary dropdown-toggle" type="button" id="dropdownMenuButton" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
            Actions
          </button>
          <div class="dropdown-menu" aria-labelledby="dropdownMenuButton">
            <a class="dropdown-item" href="#">Edit</a>
            <a class="dropdown-item" href="#">Delete</a>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script src="./App.js"></script>
