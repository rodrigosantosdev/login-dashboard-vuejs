<template>
   <div class="content__nav">
      <div class="content__logo">
        <img src="@/assets/logo.svg" alt="logo">
      </div>
      <div class="content__nav--item">
        <router-link to="/login">
          <i class='bx bx-user-check'></i>
          Login
        </router-link>
        
        <router-link to="/signup">
          <i class='bx bx-user-plus'></i>
          SignUp
        </router-link>
      </div>
    </div>
</template>

<script>
export default {

}
</script>

<style lang="scss">
   .content__nav {
    width: 175px;
    height: 100%;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: space-around;
  }
  
  .content__nav--item {
    display: flex;
    flex-direction: column;
    align-items: center;

    a {
      text-transform: uppercase;
      color: var(--dark);
      font-size: 0.875rem;
      padding: 2rem 0;
    }

    i {
      display: block;
      text-align: center;
      font-size: 2rem;
    }
  }

  .content__logo {
    width: 75px;
    height: 75px;
  }
</style>