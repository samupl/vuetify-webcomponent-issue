<template>
  <div data-app>
    <v-menu>
      <template v-slot:activator="{ on, attrs }">
        <v-btn v-bind="attrs" v-on="on">click me </v-btn>
        <pre>{{ attrs }}</pre>
        <pre>{{ on }}</pre>
      </template>

      <v-list>
        <v-list-item>XXX</v-list-item>
      </v-list>
    </v-menu>

    <v-list>
      <v-list-item>Test list</v-list-item>
    </v-list>
  </div>
</template>

<script lang="ts">
import Vue from "vue";
import { VApp, VMenu, VBtn, VList, VListItem } from "vuetify/lib";
import vuetify from "@/plugins/vuetify";


export default Vue.extend({
  name: "App",
  vuetify,
  components: {
    VMenu, VBtn, VList, VListItem
  },
  data: () => ({
    //
  }),
});
</script>


<style lang="scss">
@import "vuetify/dist/vuetify";
</style>
