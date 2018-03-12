<template>
  <v-app>
      <v-container>
          <v-layout>
              <v-flex xs6>
                 <v-card>
                 <h2>Poem</h2>
                <v-text-field v-model="poem"
                    name="poem-input"
                    label="Write here"
                    textarea
                    auto-grow
                class="input">
                </v-text-field>
                 </v-card> 
              </v-flex>

              <v-flex xs6>
                  <v-card>
                      <h2>Word Finder</h2>
                       <v-flex xs8>
                            <v-text-field
                                name="searchedWord"
                                label="Look up words"
                                single-line>
                            </v-text-field>
                        </v-flex>
                  </v-card>
              </v-flex>
          </v-layout>
      </v-container>
  </v-app>
</template>
<script>
 import axios from 'axios';
 export default {
   name: 'Main',
   data () {
     return {
       poem: '',
     }
   },
   computed: {
     },
   methods: {
   }
 }
</script>
