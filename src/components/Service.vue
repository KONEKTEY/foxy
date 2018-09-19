<template>
    <div id="services">
    <div class="container">
      <div class="section-title text-center">
            <h3>Clips</h3>
            <h2>TRAP ART INTRO</h2>
        </div>
        <CarouselLarge v-if="getScreenSize===2"/>
        <CarouselMedium v-if="getScreenSize===1"/>
        <CarouselMin v-if="getScreenSize===0"/>
    </div>
  </div>
</template>

<script>
import CarouselLarge from './Carousel/CarouselLarge';
import CarouselMedium from './Carousel/CarouselMedium';
import CarouselMin from './Carousel/CarouselMin';
export default {
    name : 'Service',
    data:()=>{
      return{
        min:false,
        medium:false,
        large:true
      }
    },
    components:{
      CarouselLarge,
      CarouselMedium,
      CarouselMin
    },
    computed:{
      getScreenSize:()=>{
        if (screen.width<680){
          return 0
        }else if(screen.width < 1024 && screen.width>680){
          return 1
        }else{
          return 2
        }
      }
    },
}
</script>

<style>

</style>
