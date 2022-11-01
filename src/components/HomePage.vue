<template>
  <div class="text-center">
    <h1 class="tx-xl-h4">Galeria de Fotos SGC</h1>
    <br/>
    <br/>
    <br/>
    <v-row class="mb-6" no-gutters>
        <v-col  v-for="n in 4" :key="n">
            <card-foto
                :index="n"></card-foto>
        </v-col>
    </v-row>
  </div>
</template>

<script>
import CardFoto from './CardFoto.vue'
export default {
  components: { CardFoto },

}
</script>

<style>

</style>