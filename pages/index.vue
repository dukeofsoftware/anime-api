<template>
<div>Uygulamaya Hoşgeldiniz!</div>
</template>

<script>
import SelectComponent from "../components/SelectComponent.vue";
import AnimePhotos from "../components/AnimePhotos.vue";
import NavBar from "~/components/NavBar.vue";
export default {
  name: "IndexPage",
  data() {
    return {};
  },

  components: { SelectComponent, AnimePhotos, NavBar },
};
</script>
