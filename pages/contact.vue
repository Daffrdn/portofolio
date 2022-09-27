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
        <v-card
        elevation="0"
        height="180"
        width="450"
        color="grey"
        >
        </v-card>
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
                    label="Outlined"
                    placeholder="Placeholder"
                    outlined
                    ></v-text-field>
                </v-col>
                <v-col>
                    <span>E-mail:</span>
                    <v-text-field
                    label="Outlined"
                    placeholder="Placeholder"
                    outlined
                    ></v-text-field>
                </v-col>
            </v-row>
            <span>Messages:</span>
            <v-textarea
            outlined
            rows="8"
            label="Outlined textarea"
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