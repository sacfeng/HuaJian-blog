<template>
  <div class="main-content">
      <LeftSection></LeftSection>
  </div>
</template>

<script>
import LeftSection from './LeftSection.vue'
export default {
    name:'MainContent',
    components:{
        LeftSection
    }
}
</script>

<style scoped>
    .main-content{
        margin-top:60px;
        height: 3000px;
    }
</style>