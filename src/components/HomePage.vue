<template>
  <div class="text-center">
    <h1 class="tx-xl-h4">Galeria de Fotos SGC</h1>
    <br />
    <br />
    <br />
    <v-row class="mb-6">
      <v-col v-for="item in data1" :key="item.index">
        <card-foto
          :index="item.index"
          :caminhoImagem="item.imagem"
          :tituloImagem="item.tituloImagem"
          :textoImagem="item.textoImagem"
        ></card-foto>
      </v-col>
    </v-row>
    <v-row class="mb-6">
      <v-col v-for="item in data2" :key="item.index">
        <card-foto
          :index="item.index"
          :caminhoImagem="item.imagem"
          :tituloImagem="item.tituloImagem"
          :textoImagem="item.textoImagem"
        ></card-foto>
      </v-col>
      <v-row class="mt-6">
        <v-col v-for="item in data3" :key="item.index">
          <card-foto
            :index="item.index"
            :caminhoImagem="item.imagem"
            :tituloImagem="item.tituloImagem"
            :textoImagem="item.textoImagem"
          ></card-foto>
        </v-col>
      </v-row>
    </v-row>
  </div>
</template>

<script>
import CardFoto from "./CardFoto.vue";
export default {
  components: { CardFoto },
  data: () => ({
    data1: [
      {
        index: 1,
        imagem: require("../assets/images/sgc-foto-1.jpg"),
        tituloImagem: "Imagem 1",
        textoImagem: "Foto 1 - Ilha da Juíza e atrás a Bela Adormecida",
      },
      {
        index: 2,
        imagem: require("../assets/images/sgc-foto-2.jpg"),
        tituloImagem: "Imagem 2",
        textoImagem: "Foto 2 - Vista paronâmica da cidade",
      },
      {
        index: 3,
        imagem: require("../assets/images/sgc-foto-3.jpg"),
        tituloImagem: "Imagem 3",
        textoImagem: "Foto 3 - Vista do ginásio do Colégio São Gabriel",
      },
      {
        index: 4,
        imagem: require("../assets/images/sgc-foto-4.jpg"),
        tituloImagem: "Imagem 4",
        textoImagem: "Foto 4 - Vista da Bela Adormecida, pela praia da cidade.",
      },
    ],
    data2: [
      {
        index: 5,
        imagem: require("../assets/images/sgc-foto-5.jpg"),
        tituloImagem: "Imagem 5",
        textoImagem:
          "Foto 5 - Vista do por do sol na Serra do Cabari no fim de tarde",
      },
      {
        index: 6,
        imagem: require("../assets/images/sgc-foto-6.png"),
        tituloImagem: "Imagem 6",
        textoImagem:
          "Foto 6 - Vista da Bela Adormecida coberta por um neblina no fim de tarde",
      },
      {
        index: 7,
        imagem: require("../assets/images/sgc-foto-7.jpg"),
        tituloImagem: "Imagem 7",
        textoImagem: "Foto 7 - São Gabriel da Cahoeira por outro ângulo",
      },
      {
        index: 8,
        imagem: require("../assets/images/sgc-foto-8.jpg"),
        tituloImagem: "Imagem 8",
        textoImagem: "Foto 8 - Vista das ilhas próximas a cidade, quando se chega de avião na cidade",
      },
    ],
    data3: [
      {
        index: 9,
        imagem: require("../assets/images/sgc-foto-9.jpg"),
        tituloImagem: "Imagem 9",
        textoImagem: "Foto 9 - Outro ângulo da cidade"
      },
      {
        index: 10,
        imagem: require("../assets/images/sgc-foto-10.jpg"),
        tituloImagem: "Imagem 10",
        textoImagem: "Foto 10 - Vista da Serra do Cabari por outro ângulo, onde é possível ver também a Igreja Matriz da cidade"
      },
      {
        index: 11,
        imagem: require("../assets/images/sgc-foto-11.jpg"),
        tituloImagem: "Imagem 11",
        textoImagem:"Foto 11 - Mais outro ângulo da cidade"
      },
      {
        index: 12,
        imagem: require("../assets/images/sgc-foto-12.png"),
        tituloImagem: "Imagem 12",
        textoImagem:"Foto 12 - Vista da Bela Adormecida por completo"
      },
    ],
  }),
};
</script>

<style>
</style>