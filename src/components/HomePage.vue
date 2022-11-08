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
      <v-col
        v-for="item in data2"
        :key="item.index"
      >
        <card-foto
          :index="item.index"
          :caminhoImagem="item.imagem"
          :tituloImagem="item.tituloImagem"
          :textoImagem="item.textoImagem"
        ></card-foto>
      </v-col>
      <v-row class="mt-6">
      <v-col
        v-for="item in data3"
        :key="item.index"
      >
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
        textoImagem:
          "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum tincidunt magna justo, vel molestie risus dignissim vitae. Morbi ultricies enim ut tellus suscipit, nec placerat odio dapibus. Fusce aliquam condimentum enim, et dignissim elit. Aenean auctor blandit dictum. Proin orci mauris, commodo ac tellus et, hendrerit varius lectus. In consequat pharetra interdum. Cras rutrum faucibus dignissim. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nam gravida risus at nunc tincidunt, eu porttitor metus molestie. Cras rutrum lacus dui, consectetur tincidunt metus suscipit a.",
      },
      {
        index: 2,
        imagem: require("../assets/images/sgc-foto-2.jpg"),
        tituloImagem: "Imagem 2",
        textoImagem:
          "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum tincidunt magna justo, vel molestie risus dignissim vitae. Morbi ultricies enim ut tellus suscipit, nec placerat odio dapibus. Fusce aliquam condimentum enim, et dignissim elit. Aenean auctor blandit dictum. Proin orci mauris, commodo ac tellus et, hendrerit varius lectus. In consequat pharetra interdum. Cras rutrum faucibus dignissim. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nam gravida risus at nunc tincidunt, eu porttitor metus molestie. Cras rutrum lacus dui, consectetur tincidunt metus suscipit a.",
      },
      {
        index: 3,
        imagem: require("../assets/images/sgc-foto-3.jpg"),
        tituloImagem: "Imagem 3",
        textoImagem:
          "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum tincidunt magna justo, vel molestie risus dignissim vitae. Morbi ultricies enim ut tellus suscipit, nec placerat odio dapibus. Fusce aliquam condimentum enim, et dignissim elit. Aenean auctor blandit dictum. Proin orci mauris, commodo ac tellus et, hendrerit varius lectus. In consequat pharetra interdum. Cras rutrum faucibus dignissim. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nam gravida risus at nunc tincidunt, eu porttitor metus molestie. Cras rutrum lacus dui, consectetur tincidunt metus suscipit a.",
      },
      {
        index: 4,
        imagem: require("../assets/images/sgc-foto-4.jpg"),
        tituloImagem: "Imagem 4",
        textoImagem:
          "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum tincidunt magna justo, vel molestie risus dignissim vitae. Morbi ultricies enim ut tellus suscipit, nec placerat odio dapibus. Fusce aliquam condimentum enim, et dignissim elit. Aenean auctor blandit dictum. Proin orci mauris, commodo ac tellus et, hendrerit varius lectus. In consequat pharetra interdum. Cras rutrum faucibus dignissim. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nam gravida risus at nunc tincidunt, eu porttitor metus molestie. Cras rutrum lacus dui, consectetur tincidunt metus suscipit a.",
      },
    ],
    data2: [
      {
        index: 5,
        imagem: require("../assets/images/sgc-foto-4.jpg"),
        tituloImagem: "Imagem 5",
         textoImagem:
          "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum tincidunt magna justo, vel molestie risus dignissim vitae. Morbi ultricies enim ut tellus suscipit, nec placerat odio dapibus. Fusce aliquam condimentum enim, et dignissim elit. Aenean auctor blandit dictum. Proin orci mauris, commodo ac tellus et, hendrerit varius lectus. In consequat pharetra interdum. Cras rutrum faucibus dignissim. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nam gravida risus at nunc tincidunt, eu porttitor metus molestie. Cras rutrum lacus dui, consectetur tincidunt metus suscipit a.",
      },
      {
        index: 6,
        imagem: require("../assets/images/sgc-foto-4.jpg"),
        tituloImagem: "Imagem 7",
         textoImagem:
          "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum tincidunt magna justo, vel molestie risus dignissim vitae. Morbi ultricies enim ut tellus suscipit, nec placerat odio dapibus. Fusce aliquam condimentum enim, et dignissim elit. Aenean auctor blandit dictum. Proin orci mauris, commodo ac tellus et, hendrerit varius lectus. In consequat pharetra interdum. Cras rutrum faucibus dignissim. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nam gravida risus at nunc tincidunt, eu porttitor metus molestie. Cras rutrum lacus dui, consectetur tincidunt metus suscipit a.",
      },
      {
        index: 8,
        imagem: require("../assets/images/sgc-foto-4.jpg"),
        tituloImagem: "Imagem 8",
         textoImagem:
          "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum tincidunt magna justo, vel molestie risus dignissim vitae. Morbi ultricies enim ut tellus suscipit, nec placerat odio dapibus. Fusce aliquam condimentum enim, et dignissim elit. Aenean auctor blandit dictum. Proin orci mauris, commodo ac tellus et, hendrerit varius lectus. In consequat pharetra interdum. Cras rutrum faucibus dignissim. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nam gravida risus at nunc tincidunt, eu porttitor metus molestie. Cras rutrum lacus dui, consectetur tincidunt metus suscipit a.",
      },
      {
        index: 9,
        imagem: require("../assets/images/sgc-foto-4.jpg"),
        tituloImagem: "Imagem 9",
         textoImagem:
          "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum tincidunt magna justo, vel molestie risus dignissim vitae. Morbi ultricies enim ut tellus suscipit, nec placerat odio dapibus. Fusce aliquam condimentum enim, et dignissim elit. Aenean auctor blandit dictum. Proin orci mauris, commodo ac tellus et, hendrerit varius lectus. In consequat pharetra interdum. Cras rutrum faucibus dignissim. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nam gravida risus at nunc tincidunt, eu porttitor metus molestie. Cras rutrum lacus dui, consectetur tincidunt metus suscipit a.",
      },
    ],
    data3: [
      {
        index: 10,
        imagem: require("../assets/images/sgc-foto-4.jpg"),
        tituloImagem: "Imagem 10",
         textoImagem:
          "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum tincidunt magna justo, vel molestie risus dignissim vitae. Morbi ultricies enim ut tellus suscipit, nec placerat odio dapibus. Fusce aliquam condimentum enim, et dignissim elit. Aenean auctor blandit dictum. Proin orci mauris, commodo ac tellus et, hendrerit varius lectus. In consequat pharetra interdum. Cras rutrum faucibus dignissim. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nam gravida risus at nunc tincidunt, eu porttitor metus molestie. Cras rutrum lacus dui, consectetur tincidunt metus suscipit a.",
      },
      {
        index: 11,
        imagem: require("../assets/images/sgc-foto-4.jpg"),
        tituloImagem: "Imagem 12",
         textoImagem:
          "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum tincidunt magna justo, vel molestie risus dignissim vitae. Morbi ultricies enim ut tellus suscipit, nec placerat odio dapibus. Fusce aliquam condimentum enim, et dignissim elit. Aenean auctor blandit dictum. Proin orci mauris, commodo ac tellus et, hendrerit varius lectus. In consequat pharetra interdum. Cras rutrum faucibus dignissim. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nam gravida risus at nunc tincidunt, eu porttitor metus molestie. Cras rutrum lacus dui, consectetur tincidunt metus suscipit a.",
      },
      {
        index: 12,
        imagem: require("../assets/images/sgc-foto-4.jpg"),
        tituloImagem: "Imagem 12",
         textoImagem:
          "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum tincidunt magna justo, vel molestie risus dignissim vitae. Morbi ultricies enim ut tellus suscipit, nec placerat odio dapibus. Fusce aliquam condimentum enim, et dignissim elit. Aenean auctor blandit dictum. Proin orci mauris, commodo ac tellus et, hendrerit varius lectus. In consequat pharetra interdum. Cras rutrum faucibus dignissim. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nam gravida risus at nunc tincidunt, eu porttitor metus molestie. Cras rutrum lacus dui, consectetur tincidunt metus suscipit a.",
      },
      {
        index: 13,
        imagem: require("../assets/images/sgc-foto-4.jpg"),
        tituloImagem: "Imagem 13",
         textoImagem:
          "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum tincidunt magna justo, vel molestie risus dignissim vitae. Morbi ultricies enim ut tellus suscipit, nec placerat odio dapibus. Fusce aliquam condimentum enim, et dignissim elit. Aenean auctor blandit dictum. Proin orci mauris, commodo ac tellus et, hendrerit varius lectus. In consequat pharetra interdum. Cras rutrum faucibus dignissim. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nam gravida risus at nunc tincidunt, eu porttitor metus molestie. Cras rutrum lacus dui, consectetur tincidunt metus suscipit a.",
      },
    ],
  }),
};
</script>

<style>
</style>