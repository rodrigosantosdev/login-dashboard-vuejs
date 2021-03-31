<template>
  <div class="content__description">
      <h1>Welcome to Splash.</h1>
      <h3>The Inkling client project admin board</h3>
      <div class="social-icons">
        <li><a href="#"><i class='bx bxl-facebook'></i></a></li>
        <li><a href="#"><i class='bx bxl-twitter'></i></a></li>
        <li><a href="#"><i class='bx bxl-instagram'></i></a></li>
        <li><a href="#"><i class='bx bxl-linkedin'></i></a></li>        
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
  padding-left: 5.3rem;
  margin-top: 250px;
  transition: .6s ease-in;

  li {
    display: inline;
  }

  a {
    color: var(--secondary);
    font-size: 1.2rem;
  }

  i {
    padding-right: 10px;

    &:hover {
      color: var(--primary);
    }
  }
}

@media ( max-width: 1260px ) {
    .content__description {
      width: 680px;
      height: 176px;
      display: flex;
      flex-direction: column;
      justify-content: space-around;
      margin: 0;

      h1, h3 {
        text-align: center;
        padding: 0;
      }

      h3 {
        width: auto;
        line-height: 0;
      }
    }

    .social-icons {
        margin-top: 0;
        text-align: center;
        padding: 0;
    }
}

@media ( max-width: 700px ) {
  .content__description {
    width: 380px;

    h1 {
      font-size: 1.4rem;
    }

    h3 {
      font-size: 1rem;
    }
  }
}
</style>