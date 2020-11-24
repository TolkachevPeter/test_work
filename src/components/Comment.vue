<template>
      <div class="media text-muted pt-3">
        <img class="mr-2 rounded" style="width: 32px; height: 32px;" src="https://dummyimage.com/32x32/007bff/007bff.png">
        <p class="media-body pb-3 mb-0 small lh-125 border-bottom border-gray">
          <strong class="d-block text-gray-dark">{{comment.author_login}}</strong> {{comment.text}}
        </p>
        <div class="dropdown">
          <button class="btn btn-secondary dropdown-toggle" type="button" id="dropdownMenuButton" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
            Actions
          </button>
          <div class="dropdown-menu" aria-labelledby="dropdownMenuButton">
            <a class="dropdown-item" href="#">Edit</a>
            <a class="dropdown-item" href="#" v-on:click="$emit('remove-comment', comment.id)">Delete</a>
          </div>
        </div>
      </div>
</template>

<script>
export default {
        props: {
        comment: {
            required: true
        }
    },
}
</script>