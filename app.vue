<template>
    <v-container>
        <v-row justify="center" >
            <v-col cols="12" sm="10">
              <v-card class="elevation-6 mt-10"  >
               <v-window v-model="step">
                  <v-window-item :value="1">
                    <v-row>
                      <v-col cols="12" md="6">
                        <v-card-text class="mt-12">
                          <h4
                            class="text-center"
                          >Mindy</h4>
                          <v-row justify="center">
                            <v-col cols="12" sm="8">
                             
                            <v-text-field
                              label="Mail"
                              outlined
                              dense
                              color="blue"
                              autocomplete="false"
                             class="mt-16"
                            />
                            <v-text-field
                              label="Contraseña"
                              outlined
                              dense
                              color="blue"
                            autocomplete="false"
                             type="password"
                            
                            />
                              <v-row>
                                <v-col cols="12" sm="7">
                                  <v-checkbox
                         
                          label="Recordarme"
                          class="mt-n1"
                          color="blue"
                        > </v-checkbox>
                                </v-col>
                                <v-col cols="12" sm="5">
                                  <button class="caption blue--text">Restablecer contraseña</button>
                                </v-col>
                              </v-row>
                            <v-btn color="blue" dark block tile>Ingresar</v-btn>
                            </v-col>
                          </v-row>  
                        </v-card-text>
                      </v-col>
                      <v-img src="https://cdn.vuetifyjs.com/images/parallax/material.jpg" />
                      <v-col cols="12" md="6" class="blue rounded-bl-xl" >
                      <div style="  text-align: center; padding: 180px 0;">
                        <v-card-text class="white--text" >
                          <h3 class="text-center ">No tenés tu cuenta aún?</h3>
                          <h6
                            class="text-center"
                          >Creá tu cuenta para ser parte de <br> Mindy </h6>
                        </v-card-text>
                        <div class="text-center">
                          <v-btn tile outlined dark @click="step++">Crear cuenta</v-btn>
                        </div>
                        </div>
                      </v-col>
                    </v-row>
                  </v-window-item>
                  <v-window-item :value="2">
                    <v-row >
                      <v-col cols="12" md="6" class="blue rounded-br-xl">
                       <div style="  text-align: center; padding: 180px 0;">
                        <v-card-text class="white--text" >
                          <h3 class="text-center ">Ya ténes tu cuenta?</h3>
                          <h6
                            class="text-center"
                          >Logueate para poder ingresar al sistema</h6>
                        </v-card-text>
                        <div class="text-center">
                          <v-btn tile outlined dark @click="step--">Ingresar</v-btn>
                        </div>
                        </div>
                      </v-col>
  
                      <v-col cols="12" md="6">
                        <v-card-text class="mt-12">
                          <h4
                            class="text-center"
                          >Creá tu cuenta</h4>
                          <h6
                            class="text-center  grey--text "
                          >Sólo necesitas llenar los siguientes campos</h6>
                          <v-row justify="center">
                            <v-col cols="12" sm="8">
                             <v-row>
                             <v-col cols="12" sm="6">
                              <v-text-field
                              label="Nombre"
                              outlined
                              dense
                              color="blue"
                              autocomplete="false"
                             class="mt-4"
                            />
                             </v-col>
                             <v-col cols="12" sm="6">
                              <v-text-field
                              label="Apellido"
                              outlined
                              dense
                              color="blue"
                              autocomplete="false"
                             class="mt-4"
                            />
                             </v-col>
                             </v-row>
                            <v-text-field
                              label="Mail"
                              outlined
                              dense
                              color="blue"
                              autocomplete="false"
                            />
                            <v-text-field
                              label="Contraseña"
                              outlined
                              dense
                              color="blue"
                            autocomplete="false"
                             type="password"
                            
                            />
                              <v-row>
                                <v-col cols="12" sm="7">
                                </v-col>
                              </v-row>
                            <v-btn color="blue" dark block tile>Crear cuenta</v-btn>
                       
                           <div class="d-flex  justify-space-between align-center mx-10 mb-11">
                           </div>
                            </v-col>
                          </v-row>  
                        </v-card-text>
                      </v-col>
                    </v-row>
                  </v-window-item>
                </v-window>
              </v-card>
            </v-col>
        </v-row>
    </v-container>
  </template>
  
  <script>
    
  
    export default {
     data: () => ({
      step: 1
    }),
    props: {
      source: String
    } 
  
      
    }
  </script>
  <style scoped>
  .v-application .rounded-bl-xl {
      border-bottom-left-radius: 300px !important;
  }
  .v-application .rounded-br-xl {
      border-bottom-right-radius: 300px !important;
  }
  </style>