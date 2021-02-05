<template>
  <header class="main-header">
      花间博客
  </header>
</template>

<script>
export default {
    name:'MainHeader'
}
</script>

<style scoped>
    .main-header{
        position: fixed;
        z-index: 10;
        top:0;
        margin: 0;
        width: 100%;
        height: 60px;
        /* border-bottom: 1px solid #d64a74; */
        box-shadow: 0 0 10px #d64a74;
        background:rgb(255 255 255 / 14%);
    }
</style>