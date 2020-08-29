<template>
<div id="inizio">

      <Navigation>
      </Navigation>

    	<!-- <div v-for="(dataHomes, index) in dataHome" :key=" `__home_$(index)`">
    <home
              :name         = "dataHomes.name"
              :title        = "dataHomes.title"
              :desc         = "dataHomes.desc"
              :location     = "dataHomes.location"
              :phone        = "dataHomes.phone"
              :email        = "dataHomes.email"
    >
    </home> -->
    <!-- </div> -->
 </div>
</template>


<script>
import Navigation from '~/components/Navigation.vue'

export default {
    head: {
    bodyAttrs: {
      class: ' antialiased leading-normal tracking-wider steback'
    }
  },

  data(){
          return{

        }
    }

}
</script>

<style>
/* Sample `apply` at-rules with Tailwind CSS
.container {
@apply min-h-screen flex justify-center items-center text-center mx-auto;
}
*/
#top{
    width: calc(100vw - 18px);
    min-height: 10rem;
    height: auto;
    background-color: transparent;
    position: absolute;
    z-index: 11;
    top: 0;
    padding: 0 9rem;
    
}
#inizio{
    width: 100%;
    overflow: hidden;
}

.steback{
  background:url('~assets/bg/backHome.jpg');
  background-size: cover;
}

</style>
