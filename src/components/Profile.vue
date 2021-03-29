<template>
  <div class="profile-sign-in">
    <img src="https://picsum.photos/200" alt="">
    <h4>Hi, John Doe</h4>
    <i class='bx bxs-down-arrow'></i>
   </div>
</template>

<style lang="scss">

.profile-sign-in {
   display: flex;
   align-items:center;
   border-left: 2px solid var(--border);
   padding-left: 25px;
   height:80px;

   img {
   width: 35px;
   height: 35px;
   border-radius: 50%;
   margin-right: 10px;
   }

   h4 {
      color: var(--white);
      font-weight: normal;
   }

   i {
      color: var(--gray-light);
      margin-left: 10px;
   }
}

</style>