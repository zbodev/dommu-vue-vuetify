<template>
  <v-dialog v-model="dialog" width="500">
    <template v-slot:activator="{ on }">
      <a v-on="on" href="#">Terms and Conditions</a>
    </template>
    <v-card>
      <v-card-title class="headline grey lighten-2" primary-title
        >Terms and Conditions</v-card-title
      >
      <v-card-text>
        Lorem sit dolor amet, consectetur adipiscing elit, sed do eiusmod tempor
        incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam,
        quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo
        consequat. Duis aute irure dolor in reprehenderit in voluptate velit
        esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat
        cupidatat non proident, sunt in culpa qui officia deserunt mollit anim
        id est laborum.
      </v-card-text>
      <v-divider></v-divider>
      <v-card-actions>
        <div class="flex-grow-1"></div>
        <v-btn color="primary" text @click="dialog = false">I accept</v-btn>
      </v-card-actions>
    </v-card>
  </v-dialog>
</template>
<script>
export default {
  name: "popup",
  data() {
    return {
      dialog: false,
      error: null
    };
  },
  methods: {}
};
</script>
<style scoped lang="scss"></style>
