<template>
<v-container>
  <!-- <div>
    <h1 class="text-center"> My Contact</h1>
  </div> -->
  <div class="concept concept-six">
    <h1 class="word">
    <span class="char">C</span>
    <span class="char">o</span>
    <span class="char">n</span>
    <span class="char">t</span>
    <span class="char">a</span>
    <span class="char">c</span>
    <span class="char">t</span>
    </h1>
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
</v-container>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>

.hover,
.word,

h1 {
  position: relative  ;
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

.concept-six {
  display: flex;
  align-items: center;
}
.concept-six .word {
  width: 100px;
  margin: auto;
  display: flex;
  align-items: center;
  justify-content: center;
}
.concept-six .word:hover .char:nth-child(1) {
  margin-top: -30px;
  transform: rotate(-20deg);
}
.concept-six .word:hover .char:nth-child(2) {
  margin: -20px 0px 0 10px;
  transform: rotate(5deg);
}
.concept-six .word:hover .char:nth-child(3) {
  margin: 5px 0 0 10px;
  transform: rotate(12deg);
}
.concept-six .word:hover .char:nth-child(4) {
  margin: -20px 0 0;
  transform: rotate(5deg);
}
.concept-six .word:hover .char:nth-child(5) {
  margin: -40px 5px 0;
  transform: rotate(-10deg);
}
.concept-six .word:hover .char:nth-child(6) {
  margin: -20px 5px 0;
  transform: rotate(15deg);
}
.concept-six .word:hover .char:nth-child(7) {
  margin: -40px 5px 0;
  transform: rotate(10deg);
}
.concept-six .char {
  flex: 1;
  transition: 0.3s ease-in-out;
  position: relative;
}
</style>>
