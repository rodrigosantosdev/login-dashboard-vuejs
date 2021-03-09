<template>
  <div class="content__form">
      <p><strong>Login</strong> to your account to browser through projects and explore our tools</p>
      <form>
        <label for="username"><input type="name" placeholder="username"></label>
        <label for="mail"><input type="email" placeholder="email@email.com"></label>
        <label for="password"><input type="epassword" placeholder="password"></label>
      </form>
      <button class="btn-sign-up" type="submit">Cadastrar</button>
      <small>Have Account? <strong><a href="/login">Login</a></strong></small>
   </div>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>

.content__form {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
   
   p {
      width: 300px;
      margin-bottom: 42px;
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
    }
}

.btn-sign-up {
   width: 300px;
   height: 48px;
   border: none;
   background-color: var(--primary);
   margin-top: 42px;
   margin-bottom: 42px;
}
</style>