<template>
      <div class="media text-muted pt-3">
        <img class="mr-2 rounded" style="width: 32px; height: 32px;" src="https://dummyimage.com/32x32/007bff/007bff.png">
        <p class="media-body pb-3 mb-0 small lh-125 border-bottom border-gray">
          <strong class="d-block text-gray-dark">@troodon</strong>

          <textarea class="form-control" rows="2">Education is the best provision for old age.</textarea>
          <button type="button" class="btn btn-warning">Cancel</button>
          <button type="button" class="btn btn-light"
          @submit.prevent="onSubmit"
          >Save</button>
        </p>
      </div>
</template>

<script>
export default {
    methods: {
        onSubmit() {

        }
    }
}
</script>