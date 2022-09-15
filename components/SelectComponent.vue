<template>
  <div class="container">
    <div class="m-5">
      <label
        for="anime"
        class="block text-center text-2xl m-3 mb-2 text-sm font-medium text-gray-900 dark:text-gray-400"
        >Gif türünü seçin</label
      >
      <select
        @change="$router.push(`/${routeParam}/${selected}`)"
        v-model="selected"
        id="anime"
        class="bg-gray-50 border border-gray-300 text-gray-900 text-sm rounded-lg focus:ring-blue-500 focus:border-blue-500 block w-full p-2.5 dark:bg-gray-700 dark:border-gray-600 dark:placeholder-gray-400 dark:text-white dark:focus:ring-blue-500 dark:focus:border-blue-500"
      >
        <option selected>tür seçin</option>
        <option v-for="(select, i) in animeList" :key="i" :value="select">
          {{ select }}
        </option>
      </select>
    </div>
  </div>
</template>
<script>
export default {
  props: ["routeParam", "animeList"],
  data() {
    return {
      selected: "",
    };
  },
};
</script>
<style lang=""></style>
