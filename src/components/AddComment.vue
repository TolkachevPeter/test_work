<template>
    <div>
      <form v-on:submit.prevent="onSubmit" type="button">
        <div class="form-group">
          <label for="exampleFormControlTextarea1">Your comment:</label>
          <textarea class="form-control"  rows="3" v-model="text"></textarea>
          <button class="btn">Send comment</button>
        </div>
      </form>
    </div>
</template>

<script>
export default {
    data() {
        return {
            text: "",
        }
    },
    methods: {
        onSubmit() {
            if(this.text.trim()) {
                const newComment ={
                    id: Date.now(),
                    text: this.text,
                }

            this.$emit('add-comment', newComment)
            }
        }
    }
}
</script>