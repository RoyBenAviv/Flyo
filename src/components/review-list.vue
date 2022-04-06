<template>
  <section class="review-list">
    <ul>
      <li v-for="profile in profiles" :key="profile.src">
        <p class="text">Fylo has improved our team productivity by an order of magnitude. Since making the switch our team has become a well-oiled collaboration machine.</p>
        <div class="profile">
          <img :src="profile.src" />
          <div class="name">
            <p>{{ profile.name }}</p>
            <span>Founder & CEO, Huddle</span>
          </div>
        </div>
      </li>
    </ul>
  </section>
</template>

<script>
export default {
  name: 'reviews',
  data() {
    return {
      profiles: [
        {
          name: 'Satish Patel',
          src: 'assets/images/profile-1.jpg',
        },
        {
          name: 'Bruce McKenzie',
          src: '/src/assets/images/profile-2.jpg',
        },
        {
          name: 'Iva Boyd',
          src: '/src/assets/images/profile-3.jpg',
        },
      ],
    }
  },
  methods: {},
  computed: {},
  components: {},
}
</script>

<style></style>
