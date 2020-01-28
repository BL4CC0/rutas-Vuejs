<template>
  <div class="pb-5">
    <h1>Estos son los servicios :</h1>

      <router-link :to="{ name: 'services', params:{ id: items} }" 
        
        v-for="(items , index) of servicios" :key="index" >

            <button class="btn btn-outline-success px-5 mx-2">{{items}}</button>

        </router-link>

    <Servicio class="my-5"/>

        <button class="btn btn-primary px-5 mx-2" @click="anterior">Anterior</button>
        <button class="btn btn-info px-5 mx-2" @click="home">Home</button>
        <button class="btn btn-primary px-5 mx-2" @click="siguiente">Siguiente</button>
  </div>

</template>

<script>

  import Servicio from '@/components/Servicio.vue'

export default {
  name: "Servicios",
  components:{
    Servicio
  },
   data() {
        return {
            servicios :[1,2,3]
        }
    },methods: {
      home(){
        this.$router.push("/")
      },
      anterior(){
        this.$router.go(-1)
      },
      siguiente(){
        this.$router.go(1)
      }
    }
}
</script>