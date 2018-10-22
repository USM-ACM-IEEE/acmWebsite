<template>
  <v-layout>
    <p>Hello World</p>
    <div class="text-xs-center">
      <v-dialog
        v-model="dialog"
        width="500"
      >
        <v-btn
          slot="activator"
          color="red lighten-2"
          dark
        >
          Click Me
        </v-btn>

        <v-card>
          <v-card-title
            class="headline grey lighten-2"
            primary-title
          >
            Hello World!
          </v-card-title>

          <v-card-text>
            Javascript Rules!
          </v-card-text>

          <v-divider></v-divider>

          <v-card-actions>
            <v-spacer></v-spacer>
            <v-btn
              color="primary"
              flat
              @click="dialog = false"
            >
              I Agree
            </v-btn>
          </v-card-actions>
        </v-card>
      </v-dialog>
    </div>
  </v-layout>
</template>

<script>
export default {
  data() {
    return {
      dialog: false,
    };
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1, h2 {
  font-weight: normal;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
