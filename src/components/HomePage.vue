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
          :textoImagem="item.textoImagem"
        ></card-foto>
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
        imagem:"@/src/assets/images/sgc-foto-1.jpg",
        tituloImagem: "Imagem 1",
        textoImagem: "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum tincidunt magna justo, vel molestie risus dignissim vitae. Morbi ultricies enim ut tellus suscipit, nec placerat odio dapibus. Fusce aliquam condimentum enim, et dignissim elit. Aenean auctor blandit dictum. Proin orci mauris, commodo ac tellus et, hendrerit varius lectus. In consequat pharetra interdum. Cras rutrum faucibus dignissim. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nam gravida risus at nunc tincidunt, eu porttitor metus molestie. Cras rutrum lacus dui, consectetur tincidunt metus suscipit a.",
      },
      {
        index: 2,
        imagem: '../../assets/images/sgc-foto-2.jpg',
        tituloImagem: "Imagem 2",
         textoImagem: "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum tincidunt magna justo, vel molestie risus dignissim vitae. Morbi ultricies enim ut tellus suscipit, nec placerat odio dapibus. Fusce aliquam condimentum enim, et dignissim elit. Aenean auctor blandit dictum. Proin orci mauris, commodo ac tellus et, hendrerit varius lectus. In consequat pharetra interdum. Cras rutrum faucibus dignissim. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nam gravida risus at nunc tincidunt, eu porttitor metus molestie. Cras rutrum lacus dui, consectetur tincidunt metus suscipit a.",
      },
      {
        index: 3,
        imagem: '../../assets/images/sgc-foto-3.jpg',
        tituloImagem: 'Imagem 3',
         textoImagem: "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum tincidunt magna justo, vel molestie risus dignissim vitae. Morbi ultricies enim ut tellus suscipit, nec placerat odio dapibus. Fusce aliquam condimentum enim, et dignissim elit. Aenean auctor blandit dictum. Proin orci mauris, commodo ac tellus et, hendrerit varius lectus. In consequat pharetra interdum. Cras rutrum faucibus dignissim. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nam gravida risus at nunc tincidunt, eu porttitor metus molestie. Cras rutrum lacus dui, consectetur tincidunt metus suscipit a.",
      },
      {
        index: 4,
        imagem: '../../assets/images/sgc-foto-4.jpg',
        tituloImagem: 'Imagem 4',
         textoImagem: "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum tincidunt magna justo, vel molestie risus dignissim vitae. Morbi ultricies enim ut tellus suscipit, nec placerat odio dapibus. Fusce aliquam condimentum enim, et dignissim elit. Aenean auctor blandit dictum. Proin orci mauris, commodo ac tellus et, hendrerit varius lectus. In consequat pharetra interdum. Cras rutrum faucibus dignissim. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nam gravida risus at nunc tincidunt, eu porttitor metus molestie. Cras rutrum lacus dui, consectetur tincidunt metus suscipit a.",
      },
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