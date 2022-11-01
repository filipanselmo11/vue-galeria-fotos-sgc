<template>
  <div class="text-center">
    <h1 class="tx-xl-h4">Galeria de Fotos SGC</h1>
    <br />
    <br />
    <br />
    <v-row class="mb-6">
      <v-col v-for="item in arrayData" :key="item.index">
        <card-foto
            :index="item.index"
            :caminhoImagem="item.imagem"
            :tituloImagem="item.tituloImagem"
            :textoImagem="item.textoImagem"></card-foto>
      </v-col>
    </v-row>
  </div>
</template>

<script>
import CardFoto from "./CardFoto.vue";
export default {
  components: { CardFoto },
  data: () => ({
    arrayData: [
      {
        index: 1,
        imagem:
          "https://www.wallpaperflare.com/digital-art-men-city-futuristic-night-neon-science-fiction-wallpaper-udroj",
        tituloImagem: "Imagem 1",
        textoImagem: "asdasdasdasdhjgasdjh asjhdsag hagsd",
      },
      { index: 2 },
      { index: 3 },
      { index: 4 },
      { index: 5 },
      { index: 6 },
      { index: 7 },
      { index: 8 },
      { index: 9 },
      { index: 10 },
      { index: 11 },
      { index: 12 },
    ],
  }),
};
</script>

<style>
</style>