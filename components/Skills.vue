<!-- Please remove this file from your project -->
<template>
<v-container>
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
              <v-card-title>
                <h3>Vue</h3>
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
          </v-card>
        </v-dialog> 
      </v-col>
    </v-row>
  </div>
</v-container>
</template>

<script>
export default {
  name: 'Skills',
  data () {
    return {
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
