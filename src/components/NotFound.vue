<template>
  <div>
    <v-toolbar color="#2196F3">
      <v-toolbar-title align-center>Placeholder</v-toolbar-title>
      <v-spacer></v-spacer>
      <v-btn flat to='/'>Home</v-btn>
    </v-toolbar>
    <v-parallax
      :src="require('../assets/circuit.jpg')"
      dark
      alt = "circuit board image"
      class="temp1"
    >
      <v-layout
        align-center
        column
        justify-center
      >
        <h1 class="err404 display-4 font-weight-black">Error 404</h1>
        <h4 class="sub404 display-3 font-weight-black">
          The content you are looking for does not exist.
        </h4>
      </v-layout>
    </v-parallax>
    <v-layout justify-center row wrap>
      <v-flex xs11 elevation-5>
        <v-card>
          <v-card-text style="text-decoration: underline;">
            <div class="headline">
              Perhaps what you're looking for is here:
            </div>
          </v-card-text>
        </v-card>
      </v-flex>
      <v-flex xs5 ma-1 elevation-5>
        <v-card>
          <v-card-title primary-title>
            <div class="title font-weight-bold">
              Home Page
            </div>
          </v-card-title>
          <v-card-actions>
            <v-btn color="primary">Go</v-btn>
          </v-card-actions>
        </v-card>
      </v-flex>
      <v-flex xs5 ma-1 elevation-5>
        <v-card>
          <v-card-title primary-title>
            <div class="title font-weight-bold">
              Events
            </div>
          </v-card-title>
          <v-card-actions>
            <v-btn color="primary">Go</v-btn>
          </v-card-actions>
        </v-card>
      </v-flex>
      <v-flex xs5 ma-1 elevation-5>
        <v-card>
          <v-card-title primary-title>
            <div class="title font-weight-bold">
              Blog
            </div>
          </v-card-title>
          <v-card-actions>
            <v-btn color="primary">Go</v-btn>
          </v-card-actions>
        </v-card>
      </v-flex>
      <v-flex xs5 ma-1 elevation-5>
        <v-card>
          <v-card-title primary-title>
            <div class="title font-weight-bold">
              About
            </div>
          </v-card-title>
          <v-card-actions>
            <v-btn color="primary">Go</v-btn>
          </v-card-actions>
        </v-card>
      </v-flex>
      <v-flex xs11 elevation-5>
        <v-card>
          <v-card-text style="text-decoration: underline;">
            <div class="headline">
              Still don't see what you're looking for?
            </div>
          </v-card-text>
        </v-card>
      </v-flex>
      <v-flex xs8 ma-1 elevation-5>
        <v-card>
          <v-card-actions>
            <v-btn block color="error">Contact Us</v-btn>
          </v-card-actions>
        </v-card>
      </v-flex>
    </v-layout>
  </div>
</template>

<script>
export default {
  data() {
    return {
      windowWidth: {
        x: 0,
      },
    };
  },
  mounted() {
    this.onResize();
  },
  methods: {
    onResize() {
      this.windowWidth = { x: window.innerWidth };
    },
  },
};
</script>

<style scoped>
  .temp1{
    margin-bottom: 100px;
  }
  .err404{
    padding-left: 20px;
    padding-right: 20px;
    /*font-size: 70pt;
    font-weight: 1000;*/
    color: #C70000;
    background-color: hsla(0, 0%, 0%, 0.8);
    border-radius: 10px;
    box-shadow: 10px 10px 20px #000;
  }
  .sub404{
    margin-top: 10px;
    padding: 10px;
    /*font-size: 30pt;
    font-weight: 1000;*/
    background-color: hsla(0, 0%, 0%, 0.8);
    border-radius: 10px;
    box-shadow: 10px 10px 20px #000;
  }
</style>
