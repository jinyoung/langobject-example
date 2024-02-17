<template>
  <v-container class="fill-height">
    <v-responsive class="align-center text-center fill-height">
      
      <v-row class="d-flex align-center justify-center">
       
        <v-col cols="auto">

          <v-btn
            color="primary"
            href="https://vuetifyjs.com/introduction/why-vuetify/#feature-guides"
            min-width="228"
            rel="noopener noreferrer"
            size="x-large"
            target="_blank"
            variant="flat"
            @onclick="generate"
          >

            Generate
          </v-btn>
        </v-col>

        <v-col cols="auto">
          <v-btn
            href="https://community.vuetifyjs.com/"
            min-width="164"
            rel="noopener noreferrer"
            target="_blank"
            variant="text"
          >
            <v-icon
              icon="mdi-account-group"
              size="large"
              start
            />

            Community
          </v-btn>
        </v-col>
      </v-row>
    </v-responsive>
  </v-container>
</template>

<script setup>
  import langobject from 'langobject'

  class Publisher{
        //derives the prompt from the method and parameter names
        generateJoke(topic, language){}
        
  }

  //create AI version of Publisher
  let publisher = langobject(new Publisher())

  publisher.generateJoke("a cute dog", "Korean").then(joke => alert(joke));

</script>
