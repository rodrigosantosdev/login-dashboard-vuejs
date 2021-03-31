<template>
  <div class="content__form">
      <p><strong>Login</strong> to your account to browser through projects and explore our tools</p>
      <form>
        <label for="mail"><input type="email" placeholder="email@email.com"></label>
        <label for="password"><input type="epassword" placeholder="password"></label>
      </form>
      <div class="btn-sign-in">
        <a href="/dashboard"><i class='bx bx-right-arrow-alt'></i></a>
      </div>
      <small>Don’t have on account? <strong><a href="/signup">Sign Up</a></strong></small>
   </div>
</template>

<script>
export default {

}
</script>

<style lang="scss">

.content__form {
    width: 455px;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
   
    p {
      width: 300px;
      margin-bottom: 30px;
   }
      
   strong {
      font-weight: 500;
   }

    form {
      padding-left: 4rem;
      padding-right: 4rem;
    }

    label {
      display: block;
    }

    input {
      width: 300px;
      height: 45px;
      box-shadow: 2px 3px 4px rgba(123, 123, 123, 0.25);
      border: 0;
      margin-top: 20px;
      padding-left: 20px;
    }

    small {
      color: var(--dark);

      a {
        color: var(--dark);
      }

      a:hover {
        color: var(--black);
      }
    }

    .btn-sign-in {
      width: 48px;
      height: 48px;
      display: flex;
      align-items: center;
      justify-content: center;
      border: none;
      border-radius:50%;
      background-color: var(--primary);
      margin-top: 42px;
      margin-bottom: 42px;

      &:hover {
        background:var(--dark);
        transition: all 1s ease;
      }

      i {
        font-size: 24px;
        color: var(--secondary);
      }
    }
}

@media ( max-width: 1200px ) {
  .content__form {
    margin-top: 60px;  
  }
}
</style>