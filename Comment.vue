<script setup>
    //This is menat to be a comment template but it seems to lean towards a comment section template
    import ButtonCounter from './ButtonCounter.vue'
    import { reactive, computed } from 'vue'
  
    const users = reactive(
        {
        name: 'John Doe',
        comments:[
                    'Vue 2 - Advanced Guide',
                    'Vue 3 - Basic Guide',
                    'Vue 4 - The Mystery'
                  ]
          }
      )
  
  //Checks if the user published any comments and shows them
  const userPublishedComments = computed(() => {return users.comments.length > 0 ? 'Yes' : 'No'})
  //After checking the userPublishedComments truthiness, display each comment and break the line between them
  </script>
  
  <template v-for = 'comment in users.comments'>
      <div class="">
        <h3>{{ users.name }}</h3>
        <span>{{ userPublishedComments }}</span>
        <ButtonCounter Title="Like"/>
        <ButtonCounter Title="Dislike"/>
      </div>   
  </template>