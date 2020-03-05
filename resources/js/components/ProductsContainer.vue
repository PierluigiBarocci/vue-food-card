<template>
  <div class="container d-flex flex-wrap justify-content-between">
      <single-item v-for="(item, index) in items" :key="index" :item="item"></single-item>
  </div>
</template>

<script>
import SingleItem from "./SingleItem";

export default {
  components: {
    SingleItem
  },
  data() {
    return {
      items: [
          {name:"Tiramisù", category:"Dessert", img:"https://upload.wikimedia.org/wikipedia/commons/f/fc/Tiramisu_with_blueberries_and_raspberries%2C_July_2011.jpg", description:"Lorem ipsum dolor sit amet consectetur adipisicing elit."},
          {name:"Crostata alla Marmellata", category:"Dessert", img:"https://www.cameo.it/Recipe/Recipes/cameo.it/it-it/baking/image-thumb__39758__RecipeDetail/crostata-di-marmellata.jpg", description:"Lorem ipsum dolor sit amet consectetur adipisicing elit."},
          {name:"Saint Honorè", category:"Dessert", img:"https://blobgallo.blob.core.windows.net/testi-ricette/torta-saint-honore/copertine/torta-saint-honore-landscape", description:"Lorem ipsum dolor sit amet consectetur adipisicing elit."},
          {name:"Gelato artigianale", category:"Dessert", img:"https://www.ilgelatoartigianale.info/imgpub/1900160/1000/0/come-si-fa-il-gelato.jpg", description:"Lorem ipsum dolor sit amet consectetur adipisicing elit."},
          {name:"Granita", category:"Dessert", img:"https://flockler.com/thumbs/sites/192/river-cafe-classic-italian-2_s640x0_c1997x1166_l0x462_q70_noupscale.jpg", description:"Lorem ipsum dolor sit amet consectetur adipisicing elit."},
          {name:"Arrosto di Maiale", category:"Secondo Piatto", img:"https://i0.wp.com/www.piccolericette.net/piccolericette/wp-content/uploads/2018/10/3746_Arrosto.jpg?resize=895%2C616&ssl=1", description:"Lorem ipsum dolor sit amet consectetur adipisicing elit."},
          {name:"Lasagne", category:"Primo Piatto", img:"https://realfood.tesco.com/media/images/LASAGNE-2-CLEAN-1400x919-mini-84433cf0-e601-4352-be89-de12013e52d0-0-1400x919.jpg", description:"Lorem ipsum dolor sit amet consectetur adipisicing elit."},
          {name:"Spaghetti alla Carbonara", category:"Primo Piatto", img:"https://www.donnamoderna.com/wp-content/uploads/2003/06/Spaghetti-alla-carbonara-725x545.jpg", description:"Lorem ipsum dolor sit amet consectetur adipisicing elit."},
          {name:"Insalata Mista", category:"Contorno", img:"https://www.vegolosi.it/wp-content/uploads/2018/06/insalata-dressing-burro-arachidi_1490_650.jpg", description:"Lorem ipsum dolor sit amet consectetur adipisicing elit."},
          {name:"Verdicchio", category:"Vino", img:"https://encrypted-tbn0.gstatic.com/images?q=tbn%3AANd9GcSlyT7SkVbLSTpqdImePBiW-MIv_dR69SIfGoF7dualQ_FpPMe_", description:"Lorem ipsum dolor sit amet consectetur adipisicing elit."},
      ]
    };
  }  
};
</script>