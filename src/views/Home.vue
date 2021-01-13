<template>
  <div class="home">
    <Header />
    <HomeOffer />
    <HomeAbout />
    <HomeInvitations />
  </div>
</template>

<script>
import Header from "@/components/Header";
import HomeOffer from "@/components/HomeOffer";
import HomeAbout from "@/components/HomeAbout";
import HomeInvitations from '../components/HomeInvitations.vue';

export default {
  name: "Home",
  components: {
    Header,
    HomeOffer,
    HomeAbout,
    HomeInvitations,
  },
  methods: {},
};
</script>
