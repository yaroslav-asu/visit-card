<template>
  <header class="header">
    <p class="tab">AOEU</p>
    <p class="tab">AOEU</p>
    <p class="tab">AOUE</p>
    <p class="tab">AOEU</p>
    <p class="tab">AOEU</p>
  </header>
</template>

<script>
export default {
  name: "HeaderComponent",
  data() {
    return {
      tab: "",
    }
  }
}
</script>

<style>
.header {
  color: white;
  display: flex;
  justify-content: space-between;
}
</style>
