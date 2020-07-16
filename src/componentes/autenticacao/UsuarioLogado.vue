<template>
  <v-card v-if="usuario" class="ma-2 pa-1">
    <v-layout fill-height align-center>
      <v-flex>
        <span class="ml-3 body-1">Nome:{{' '}}</span>
        <span class="body-1 blue--text text--darken-2">{{ usuario.nome }}</span>

        <span class="ml-3 body-1">Email:{{' '}}</span>
        <span class="body-1 blue--text text--darken-2">{{ usuario.email }}</span>

        <span class="ml-3 body-1">Perfis:{{' '}}</span>
        <span class="body-1 red--text text--darken-2">{{ perfis }}</span>
      </v-flex>
      <v-flex></v-flex>
      <v-flex shrink>
        <v-btn color="error" @click="setUsuario(null)" small flat>Sair</v-btn>
      </v-flex>
    </v-layout>
  </v-card>
</template>

<script>
import { mapGetters, mapActions } from "vuex";

export default {
  computed: {
    ...mapGetters(["usuario"]),
    perfis() {
      if (!this.usuario && !this.usuario.perfis) return null;
      return this.usuario.perfis.map(p => p.rotulo).join(", ");
    }
  },
  methods: mapActions(["setUsuario"])
};
</script>

<style>
</style>
