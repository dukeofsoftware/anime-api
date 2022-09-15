<template>
  <div>
    <div class="grid white-300 grid-cols-3 p-3">
      <div v-for="(anime, i) in animeList" :key="i" class="m-3">
        <img
          :src="anime.url"
          alt="anime img"
          class="w-[300px] h-[300px] border-4 border-black"
        />
      </div>
    </div>
  </div>
</template>
<script>
export default {
  props: ["animeList"],
};
</script>
<style lang=""></style>
