<template>
  <div id="bloqueContactos" style="margin-bottom: -80px">
    <v-sheet color="#000345">
      <v-container fluid class="px-4 justify-center">
        <v-row no-gutters class="justify-center">

          <v-col cols="12" md="4" sm="6" id="footContact">
            <v-card color="#000345" flat tile dark>
              <v-card-title class="justify-center pt-7">
                <h3 style="letter-spacing:4px;" class="mayeka">INFORMACIÓN</h3>
              </v-card-title>
              <v-card-text class="">
                <p class="text-center mayeka inf-text">
                  <a style="font-size:11pt; text-decoration:none; color:white">
                    Reglas y Terminos
                  </a>
                </p>

                <p class="text-center mayeka inf-text">
                  <a href="soporte@caribeapuesta.com" target="soporte@caribeapuesta.com" style="font-size:11pt; text-decoration:none; color:white">
                    soporte@caribeapuesta.com
                  </a>
                </p>

                <p class="text-center mayeka inf-text">
                  <a style="font-size:11pt; text-decoration:none; color:white">
                    Número: +58-412-3010777
                  </a>
                </p>

                <p class="text-center mayeka inf-text">
                  <a style="font-size:11pt; text-decoration:none; color:white">
                    RIF: J-409540634
                  </a>
                </p>
              </v-card-text>
            </v-card>
          </v-col>

          <v-col cols="12" md="4" sm="6" id="footDirection">
            <v-card-text class="pt-7 text-center">  
                <div class="logo-18plus text-center" style="display:inline-block;vertical-align:middle;float:none;">
                  18+
                </div>
                <p class="text-center mayeka mt-2" style="font-size:10pt; color:white">
                  Caribe Apuesta no permite el ingreso a niños o menores de edad. Si no tienes mas de 18 años, por favor abstente de ingresar al sitio web. El juego puede ser adictivo, por favor juega responsablemente.
                </p>
            </v-card-text>
          </v-col>

          <v-col cols="12" md="4" sm="6" id="footDirection" >
            <v-row class="py-4 ">
              <v-col class="white--text mayeka pb-0 d-flex justify-end" cols="6" md="6" sm="6" id="footImages">
                <v-card color="#000345" width="160" flat tile class="text-center">
                  <img src="@/assets/images/inh.png" width="160" height="auto"/>
                </v-card>
              </v-col>

              <v-col class="white--text mayeka pb-0 d-flex justify-center" cols="6" md="6" sm="6" id="footImages">
                <v-card color="white" width="160" flat class="text-center">
                  <img src="@/assets/images/conalot.png" width="130" height="auto"/>
                </v-card>
              </v-col>
              <v-col class="white--text mayeka pb-0 d-flex justify-end" cols="6" md="6" sm="6" id="footImages">
                <v-card color="#000345" width="160" flat tile class="text-center">
                  <img src="@/assets/images/lim.jpg" width="70" height="auto"/>
                </v-card>
              </v-col>

              <v-col class="white--text mayeka pb-0 d-flex justify-center" cols="6" md="6" sm="6" id="footImages">
                <v-card color="white" width="160" flat class="text-center">
                  <img src="@/assets/images/sunahip.jpg" width="130" height="auto"/>
                </v-card>
              </v-col>
            </v-row>


          </v-col>

        </v-row>

        <v-row no-gutters class="justify-center" style="border-top: 1px solid white">
          <v-col cols="12" md="4" sm="6" id="footDirection">
            <v-card color="#000345" flat tile class="text-center">
              <v-card-title class="justify-center">
                <v-btn icon fab dark class="ml-4" href="https://twitter.com/caribeapuesta_" target="https://twitter.com/caribeapuesta_">
                  <v-icon size="35">mdi-twitter</v-icon>
                </v-btn>
                <v-btn icon fab dark class="ml-4" href="https://www.instagram.com/caribeapuesta/" target="https://www.instagram.com/caribeapuesta/">
                  <v-icon size="35">mdi-instagram</v-icon>
                </v-btn>
                <v-btn icon fab dark class="ml-4" href="https://www.facebook.com/Caribe-Apuesta-115899600246533" target="https://www.facebook.com/Caribe-Apuesta-115899600246533">
                  <v-icon size="35">mdi-facebook</v-icon>
                </v-btn>
              </v-card-title>
            </v-card>
          </v-col>

          <v-col class="white--text mayeka pb-0" cols="12" md="4" sm="6" id="footImages">
            <v-card color="#000345" flat tile class="text-center pa-0">
              <img src="@/assets/images/Logo-02.png" width="150" height="auto"/>
            </v-card>
          </v-col>

          <v-col class="white--text mayeka pb-0" cols="12" md="4" sm="6" id="footImages">
            <v-card color="#000345" flat tile class="text-center">
              <img src="@/assets/images/ssl-certificate.png" width="150" height="auto"/>
            </v-card>
          </v-col>
        </v-row>
      </v-container>
    </v-sheet>
  </div>
</template>

<script>
export default {
  name: "bloqueContactos",
};
</script>

<style>
  .logo-18plus {
    color: #fff;
    background-color: #000345;
    border: 3px solid #fff;
    border-radius: 50%;
    width: 60px;
    height: 60px;
    line-height: 55px;
    text-align: center;
    font-size: 28px;
    font-weight: bold;
    float: left;
    display: block;
    margin-right: 4px;
  }

  .inf-text:hover{
    font-weight: bold;
  }
</style>

