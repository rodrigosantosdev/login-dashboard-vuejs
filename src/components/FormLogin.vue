<template>
  <div class="content__form">
      <p><strong>Login</strong> to your account to browser through projects and explore our tools</p>
      <form>
        <label for="mail"><input type="email" placeholder="email@email.com"></label>
        <label for="password"><input type="epassword" placeholder="password"></label>
      </form>
      <a href="/dashboard" type="submit"><i class='bx bx-right-arrow-alt'></i></a>
      <small>Don’t have on account? <strong><a href="/signup">Sign Up</a></strong></small>
   </div>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
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

    a {
      width: 48px;
      height: 48px;

      border: none;
      border-radius:50%;
      background-color: var(--primary);

      margin-top: 42px;
      margin-bottom: 42px;

      i {
        font-size: 24px;
        color: var(--secondary);
      }
    }

    small {
      color: var(--dark);

      a {
        color: var(--dark);
      }
    }
}
</style>