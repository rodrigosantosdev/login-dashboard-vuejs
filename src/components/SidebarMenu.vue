<template>
   <aside class="sidebarMenu">
   <i class='bx bx-menu-alt-left' ></i>
      <nav>
         <i class='bx bx-home-alt' ></i>
         <i class='bx bxs-cart' ></i>
         <i class='bx bx-message-square-add' ></i>
         <i class='bx bxs-data'></i>
         <i class='bx bxs-user-detail' ></i>
      </nav>
      <i class='bx bx-log-out' ></i>
   </aside>
</template>

<script>
export default {

}
</script>

<style lang="scss">
   .sidebarMenu {
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: space-between;
      padding-top: 30px;
      padding-bottom: 30px;
      width: 100px;
      height: 100vh;
      background-color: var(--primary);
      font-size: 1.5rem;
   }

   nav {
      display: flex;
      flex-direction: column;
      align-items: center;

      font-size: 1.5rem;
   }

   nav i {
      padding: 20px 0;
   }
</style>