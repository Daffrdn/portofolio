<template>
<v-container>
  <div class="d-flex justify-center concept concept-two">
    <div class="hover">
      <h1>Projects</h1>
    </div>
  </div>
  <div>
    <v-row>
      <v-col cols="12" md="2">
      </v-col>
      <v-col cols="12" md="4" align="center">
        <v-card
        width="100"
        router
        exact
        @click="ongoing"
        elevation="0"
        class="mx-auto"
        >
        <h2>On Going
          <br>0
        </h2>
        </v-card>
      </v-col>
      <v-col cols="12" md="4" align="center">
        <v-card
        width="100"
        router
        exact
        @click="done"
        elevation="0"
        >
        <h2>Done!
          <br>1
        </h2>
        </v-card>
      </v-col>
      <v-col cols="12" md="2">
      </v-col>
    </v-row>

    <v-row>
      <v-col>
        
      </v-col>
    </v-row>
  </div>
</v-container>
</template>

<script>
export default {
  data() {
      return {
        projects1: false,
      }
  },
  methods: {

  }
}
</script>

<style scoped>
.hover,
.word,

h1 {
  position: absolute;
  color:black;
}
.concept {
  position: relative;
  overflow: hidden;
  scroll-snap-align: center;
}
.concept:before {
  content: "";
  position: relative;
  top: 0;
  left: 0;
  opacity: 0;
  transition: all 1s cubic-bezier(0.19, 1, 0.22, 1);
}
.concept:hover:before {
  opacity: 0.5;
}

.concept-two {
  display: grid;
  grid: 100%/repeat(6, 1fr);
  padding: 5em 15em;
}
.concept-two .hover {
  position: relative;
  display: grid;
  place-items: center;
}
.concept-two h1 {
  color: transparent;
  -webkit-text-stroke: 2px BLACK;
  text-shadow: none;
  transition: 0.3s cubic-bezier(0.175, 0.885, 0.32, 1.275);
}
.concept-two .hover:hover h1 {
  transform: scale(1.5);
  color: black;
  -webkit-text-stroke: 2px transparent;
}
</style>

