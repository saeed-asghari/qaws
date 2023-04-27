
<template>
   <div class="home mx-1">
      <div class="container">
         <img class="container__image" src="@/assets/cargo-ship.jpg">
         <div class="container__text">
            <h2>Maritime transport</h2>
            <p>
            Maritime transport (or ocean transport) or more generally waterborne transport, is the transport of people
            (passengers) or goods (cargo) via waterways. Freight transport by sea has been widely used throughout
            recorded history. The advent of aviation has diminished the importance of sea travel for passengers, though
            it is still popular for short trips and pleasure cruises. Transport by water is cheaper than transport by
            air,[1] despite fluctuating exchange rates and a fee placed on top of freighting charges for carrier
            companies known as the currency adjustment factor. Maritime transport accounts for roughly 80% of
            international trade, according to UNCTAD in 2020.

            Maritime transport can be realized over any distance by boat, ship, sailboat or barge, over oceans and
            lakes, through canals or along rivers. Shipping may be for commerce, recreation, or military purposes. While
            extensive inland shipping is less critical today, the major waterways of the world including many canals are
            still very important and are integral parts of worldwide economies. Particularly, especially any material
            can be moved by water; however, water transport becomes impractical when material delivery is time-critical
            such as various types of perishable produce. Still, water transport is highly cost effective with regular
            schedulable cargoes, such as trans-oceanic shipping of consumer products – and especially for heavy loads or
            bulk cargos, such as coal, coke, ores, or grains. Arguably, the industrial revolution took place best where
            cheap water transport by canal, navigations, or shipping by all types of watercraft on natural waterways
            supported cost-effective bulk transport.

            Containerization revolutionized maritime transport starting in the 1970s. "General cargo" includes goods
            packaged in boxes, cases, pallets, and barrels. When a cargo is carried in more than one mode, it is
         </p>
         </div>
      </div>

   </div>


</template>
<style lang="scss" scoped>
.container {
   // border: 3px solid blue;
   padding: 20px 40px 40px;

   // max-width: 640px;
   &__image {
      display: inline-block;
      vertical-align: top;
      width: 46%;
      margin: 20px 30px 0 0;
   }

   &__text {
      display: inline-block;
      width: 46%;
      overflow-y: auto;
      @media (max-width: 620px) {
         width: 100%;
      }
   }
}
</style>