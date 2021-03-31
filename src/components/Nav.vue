<template>
   <div class="content__nav">
      <div class="content__logo">
        <img src="@/assets/logo.svg" alt="logo">
      </div>
      <div class="content__nav--item">
        <router-link to="/">
          <li><i class='bx bx-user-check'></i>Login</li>
        </router-link>        
        <router-link to="/signup">
          <li><i class='bx bx-user-plus'></i>SignUp</li>     
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

  .content__logo {
    width: 75px;
    height: 75px;
  }
  
  .content__nav--item {
    display: flex;
    flex-direction: column;
    align-items: center;
    width: 100%;

    li {
      text-align: center;
      padding: 0 30px;      
    }

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

  @media ( max-width: 1260px ) {
    .content__nav {
      width: 100%;
      height: 100px;
      display: flex;
      flex-direction: row;
      padding: 0 50px;
    }

    .content__nav--item {
      display: flex;
      flex-direction: row;
      justify-content: flex-end;
    }

    .content__logo {
      padding: 0;
      margin: 0;
    }
  }

  @media ( max-width: 700px) {
    .content__nav {
      padding: 0 10px;
    }

    .content__nav--item {
      display: flex;
      flex-direction: row;
      justify-content: flex-end;
    }
  }
  
</style>