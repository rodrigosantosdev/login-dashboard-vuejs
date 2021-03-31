<template>
   <nav class="sidebarMenu">
      <div class="navBurguer">
         <button type="button" @click="handdleToggle" aria-label="button navigation"><i aria-hidden="true" class='bx bx-menu-alt-left'></i></button>
      </div> 
      <nav class="navigation">
         <li><a href=""><i class='bx bx-home-alt'></i></a></li>
         <li><a href=""><i class='bx bxs-cart'></i></a></li>
         <li><a href=""><i class='bx bx-message-square-add'></i></a></li>
         <li><a href=""><i class='bx bxs-data'></i></a></li>
         <li><a href=""><i class='bx bxs-user-detail'></i></a></li>
      </nav>

      <div class="sliderNav" :class="{'isActive': openSliderNav}">
         <li><a href="#">Home</a></li>
         <li><a href="#">Cart</a></li>
         <li><a href="#">Messege</a></li>
         <li><a href="#">Data Base</a></li>
         <li><a href="#">Details</a></li>
      </div>

      <div class="button-sign-out">
         <a href="/"><i class='bx bx-log-out'></i></a>
      </div>
   </nav>
</template>

<script>

import { ref } from 'vue'

export default {
   setup() {
      let openSliderNav = ref(false) // magica

      function handdleToggle() {
         openSliderNav.value = !openSliderNav.value
      }

      return {
         openSliderNav,
         handdleToggle,
      }
   }
}

</script>

<style lang="scss">

   .sidebarMenu {
      width: 100px;
      height: 100vh;
      
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: space-between;
      padding-top: 30px;
      padding-bottom: 30px;
      background-color: var(--primary);
      font-size: 1.5rem;
   }

   .navigation {
      display: flex;
      flex-direction: column;
      align-items: center;

      font-size: 1.5rem;

      li {
         display: flex;
         justify-content: center;
         width:90px;
      }

      a {
        color: var(--dark);
      }

      i {
         padding: 20px 0;
      }

      i:hover {
         color: var(--black);
      }      
   }

   .sliderNav {
      width: 0;
      height: 100%;
      pointer-events: none;
      overflow: hidden;
      background-color: var(--primary);
      position: absolute;
      left:90px;
      top: 0;
      transition: all 0.5s ease-in-out;
      padding-top: 99px;

      li {
         min-width: 200px;
         display: flex;
         align-items: center;
         height:64px;
      }

      a {
         color: var(--dark);
         font-size: 1.2rem;
      }

      a:hover {
         color: var(--black);
      }
      
   }

   .navBurguer {
      margin-bottom: 40px;

      button {
        color: var(--dark);
        font-size: 1.6rem;
        background: transparent;
        cursor: pointer;
      }

      i:hover {
         color: var(--black);
      }
   }

   .isActive {
      width: 200px;
      pointer-events: all;
   }

   .button-sign-out {
      display: flex;
      align-items:flex-end;
      flex: 1;

      a {
        color: var(--dark);
      }

      i:hover {
         color: var(--black);
      }
   }
 
</style>