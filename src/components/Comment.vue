<template>
      <div class="media text-muted pt-3">
        <img class="mr-2 rounded" style="width: 32px; height: 32px;" src="https://dummyimage.com/32x32/007bff/007bff.png">
        <p class="media-body pb-3 mb-0 small lh-125 border-bottom border-gray">
          <strong class="d-block text-gray-dark">{{comment.author_login}}</strong> {{comment.text}}
        </p>
          <div>
  <b-dropdown id="dropdown-1" text="Actions" class="m-md-2">
    <b-dropdown-item>Edit</b-dropdown-item>
    <b-dropdown-item v-on:click="$emit('remove-comment', comment.id)">Delete</b-dropdown-item>
  </b-dropdown>
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