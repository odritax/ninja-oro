<template>
 <div class="row">
   <div class="col">
     <button id ="botoncito" class="waves-effect orange btn" v-on:click="reset()">Reiniciar</button>
   </div>
 </div>
</template>
<script>
  export default {
    name:'Reset',
    methods: {
      reset: function(){
        // ev.preventDefault();
        if(window.confirm('¿Quieres reiniciar tu oro?')){
          this.$store.commit("reset");
        }
      }
    }
  }
</script>
<style>
  #botoncito{
    margin:10px;
  }
</style>

