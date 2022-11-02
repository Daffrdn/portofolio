<template>
<div>
  <div id="home"><br><br>
    <h1>Hi, I'am Daffa</h1>
    <h1>A Web Developer</h1><br>
    <span>
     A Frontend Engineer focused  Web Developer <br> 
     building the Frontend of Websites and Web Applications <br> 
     that leads to success of the overall product 
    </span>
    <br><br><br>
    <v-btn outlined> My Projects</v-btn>
    <v-btn outlined href="#contact"> Contact Me!</v-btn>
  </div>
  <br><br><br><br><br><br>
  <div>
    <v-divider></v-divider>
  </div>
  <div id="projects">
    <Projects/>
    <v-hover v-slot="{ hover }">
      <v-card
        width="300"
        height="300"
        rounded
        outlined
        class="mx-auto d-flex align-center"
        router
        exact
        @click.stop="projects1 = true"
        :elevation="hover ? 8 : 0"
        :class="{ 'on-hover': hover }"
      >
        <div class="mx-auto" align="center" >
          <img src="/projects/1 51.png"  width="250"/>
        </div>
      </v-card>
    </v-hover>
    <v-dialog
      v-model="projects1"
      max-width="1100"
    >
      <v-card>
        <v-container>
          <div class="d-flex justify-end">
            <v-icon
              @click="projects1 = false"
            >
              mdi-close
            </v-icon>
          </div>
        <v-row>
          <v-col cols="12" md="6" class="mt-5">
            <img src="/projects/walle desktop.png" class="ml-3" width="500">
          </v-col>
          <v-col cols="12" md="6">
            <v-card-title class="text-h5">
              Wall E - Wallet Electronic
              
            </v-card-title>
              <v-card-subtitle>7 June - 21 July 2022</v-card-subtitle>
            <v-card-text>
            Wall E or known as Electronic Wallet is a top up service website using the PPOB tay system commonly known as Payment Point Online banking, which is a 24-hour real-time online bill payment service so that the data and fund reconciliation process can be faster and more accurate and safe.
            <br><br>
            This website was created by a team where there are several roles, namely Frontend, Backend, UI UX, Mobile Engineer, QE. Me and myfriend here as a Frontend Engineer Using Nuxt JS.
            </v-card-text>
            <v-card-text>
              <v-btn 
                outlined
                href="https://walle-app.netlify.app"
                color="green"
              >
              Demo!</v-btn>
            </v-card-text>
          </v-col>
        </v-row>
        </v-container>
        <br>
      </v-card>
    </v-dialog>
  </div>
  <br><br>
  <div>
    <v-divider></v-divider>
  </div>
  <div id="skills">
    <Skills/>
  </div>
  <br><br>
  <div>
    <v-divider></v-divider>
  </div>
  <div id="contact">
  <br><br>
  <Contact/>
  </div>
  <br><br>
</div>
</template>

<script>

export default {
  name: 'IndexPage',
  data() {
      return {
        projects1: false,
      }
  },
}
</script>

<style scoped>

</style>