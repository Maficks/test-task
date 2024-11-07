<script setup lang="ts">
fetch("E:\\Projects\\nuxt-test-task\\nuxt-app\\tree\\task_json.txt").then(
  function (response) {
    return response.text().then(function (text) {
      let el = document.getElementById("content");
      el.innerHTML = text;
    });
  },
);
</script>

<template>
  <main>
    <slot />
  </main>
  <div id="content">gg</div>
</template>

<style scoped></style>
