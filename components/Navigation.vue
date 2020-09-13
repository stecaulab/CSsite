<template>
<div>
  <div id="top" class="flex justify-between ">
    <a href="" id="marca" class="text-white">

    </a>

  <div id="navigator" class="flex justify-end items-center">
        <nav>
          <ul class="menu">
            <!-- <li class="mr-6 efeito-menu"><nuxt-link  to="/">Home</nuxt-link></li>
            <li class="mr-6 efeito-menu" ><nuxt-link class="text-white" to="/about">About</nuxt-link></li>
            <li class="mr-6 efeito-menu" ><nuxt-link class="text-white" to="">Project</nuxt-link> </li>
            <li class="mr-6 efeito-menu" ><nuxt-link class="text-white" to="">Contatti</nuxt-link> </li> -->
            <li class="mr-6 efeito-menu" v-for="(Item , i) in menuItem" :key="i"><nuxt-link :class="[currentPage === (`${Item.address}`) ? activeClass: '']" :to="`/${Item.address}`">{{ Item.page}}</nuxt-link></li>
          </ul>
        </nav>
    </div>
  </div>
</div>
</template>
<script>

export default {
  name: 'Navigation',

  data(){


      return{
            menuItem:[
                      {page:'Home',address:''},
                      {page:'About',address:'About'},
                      {page:'Project',address:'Project'},
                      {page:'Contacts',address:'Contacts'},
            ],

            activeClass: 'active',

    };
},
  computed:{
      currentPage(){
          return this.$route.path;
        },
    },

}
</script>
<style>

#marca{
    /* background: url(../images/marca.svg) no-repeat center; */
    background-size: 21.8rem 6.5rem;
    width: 10rem;
    height: 10rem;
    display: block;
    float: left;
    left: 0;
    position: relative;
    top: 0;


  }
#navigator{}

ul.menu{ width: 100%; height: 100%; list-style: none; position: relative;}
ul.menu > li { width:auto; height: auto; position: relative; float: left;}
ul.menu > li > a{ width: auto; font-size: 2.1rem; line-height: 1em; margin-left: 2.5rem; padding-bottom: 1.2rem; color: #fff; position: relative; font-family: 'Roboto'; text-transform: uppercase;}
ul.menu > li > a:after{ content: ''; position: absolute; width: 100%; height: 1px; background: #fff; left: 0; bottom: 0;
-webkit-transition: all 800ms cubic-bezier(0.645, 0.045, 0.355, 1.000);
   -moz-transition: all 800ms cubic-bezier(0.645, 0.045, 0.355, 1.000);
     -o-transition: all 800ms cubic-bezier(0.645, 0.045, 0.355, 1.000);
        transition: all 800ms cubic-bezier(0.645, 0.045, 0.355, 1.000); /* easeInOutCubic */

-webkit-transition-timing-function: cubic-bezier(0.645, 0.045, 0.355, 1.000);
   -moz-transition-timing-function: cubic-bezier(0.645, 0.045, 0.355, 1.000);
     -o-transition-timing-function: cubic-bezier(0.645, 0.045, 0.355, 1.000);
        transition-timing-function: cubic-bezier(0.645, 0.045, 0.355, 1.000); /* easeInOutCubic */}

ul.menu > li > a:before{
}

/* ul.menu > li > a.menu-active:after{height: 4px;} */

.efeito-menu:hover a:after {
height: 1px;
    -webkit-animation: efeitoMenuAfter 0.25s ease forwards;
    animation: efeitoMenuAfter 0.25s ease forwards;

    -webkit-transition: all 800ms cubic-bezier(0.645, 0.045, 0.355, 1.000);
   -moz-transition: all 800ms cubic-bezier(0.645, 0.045, 0.355, 1.000);
     -o-transition: all 800ms cubic-bezier(0.645, 0.045, 0.355, 1.000);
        transition: all 800ms cubic-bezier(0.645, 0.045, 0.355, 1.000); /* easeInOutCubic */

-webkit-transition-timing-function: cubic-bezier(0.645, 0.045, 0.355, 1.000);
   -moz-transition-timing-function: cubic-bezier(0.645, 0.045, 0.355, 1.000);
     -o-transition-timing-function: cubic-bezier(0.645, 0.045, 0.355, 1.000);
        transition-timing-function: cubic-bezier(0.645, 0.045, 0.355, 1.000); /* easeInOutCubic */
}


@keyframes efeitoMenuAfter {
    0% { height: 1px;  }
    100% {height: 4px; }
}

/*
.efeito-menu:hover a:before {
height: 0;
    -webkit-animation: efeitoMenu 0.45s  forwards;
-webkit-transition: all 800ms cubic-bezier(0.645, 0.045, 0.355, 1.000);
   -moz-transition: all 800ms cubic-bezier(0.645, 0.045, 0.355, 1.000);
     -o-transition: all 800ms cubic-bezier(0.645, 0.045, 0.355, 1.000);
        transition: all 800ms cubic-bezier(0.645, 0.045, 0.355, 1.000);

-webkit-transition-timing-function: cubic-bezier(0.645, 0.045, 0.355, 1.000);
   -moz-transition-timing-function: cubic-bezier(0.645, 0.045, 0.355, 1.000);
     -o-transition-timing-function: cubic-bezier(0.645, 0.045, 0.355, 1.000);
        transition-timing-function: cubic-bezier(0.645, 0.045, 0.355, 1.000);
}
*/

ul.menu > li > a.active:after {
    height: 4px;
    background: #f1742c;
}

</style>



