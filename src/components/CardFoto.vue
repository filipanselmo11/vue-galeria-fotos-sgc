<template>
    <v-card class="mx-auto" max-width="344">
        <v-img :src="'caminhoImagem'"></v-img>
        <v-card-title>Foto Nº {{ index }}</v-card-title>
        <v-card-actions>
            <v-dialog transition="dialog-bottom-transition" max-width="600">
                <template v-slot:activator="{ on, attrs }">
                    <v-btn text v-bind="attrs" v-on="on">
                        Mais informações
                    </v-btn>
                </template>
                <template v-slot:default="dialog">
                    <v-card>
                        <v-toolbar color="light-blue darken-2" dark>
                            {{ tituloImagem }}
                        </v-toolbar>
                        <v-card-text>
                            {{ textoImagem }}
                        </v-card-text>
                        <v-card-actions class="justify-end">
                            <v-btn text @click="dialog.value = false">
                                Fechar
                            </v-btn>
                        </v-card-actions>
                    </v-card>
                </template>
            </v-dialog>
        </v-card-actions>
    </v-card>
</template>

<script>
export default {
    props:['index', 'caminhoImagem', 'tituloImagem', 'textoImagem'],
    data:() => ({
        reveal: false,
    }),
}
</script>

<style>

</style>