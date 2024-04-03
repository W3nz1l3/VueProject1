<script setup>
  import ButtonCounter from './ButtonCounter.vue'
  import BlueSquare from './BlueSquare.vue'
  import Comment from './Comment.vue'
</script>

<style>
  .comment-border{
    border: 1px grey solid
  }
</style>

<template>
  <!--This is where the user views the content and comments, likes or dislikes the content-->
  <div >
    <BlueSquare/>
    <ButtonCounter Title="Like" />
    <ButtonCounter Title="Dislike" />
    <button>Comment</button>
    <Comment/>
  </div>
</template>