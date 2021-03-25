<template>
  <section class="navbartop">
   <a href="#" class="new-order-btn">+ New Order</a>
   <div class="profile-sign-in">
    <img src="https://i.pravatar.cc/150?img=3" alt="">
    <h4>Hi John Doe</h4>
    <i class='bx bxs-down-arrow'></i>
   </div>
  </section>
</template>

<script>
export default {

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