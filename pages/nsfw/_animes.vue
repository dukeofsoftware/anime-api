<template>
  <div>
    <AnimePhotos :animeList="animes"></AnimePhotos>
  </div>
</template>
<script>
export default {
  async asyncData({ params, $axios }) {
    let animes = [];
    for (let i = 0; i < 20; i++) {
      let anime = await $axios.$get(
        `https://api.waifu.pics/nsfw/${params.animes}`
      );
      animes.push(anime);
    }
    console.log(params);
    return { animes };
  },
  layout: "animepage",
};
</script>
<style lang=""></style>
