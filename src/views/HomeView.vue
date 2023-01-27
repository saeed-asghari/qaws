
<template>
   <div class="home">
      <v-row>
         <v-col col="7">
            <h3>QAWS</h3>
         </v-col>
         <v-col col="5">
            <div >
               <img class="banner" src="@/assets/banner-img-5.png" alt="banner-img" />
            </div>
         </v-col>
      </v-row>
   </div>


</template>
<style scoped>
@media (min-width: 300px) {
   .home {
      min-height: 100vh;

   }
}


@media all and (max-width: 1024px) and (min-width: 768px) {
   .banner {
      width: 600px;
   }
}
@media all and (max-width: 500px) and (min-width: 250px) {
   .banner {
      width: 200px;
   }
}
</style>