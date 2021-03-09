<template>
  <div class="content__description">
      <h1>Welcome to Splash.</h1>
      <h3>The Inkling client project admin board</h3>
      <div class="social-icons">
        <i class='bx bxl-facebook'></i>
        <i class='bx bxl-twitter'></i>
        <i class='bx bxl-instagram'></i>
        <i class='bx bxl-linkedin'></i>
      </div>
    </div>
</template>

<script>
export default {

}
</script>

<style lang="scss">
   .content__description {
    width: 600px;
    height: 725px;

    display: flex;
    flex-direction: column;
    justify-content: center;
    margin-top: -6%;
    background-color: var(--dark);
       
      h1 {
        color: var(--secondary);
        font-size: 2rem;
        padding-left: 5.3rem;
        padding-bottom: 2rem;
      }

      h3 {
        width: 300px;
        font-size: 1.3rem;
        font-weight: 400;
        text-align: left;
        color: var(--secondary);
        line-height: 25px;
        padding-left: 5.3rem;
      }
  }

  
.social-icons {
  color: var(--secondary);
  padding-left: 5.3rem;
  margin-top: 250px;
  transition: .6s ease-in;

  i {
    padding-right: 10px;

    &:hover {
      color: var(--primary);
    }
  }
}
</style>