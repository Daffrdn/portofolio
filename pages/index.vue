<template>
<div>
  <div><br><br>
    <h1>Hi, I'am Daffa</h1>
    <h1>A Web Developer</h1><br>
    <span>
     A Frontend Engineer focused  Web Developer <br> 
     building the Frontend of Websites and Web Applications <br> 
     that leads to success of the overall product 
    </span>
    <br><br><br>
    <v-btn outlined> My Projects</v-btn>
    <v-btn outlined> Contact Me!</v-btn>
  </div>
  <br><br><br><br><br><br>
  <div>
    <v-divider></v-divider>
  </div>
  <br><br>
  <div>
    <h1 class="text-center"> My Projects</h1>
  </div>
  <br><br>
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
        @click="Done"
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
        <v-hover v-slot="{ hover }">
          <v-card
            width="300"
            height="300"
            rounded
            outlined
            class="mx-auto d-flex align-center"
            router
            exact
            @click.stop="ewalle = true"
            :elevation="hover ? 8 : 0"
            :class="{ 'on-hover': hover }"
          >
            <div class="mx-auto" align="center" >
              <img src="/projects/1 51.png"  width="250"/>
            </div>
          </v-card>
        </v-hover>
        <v-dialog
          v-model="ewalle"
          max-width="1100"
        >
          <v-card>
            <v-container>
              <div class="d-flex justify-end">
                <v-icon
                  @click="ewalle = false"
                  
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
                <a href="https://walle-app.netlify.com">Here the Appplication that were builds..</a>
              </v-card-text>
            </v-col>
            </v-row>
            </v-container>
            <br>
          </v-card>
        </v-dialog>
      </v-col>
    </v-row>
  </div>
  <br><br>
  <div>
    <v-divider></v-divider>
  </div>
  <br><br>
  <div>
    <h1 class="text-center"> My Skills & Experience</h1>
  </div>
  <br><br>
  <div>
    <v-container>
    <v-row>
      <v-col cols="12" md="6" align="center">
        <strong>Frontend</strong>
        <v-progress-linear
          v-model="frontend"
          height="25"
          color="teal"
        >
          <strong class="white--text">{{ Math.ceil(frontend) }}%</strong>
        </v-progress-linear>
      </v-col>
      <v-col cols="12" md="6" align="center">
        <strong>Backend</strong>
        <v-progress-linear
          v-model="backend"
          height="25"
          color="lime"
        >
          <strong class="white--text">{{ Math.ceil(backend) }}%</strong>
        </v-progress-linear>
      </v-col>
    </v-row>
    </v-container>
    <br>
    <v-row>
      <v-col>
        <v-hover v-slot="{ hover }">
          <v-card
            width="200"
            height="200"
            outlined
            rounded
            class="mx-auto d-flex align-center"
            router
            exact
            :elevation="hover ? 8 : 0"
            :class="{ 'on-hover': hover }"
            @click.stop="html = true"
          >
            <div class="mx-auto" align="center" >
              <img src="/HTML.png"  width="150"/>
            </div>
          </v-card>
        </v-hover>
        <v-dialog
          v-model="html"
          max-width="600"
        >
          <v-card>
            <v-container>
              <div class="d-flex justify-end">
                <v-icon
                  @click="html = false"
                >
                  mdi-close
                </v-icon>
              </div>
              <v-card-title class="text-h5">
                HTML
                
              </v-card-title>
                <v-card-subtitle>Hypertext Markup Language</v-card-subtitle>
                <v-card-text>
                <v-progress-circular
                  v-model="htmlskill"
                  :width="15"
                  :size="100"
                  :value="htmlskill"
                  color="orange darken-4"
                >
                  <strong>{{ htmlskill }}</strong>
                </v-progress-circular>
                </v-card-text>
              <v-card-text>
              
              </v-card-text>
            </v-container>
          </v-card>
        </v-dialog>
      </v-col>
      <v-col>
        <v-hover v-slot="{ hover }">
          <v-card
            width="200"
            height="200"
            outlined
            rounded
            class="mx-auto d-flex align-center"
            :elevation="hover ? 8 : 0"
            :class="{ 'on-hover': hover }"
            @click.stop="css = true"
          >
            <div class="mx-auto" align="center" >
              <img src="/CSS.png"  width="150"/>
            </div>
          </v-card>
        </v-hover>
        <v-dialog
          v-model="css"
          max-width="600"
        >
          <v-card>
            <v-container>
              <div class="d-flex justify-end">
                <v-icon
                  @click="css = false"
                >
                  mdi-close
                </v-icon>
              </div>
              <v-card-title class="text-h5">
                CSS
                
              </v-card-title>
                <v-card-subtitle>Cascading Style Sheets</v-card-subtitle>
                <v-card-text>
                <v-progress-circular
                  v-model="cssskill"
                  :width="15"
                  :size="100"
                  :value="95"
                  color="blue darken-4"
                >
                  <strong>{{ cssskill }}</strong>
                </v-progress-circular>
                </v-card-text>
              <v-card-text>
              
              </v-card-text>
            </v-container>
          </v-card>
        </v-dialog> 
      </v-col>
      <v-col>
        <v-hover v-slot="{ hover }">
          <v-card
            :elevation="hover ? 8 : 0"
            :class="{ 'on-hover': hover }"
            @click.stop="js = true"
            width="200"
            height="200"
            outlined
            rounded
            class="mx-auto d-flex align-center"
          >
            <div class="mx-auto" align="center" >
              <img src="/Javascript-logo.png"  width="150"/>
            </div>
          </v-card>
        </v-hover>
        <v-dialog
          v-model="js"
          max-width="600"
        >
          <v-card>
            <v-container>
              <div class="d-flex justify-end">
                <v-icon
                  @click="js = false"
                >
                  mdi-close
                </v-icon>
              </div>
              <v-card-title class="text-h5">
                Javascript
                
              </v-card-title>
                <v-card-subtitle>Native Javascript</v-card-subtitle>
                <v-card-text>
                <v-progress-circular
                  v-model="jsskill"
                  :width="15"
                  :size="100"
                  :value="95"
                  color="amber lighten-2"
                >
                  <strong>{{ jsskill }}</strong>
                </v-progress-circular>
                </v-card-text>
              <v-card-text>
              
              </v-card-text>
            </v-container>
          </v-card>
        </v-dialog> 
      </v-col>
      <v-col>
        <v-hover v-slot="{ hover }">
          <v-card
            :elevation="hover ? 8 : 0"
            :class="{ 'on-hover': hover }"
            @click.stop="node = true"
            width="200"
            height="200"
            outlined
            rounded
            class="mx-auto d-flex align-center"
          >
            <div class="mx-auto" align="center" >
              <img src="/nodejs.png"  width="180"/>
            </div>
          </v-card>
        </v-hover>  
        <v-dialog
          v-model="node"
          max-width="600"
        >
          <v-card>
            <v-container>
              <div class="d-flex justify-end">
                <v-icon
                  @click="node = false"
                >
                  mdi-close
                </v-icon>
              </div>
              <v-card-title class="text-h5">
                Node JS
                
              </v-card-title>
                <v-card-subtitle>Node Javascript</v-card-subtitle>
                <v-card-text>
                <v-progress-circular
                  v-model="nodeskill"
                  :width="15"
                  :size="100"
                  :value="95"
                  color="grey darken-4"
                >
                  <strong>{{ nodeskill }}</strong>
                </v-progress-circular>
                </v-card-text>
              <v-card-text>
              
              </v-card-text>
            </v-container>
          </v-card>
        </v-dialog> 
      </v-col>
      <v-col>
        <v-hover v-slot="{ hover }">
          <v-card
            :elevation="hover ? 8 : 0"
            :class="{ 'on-hover': hover }"
            @click.stop="php = true"
            width="200"
            height="200"
            outlined
            rounded
            class="mx-auto d-flex align-center"
          >
            <div class="mx-auto" >
              <img src="/php.png"  width="180"/>
            </div>
          </v-card>
        </v-hover>
        <v-dialog
          v-model="php"
          max-width="600"
        >
          <v-card>
            <v-container>
              <div class="d-flex justify-end">
                <v-icon
                  @click="php = false"
                >
                  mdi-close
                </v-icon>
              </div>
              <v-card-title class="text-h5">
                php
                
              </v-card-title>
                <v-card-subtitle>Cascading Style Sheets</v-card-subtitle>
                <v-card-text>
                <v-progress-circular
                  v-model="phpskill"
                  :width="15"
                  :size="100"
                  :value="95"
                  color="indigo lighten-2"
                >
                  <strong>{{ phpskill }}</strong>
                </v-progress-circular>
                </v-card-text>
              <v-card-text>
              
              </v-card-text>
            </v-container>
          </v-card>
        </v-dialog> 
      </v-col>
      <v-col>
        <v-hover v-slot="{ hover }">
          <v-card
            :elevation="hover ? 8 : 0"
            :class="{ 'on-hover': hover }"
            @click.stop="sql = true"
            width="200"
            height="200"
            outlined
            rounded
            class="mx-auto d-flex align-center"
          >
            <div class="mx-auto" >
              <img src="/MySQL.png"  width="180"/>
            </div>
          </v-card>
        </v-hover>  
        <v-dialog
          v-model="sql"
          max-width="600"
        >
          <v-card>
            <v-container>
              <div class="d-flex justify-end">
                <v-icon
                  @click="sql = false"
                >
                  mdi-close
                </v-icon>
              </div>
              <v-card-title class="text-h5">
                MySQL
                
              </v-card-title>
                <v-card-subtitle>Database MySQL</v-card-subtitle>
                <v-card-text>
                <v-progress-circular
                  v-model="sqlskill"
                  :width="15"
                  :size="100"
                  :value="95"
                  color="orange darken-1"
                >
                  <strong>{{ sqlskill }}</strong>
                </v-progress-circular>
                </v-card-text>
              <v-card-text>
              
              </v-card-text>
            </v-container>
          </v-card>
        </v-dialog> 
      </v-col>
      <v-col>
        <v-hover v-slot="{ hover }">
          <v-card
            :elevation="hover ? 8 : 0"
            :class="{ 'on-hover': hover }"
            @click.stop="laravel = true"
            width="200"
            height="200"
            outlined
            rounded
            class="mx-auto"
          >
            <div class="mx-auto mt-5" align="center" >
              <img src="/Laravel.svg"  width="150"/>
            </div>
          </v-card>
        </v-hover>  
        <v-dialog
          v-model="laravel"
          max-width="600"
        >
          <v-card>
            <v-container>
              <div class="d-flex justify-end">
                <v-icon
                  @click="laravel = false"
                >
                  mdi-close
                </v-icon>
              </div>
              <v-card-title class="text-h5">
                Laravel
                
              </v-card-title>
                <v-card-subtitle>Framework Laravel PHP</v-card-subtitle>
                <v-card-text>
                <v-progress-circular
                  v-model="laravelskill"
                  :width="15"
                  :size="100"
                  :value="95"
                  color="red darken-1"
                >
                  <strong>{{ laravelskill }}</strong>
                </v-progress-circular>
                </v-card-text>
              <v-card-text>
              
              </v-card-text>
            </v-container>
            <br>
          </v-card>
        </v-dialog> 
      </v-col>
      <v-col>
        <v-hover v-slot="{ hover }">
          <v-card
            :elevation="hover ? 8 : 0"
            :class="{ 'on-hover': hover }"
            @click.stop="vue = true"
            width="200"
            height="200"
            outlined
            rounded
            class="mx-auto"
          >
            <div class="mx-auto mt-5" align="center" >
              <img src="/Vue.png"  width="180"/>
            </div>
          </v-card>
        </v-hover> 
        <v-dialog
          v-model="vue"
          max-width="600"
        >
          <v-card>
            <v-container>
              <div class="d-flex justify-end">
                <v-icon
                  @click="vue = false"
                >
                  mdi-close
                </v-icon>
              </div>
              <v-card-title class="text-h5">
                Vue
                
              </v-card-title>
                <v-card-subtitle>Framework Vue Javascript</v-card-subtitle>
                <v-card-text>
                <v-progress-circular
                  v-model="vueskill"
                  :width="15"
                  :size="100"
                  :value="95"
                  color="green lighten-1"
                >
                  <strong>{{ vueskill }}</strong>
                </v-progress-circular>
                </v-card-text>
              <v-card-text>
              
              </v-card-text>
            </v-container>
            <br>
          </v-card>
        </v-dialog>  
      </v-col>
      <v-col>
        <v-hover v-slot="{ hover }">
          <v-card
            :elevation="hover ? 8 : 0"
            :class="{ 'on-hover': hover }"
            @click.stop="react = true"
            width="200"
            height="200"
            outlined
            rounded
            class="mx-auto"
          >
            <img src="/React.png" width="200"/>
          </v-card>
        </v-hover>  
        <v-dialog
          v-model="react"
          max-width="600"
        >
          <v-card>
            <v-container>
              <div class="d-flex justify-end">
                <v-icon
                  @click="react = false"
                >
                  mdi-close
                </v-icon>
              </div>
              <v-card-title class="text-h5">
                React 
                
              </v-card-title>
                <v-card-subtitle>Framework React Javascript</v-card-subtitle>
                <v-card-text>
                <v-progress-circular
                  v-model="reactskill"
                  :width="15"
                  :size="100"
                  :value="95"
                  color="blue lighten-3"
                >
                  <strong>{{ reactskill }}</strong>
                </v-progress-circular>
                </v-card-text>
              <v-card-text>
              
              </v-card-text>
            </v-container>
            <br>
          </v-card>
        </v-dialog> 
      </v-col>
    </v-row>
  </div>
  <br><br>
  <div>
    <v-divider></v-divider>
  </div>
  <br><br>
  <div>
    <h1 class="text-center"> My Contact</h1>
  </div>
  <br><br>
  <div>
    <v-row>
      <v-col cols="12" md="3">
        <div class="d-flex justify-center mt-2" >
          <img src="/profile.jpeg"  width="200"/>
        </div>
      </v-col>
      <v-col class="mx-auto" cols="12" md="4">
        <br>
        <h3>Daffa Erdian Fahrezy</h3>
        <br>
        <span>Hi, My name is Daffa Erdian Fahrezy, im 21 years old, if your need something just call me or text me in the down below... </span>
        <br><br>
        <v-btn 
        icon
        href="https://wa.me/0895372254680">
          <v-icon x-large color="black">
              mdi-whatsapp
          </v-icon>
        </v-btn>
        <v-btn 
        icon
        href="https://github.com/Daffrdn">
          <v-icon x-large color="black">
              mdi-github
          </v-icon>
        </v-btn>
        <v-btn 
        icon
        href="https://www.linkedin.com/in/daffa-erdian-fahrezy-611635148/">
          <v-icon x-large color="black">
              mdi-linkedin
          </v-icon>
        </v-btn>
        <v-btn 
        icon
        href="https://www.linkedin.com/in/daffa-erdian-fahrezy-611635148/">
          <v-icon x-large color="black">
              mdi-gmail
          </v-icon>
        </v-btn>
      </v-col>
      <v-col>
        <div>
          My Location:
          <iframe 
          src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3961.091774614524!2d107.60653793998947!3d-6.879608010212437!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x2e68e6f1a2c477bf%3A0x69776f70b1f628e6!2s4JC4%2BC4G%2C%20Hegarmanah%2C%20Cidadap%2C%20Bandung%20City%2C%20West%20Java%2040141!5e0!3m2!1sen!2sid!4v1664260156165!5m2!1sen!2sid" 
          width="450" 
          height="200" 
          style="border:0;" 
          allowfullscreen="" 
          loading="lazy" 
          referrerpolicy="no-referrer-when-downgrade"
          outlined
          >
          </iframe>
        </div>
      </v-col>
    </v-row>
  </div>
  <br><br>
</div>
</template>

<script>
export default {
  name: 'IndexPage',
  data () {
      return {
        ewalle: false,
        html: false,
        css: false,
        js: false,
        php: false,
        node: false,
        sql: false,
        vue: false,
        react: false,
        laravel: false,
        htmlskill: 95,
        cssskill: 70,
        jsskill: 70,
        nodeskill: 80,
        phpskill: 60,
        sqlskill: 75,
        laravelskill: 50,
        vueskill: 90,
        reactskill: 60,
        frontend: 70,
        backend: 50,

        query: false,
        show: true,
      }
    },
}
</script>
