<template>
  <li>
    <h2>{{ resource.title }}</h2>
    <p>{{ resource.description }}</p>
    <a :href="resource.link">Go to resource</a>
  </li>
</template>

<script>
export default {
  props: ['resource'],
}
</script>