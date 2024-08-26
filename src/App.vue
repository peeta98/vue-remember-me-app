<template>
  <ul>
    <list-item 
      v-for="resource in storedResources" 
      :key="resource.id" 
      :resource="resource"
    ></list-item>
  </ul>
</template>

<script>
import ListItem from './components/ListItem.vue';

export default {
  components: {
    ListItem
  },
  data() {
    return {
      storedResources: [
        {
          id: 'offical-guide',
          title: 'Official Guide',
          description: 'The official Vue.js documentation.',
          link: 'https://vuejs.org'
        },
        {
          id: 'google',
          title: 'Google',
          description: 'Learn to google...',
          link: 'https://google.org'
        }
      ]
    }
  }
}
</script>