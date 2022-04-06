<template>
  <section class="info-preview">
    <img :src="info.src" />
    <h3>{{ info.title }}</h3>
    <p>{{ info.text }}</p>
  </section>
</template>

<script>
export default {
  props: {
    info: Object,
  },
  name: 'preview',
  data() {
    return {}
  },
}
</script>

<style></style>
