<script>
export default {
  props: {
    title: {
      type: String,
      default: 'Maple'
    },
    cost: {
      type: Number,
      default: 1000
    },
    description: {
      type: String,
      default: 'Default description: Best Dog!'
    }
  },
  data() {
    return {
      count: 0
    }
  }
}
</script>

<template>
  <section :id="`${title}`" class="dog">
    <img :src="require(`../assets/${title}.jpg`)" :alt="`${title}'s picture'`" />
    <h3>{{ title[0].toUpperCase() + title.slice(1) }}</h3>
    <h6>Cost to Adopt: ${{ cost }}</h6>
    <p>{{ description }}</p>
  </section>
</template>

<style>
.dog {
  padding: 2rem;
  margin: 1.5rem auto;
  border: .1rem solid #2c3e50;
}

.dog h3 {
  margin-top: 1rem;
}

.dog img {
  max-width: 400px;
}
</style>
