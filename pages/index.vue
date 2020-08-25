<template>
<div>
    	<div v-for="(dataHomes, index) in dataHome" :key=" `__home_$(index)`">
    <home
              :name         = "dataHomes.name"
              :title        = "dataHomes.title"
              :desc         = "dataHomes.desc"
              :location     = "dataHomes.location"
              :phone        = "dataHomes.phone"
              :email        = "dataHomes.email"
    >
    </home>
    </div>
</div>
</template>


<script>
import Home from '~/components/Home.vue'

export default {
    head: {
    bodyAttrs: {
      class: ' antialiased leading-normal tracking-wider bg-cover text-gray-90 steback'
    }
  },
    components:{
      Home
  },
  data(){
          return{
              dataHome: [
                    { name:'Cauzzi Stefano', desc:'Impiegato Tecnico Meccanico, con la passione per la programmazione.', title : ' CNC Machine Tool Programmer', location:'Solferino (MN) 46040',phone:'+39343584908',email:'cauzzistefano@gmail.com'},

                  ]

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
.container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.title {
  font-family:
    'Quicksand',
    'Source Sans Pro',
    -apple-system,
    BlinkMacSystemFont,
    'Segoe UI',
    Roboto,
    'Helvetica Neue',
    Arial,
    sans-serif;
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: #35495e;
  letter-spacing: 1px;
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}

.links {
  padding-top: 15px;
}
.steback{
  background-image:url('~assets/bg/backHome.jpg');
}

</style>
