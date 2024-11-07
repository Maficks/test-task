<script setup lang="ts">
function ruChange() {
  setPageLayout("ru");
}
</script>

<template>
  <div>
    <form>
      <label for="language-select">Выберите язык</label>
      <select name="language" id="language-select">
        <option>Выберите язык</option>
        <option @input="ruChange">Ru</option>
        <option>En</option>
        <option>Fr</option>
      </select>
    </form>
    <button @click="ruChange">submit</button>
  </div>
</template>

<style scoped></style>
