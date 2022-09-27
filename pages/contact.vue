<template>
<div>
  <div><br><br>
    <h1>Contact</h1>
  </div>
  <br>
  <div>
    <v-row>
        <v-col
        cols="12"
        md="5"
        >
            <h2>Daffa Erdian Fahrezy, 21 Years Old</h2>
            <br>
            <span>Hi, My name is Daffa Erdian Fahrezy, im from Indonesia, if your need something just call me or text me in the down below... </span>
            <div class="mt-2">
                <v-btn 
                icon
                href="wa.me/0895372254680">
                    <v-icon x-large color="black">
                        mdi-whatsapp
                    </v-icon>
                </v-btn>
                <span class="ml-1 black--text">+62 8953 7225 4680</span>
            </div>
            <div class="mt-2">
                <v-btn 
                icon
                href="https://www.linkedin.com/in/daffa-erdian-fahrezy-611635148/">
                    <v-icon x-large color="black">
                        mdi-linkedin
                    </v-icon>
                </v-btn>
                <span class="ml-1 black--text">Daffa Erdian Fahrezy</span>
            </div>
            <div class="mt-2">
                <v-btn 
                icon
                href="https://github.com/Daffrdn">
                    <v-icon x-large color="black">
                        mdi-github
                    </v-icon>
                </v-btn >
                <span class="ml-1 black--text">Daffrdn</span>
            </div>
            <br>
            <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3961.091774614524!2d107.60653793998947!3d-6.879608010212437!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x2e68e6f1a2c477bf%3A0x69776f70b1f628e6!2s4JC4%2BC4G%2C%20Hegarmanah%2C%20Cidadap%2C%20Bandung%20City%2C%20West%20Java%2040141!5e0!3m2!1sen!2sid!4v1664260156165!5m2!1sen!2sid" width="450" height="200" style="border:0;" allowfullscreen="" loading="lazy" referrerpolicy="no-referrer-when-downgrade"></iframe>
        </v-col>
        <v-col
        class="mx-auto"
        cols="12"
        md="7"
        >
            <v-row>
                <v-col>
                    <span>Name:</span>
                    <v-text-field
                    outlined
                    ></v-text-field>
                </v-col>
                <v-col>
                    <span>E-mail:</span>
                    <v-text-field
                    outlined
                    ></v-text-field>
                </v-col>
            </v-row>
            <span>Messages:</span>
            <v-textarea
            outlined
            rows="8"
            ></v-textarea>
            <v-btn 
            outlined 
            color="secondary"
            class="mx-auto d-flex justify-center"
            > 
                Submit
            </v-btn>
        </v-col>
    </v-row>
    <br><br>
  </div>
</div>
</template>

<script>
export default {
    name: "Contact",
    methods: {

    },
}
</script>

<style>

</style>