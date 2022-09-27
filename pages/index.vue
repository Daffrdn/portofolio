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
        <v-card
          elevation="0"
          width="300"
          height="300"
          outlined
          rounded
          class="mx-auto d-flex align-center"
          router
        >
          <div class="mx-auto" align="center" >
            <img src="/projects/1 51.png"  width="250"/>
          </div>
        </v-card>
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
        <v-card
          elevation="0"
          width="200"
          height="200"
          outlined
          rounded
          class="mx-auto d-flex align-center"
        >
          <div class="mx-auto" align="center" >
            <img src="/HTML.png"  width="150"/>
          </div>
        </v-card>
      </v-col>
      <v-col>
        <v-card
          elevation="0"
          width="200"
          height="200"
          outlined
          rounded
          class="mx-auto d-flex align-center"
        >
          <div class="mx-auto" align="center" >
            <img src="/CSS.png"  width="150"/>
          </div>
        </v-card>
      </v-col>
      <v-col>
        <v-card
          elevation="0"
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
      </v-col>
      <v-col>
        <v-card
          elevation="0"
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
      </v-col>
      <v-col>
        <v-card
          elevation="0"
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
      </v-col>
      <v-col>
        <v-card
          elevation="0"
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
      </v-col>
      <v-col>
        <v-card
          elevation="0"
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
      </v-col>
      <v-col>
        <v-card
          elevation="0"
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
      </v-col>
      <v-col>
        <v-card
          elevation="0"
          width="200"
          height="200"
          outlined
          rounded
          class="mx-auto"
        >
          <img src="/React.png" width="200"/>
        </v-card>
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
  name: 'IndexPage'
}
</script>
