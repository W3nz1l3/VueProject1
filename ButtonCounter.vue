<script setup>
  import { ref } from 'vue'
  
  let count = ref(0)
  defineProps({
    Title: String
  })
  </script>
  
  <template>
    <button @click="count++">{{Title}}</button>{{ count }}
  </template>