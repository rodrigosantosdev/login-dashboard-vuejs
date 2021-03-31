<template>
  <div class="main-content">
    <Navbartop />
    <NewOrder />
  </div>
</template>

<script>
import Navbartop from './Navbartop.vue'
import NewOrder from './NewOrder.vue'

export default {
  components: { Navbartop, NewOrder },
}

</script>

<style>
 .main-content {
   width: 100%;
   background-color:var(--secondary);
  }
</style>