<template>
    <div>
        <Comment
         v-for='comment of comments'
         v-bind:comment="comment"
         :key='comment.id'
         v-on:remove-comment="removeComment"
        />
    </div>
</template>

<script>
import Comment from './Comment.vue'
export default {
    props: {
        comments: {
            required: true
        }
    },
    methods: {
        removeComment(id) {
            this.$emit('remove-comment', id)
        }
    },
    components: {
        Comment
    }
}
</script>