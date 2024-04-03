<script setup>
    import { reactive, computed } from 'vue'
    import users from './Comment.vue'
    
    //Checks if the user published any comments and shows them
    const publishedComments = computed(() => {return users.comments.length > 0 ? 'Yes' : 'No'})
    //using the template, find a way to iterate through all the comments related to a post.
</script>

<style>
</style>

<template>
    <Comment/>
</template>