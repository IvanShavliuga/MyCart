<template>
  <div class="main">
  	   <app-header></app-header>
  	   <div>
             	<router-view></router-view>   	
  	   </div>
       
  </div>
</template>

<script>
  import Header from './components/Header.vue';
  export default {
  	     components: {
  	         appHeader: Header	
  	     },

         created() {
          this.$store.dispatch('initProducts');
         }
          
     }

</script>

<style lang="scss">
@import './assets/styles/vars.scss';
body {
  background-color: $bodybackground;
  padding: 0;
  
}
.main{
  margin: 0;
  padding: 0;
  width: 100%;
}
</style>
