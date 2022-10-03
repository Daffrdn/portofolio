<template>
<v-container>
  <div>
    <h1 class="text-center"> My Projects</h1>
  </div>
  <br>
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
        >
        <h3>On-Going</h3>
        <h1>0</h1>
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
        <h3>Done!</h3>
        <h1>1</h1>
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

</style>

