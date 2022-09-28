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
                <a href="walle-app.netlify.com">Here the Appplication that were builds..</a>
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
    <h1 class="text-center"> My Skills</h1>
  </div>
  <br><br>
  <div>
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
                <v-progress-linear
                  v-model="htmlskill"
                  height="25"
                  color="orange darken-4"
                  :active="show"
                  :indeterminate="query"
                  :query="true"
                >
                  <strong class="white--text">{{ Math.ceil(htmlskill) }}%</strong>
                </v-progress-linear>
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
                <v-progress-linear
                  v-model="cssskill"
                  height="25"
                  color="blue darken-4"
                >
                  <strong class="white--text">{{ Math.ceil(cssskill) }}%</strong>
                </v-progress-linear>
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
                <v-progress-linear
                  v-model="jsskill"
                  height="25"
                  color="amber lighten-2"
                >
                  <strong class="white--text">{{ Math.ceil(jsskill) }}%</strong>
                </v-progress-linear>
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
                <v-progress-linear
                  v-model="nodeskill"
                  height="25"
                  color="grey darken-4"
                >
                  <strong class="white--text">{{ Math.ceil(nodeskill) }}%</strong>
                </v-progress-linear>
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
                <v-progress-linear
                  v-model="phpskill"
                  height="25"
                  color="indigo lighten-2"
                >
                  <strong class="white--text">{{ Math.ceil(phpskill) }}%</strong>
                </v-progress-linear>
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
                <v-progress-linear
                  v-model="sqlskill"
                  height="25"
                  color="orange darken-1"
                >
                  <strong class="white--text">{{ Math.ceil(sqlskill) }}%</strong>
                </v-progress-linear>
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
                <v-progress-linear
                  v-model="laravelskill"
                  height="25"
                  color="red darken-1"
                >
                  <strong class="white--text">{{ Math.ceil(laravelskill) }}%</strong>
                </v-progress-linear>
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
                <v-progress-linear
                  v-model="vueskill"
                  height="25"
                  color="green lighten-1"
                >
                  <strong class="white--text">{{ Math.ceil(vueskill) }}%</strong>
                </v-progress-linear>
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
                <v-progress-linear
                  v-model="reactskill"
                  height="25"
                  color="blue lighten-3"
                >
                  <strong class="white--text">{{ Math.ceil(reactskill) }}%</strong>
                </v-progress-linear>
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
      <v-col md="3">
        <v-card 
          elevation="0"
          width="220"
          height="240"
          rounded
          outlined
          class="d-flex align-center ml-5"
        >
        <div class="mx-auto mt-2" >
            <img src="/profile.jpeg"  width="200"/>
          </div>
        </v-card>
      </v-col>
      <v-col class="mr-auto">
        <br>
        <h3>Daffa Erdian Fahrezy</h3>
        <br>
        <span>A Frontend Engineer focused  Web Developer building <br>
        the Frontend of Websites and Web Applications that <br>
        leads to success of the overall product </span>
        <br><br>
        <a>Read More</a>
      </v-col>
      <v-col>
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

        query: false,
        show: true,
      }
    },
}
</script>
