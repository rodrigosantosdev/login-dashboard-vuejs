<template>

  <section class="dashboard-container">
    <SidebarMenu />
    <MainContent />  
  </section>

</template>

<script>
import SidebarMenu from '@/components/SidebarMenu.vue'
import MainContent from '@/components/MainContent.vue'

export default {
  components: { 
    SidebarMenu, 
    MainContent
    },

}
</script>

<style>
  .dashboard-container {
    width: 100%;
    height: 100%;
    display: flex;
}
</style>