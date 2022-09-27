<template>
  <v-app ligth>
    <v-app-bar
      fixed
      app
      elevation="0"
      color="white"
    >
      <v-toolbar-title v-text="title" />
      <v-spacer />
      <v-btn 
       plain
       elevation="0"
       @click="home"
      >
        Home
      </v-btn>
      <v-btn
       plain
       elevation="0"
       @click="pro"
      >
        Projects
      </v-btn>
      <v-btn
       plain
       elevation="0"
       @click="exp"
      >
        Experience
      </v-btn>
      <v-btn
       plain
       elevation="0"
       @click="edu"
      >
        Education
      </v-btn>
      <v-btn
       plain
       elevation="0" 
       @click="con" 
      >
        Contact
      </v-btn>
    </v-app-bar>
    <v-main>
      <v-container>
        <Nuxt />
      </v-container>
    </v-main>
    <v-footer
      :absolute="!fixed"
      app
      dark
    >
      <v-btn 
       plain
       elevation="0"
       @click="home"
      >
        Home
      </v-btn>
      <v-btn
       plain
       elevation="0"
       @click="pro"
      >
        Projects
      </v-btn>
      <v-btn
       plain
       elevation="0"
       @click="exp"
      >
        Experience
      </v-btn>
      <v-btn
       plain
       elevation="0"
       @click="edu"
      >
        Education
      </v-btn>
      <v-btn
       plain
       elevation="0" 
       @click="con" 
      >
        Contact
      </v-btn>
      <v-spacer/>
      <span>&copy; {{ new Date().getFullYear() }} Daffa Erdian Fahrezy. Created with Nuxt</span>
    </v-footer>
  </v-app>
</template>

<script>
export default {
  name: 'DefaultLayout',
  data () {
    return {
      title: 'LOGO'
    }
  },
  methods: {
    home(){
      this.$router.push('/')
    },
    pro(){
      this.$router.push('projects')
    },
    edu(){
      this.$router.push('education')
    },
    exp(){
      this.$router.push('experience')
    },
    con(){
      this.$router.push('contact')
    },
  },
}
</script>
