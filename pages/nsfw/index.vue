<template>
  <div>
    <SelectComponent routeParam="nsfw" :animeList="selects"></SelectComponent>
  </div>
</template>
<script>
export default {
  data() {
    return {
      selects: ["waifu", "neko", "trap", "blowjob"],
    };
  },
};
</script>
<style lang=""></style>
