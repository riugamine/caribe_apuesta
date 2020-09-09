<template>
  <div id="bloqueContactos" style="margin-bottom: -80px">
    <v-sheet color="#000345">
      <v-container fluid class="px-4">
        <v-row no-gutters class="justify-center">

          <v-col cols="12" md="4" sm="6" id="footContact">
            <v-card color="#000345" flat tile dark>
              <v-card-title class="justify-center pt-7">
                <h3 style="letter-spacing:8px;" class="mayeka">CONTACTOS</h3>
              </v-card-title>
              <v-card-text class="pt-10">
                <p class="text-center mayeka">
                  <a
                    href
                    class="my-12"
                    style="font-size:14pt; text-decoration:none; color:white"
                  >soporte@caribeapuesta.com</a>
                  <br />
                  <br />
                  <a href style="font-size:14pt; text-decoration:none; color:white">Link</a>
                  <br />
                  <br />
                  <a href style="font-size:14pt; text-decoration:none; color:white">Link</a>
                </p>
              </v-card-text>
            </v-card>
          </v-col>

          <v-col cols="12" md="4" sm="6" id="footDirection">
            <v-card color="#000345" flat tile dark>
              <v-card-title class="justify-center pt-7">
                <h3 style="letter-spacing:8px;" class="mayeka">DIRECCIÓN</h3>
              </v-card-title>
              <v-card-text class="pt-10">
                <p class="text-center mayeka">
                  <a
                    href
                    class="my-12"
                    style="font-size:14pt; text-decoration:none; color:white"
                  >CARIBEAPUESTA.COM</a>
                  <br />
                  <br />
                  <a href style="font-size:14pt; text-decoration:none; color:white">Link</a>
                  <br />
                  <br />
                  <a href style="font-size:14pt; text-decoration:none; color:white">Link</a>
                </p>
              </v-card-text>
            </v-card>
          </v-col>

          <v-col class="white--text mayeka pb-0" cols="12" md="4" sm="6" id="footImages">
            <v-card color="#000345" flat tile class="text-center">
              <v-card-title class="justify-center pb-0">
                <v-btn icon fab dark class="ml-4">
                  <v-icon size="35">mdi-whatsapp</v-icon>
                </v-btn>
                <v-btn icon fab dark class="ml-4">
                  <v-icon size="35">mdi-instagram</v-icon>
                </v-btn>
                <v-btn icon fab dark class="ml-4">
                  <v-icon size="35">mdi-facebook</v-icon>
                </v-btn>
              </v-card-title>
              
            </v-card>
            <v-card color="#000345" flat tile class="text-center pt-0" height="100">
              <img src="@/assets/images/+18.png" width="100" height="auto" />
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
  @media (max-width: 960px) {
    #footContact, #footDirection{
      border-bottom: 1px solid white;
    }
  }
</style>

