<template>
  <section class="navbartop">
   <a href="#" class="new-order-btn">+ New Order</a>
   <Profile />
  </section>
</template>

<script>
import Profile from './Profile.vue'
export default {
  components: {Profile}
}
</script>

<style>
  .navbartop {
    width: 100%;
    height: 80px;

    display: flex;
    align-items: center;
    justify-content: space-between;
    
    padding: 0 30px;
    background-color: var(--dark);
  }

  .new-order-btn {
    color: var(--primary);
    font-size: 24px;
  }
</style>