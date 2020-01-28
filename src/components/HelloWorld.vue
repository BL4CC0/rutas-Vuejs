<template>
  <div class="hello container">

      <div class="row">
        <div class="col-6 offset-3">
            <div class="card-body text-vue">
                <h3>Bienvenido a la prueba de Rutas</h3>
            </div>
        </div>
      </div>
   
  </div>
</template>

<script>

export default {
  name: 'HelloWorld',
  props: {
    msg: String
  }
}

</script>

<style >
  
    .text-vue{
      color: #42b983; 
    }

</style>