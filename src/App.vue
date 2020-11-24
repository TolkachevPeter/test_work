<template>
  <div id="app">
    <div class="my-3 p-3 bg-white rounded shadow-sm">
       <AddComment
       @add-comment="addComment"
       />
      <h6 class="border-bottom border-gray pb-2 mb-0">Recent comments</h6>
      <EditComment />

  <CommentList 
  v-bind:comments="comments"
  @remove-comment='removeComment'
  />

    </div>
  </div>
</template>

<script src="./App.js"></script>
<script>
import CommentList from './components/CommentList.vue'
import AddComment from './components/AddComment.vue'
import EditComment from './components/EditComment.vue'
export default {
  data() {
    return {
        comments: [
      {
        author_login: 'troodon!',
        author_avatar: 'https://dummyimage.com/32x32/007bff/007bff.png',
        text: 'example of cool comment',
      }
    ]
    }
  },
      methods: {
        removeComment(id) {
            this.comments = this.comments.filter(item => item.id !== id )
        },
        addComment(comment) {
          this.comments.push(comment)
        }
    },
  components: {
    CommentList,
    AddComment,
    EditComment
  }
}
</script>
