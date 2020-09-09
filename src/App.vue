<template>
  <v-app>
    <v-navigation-drawer v-model="side_menu" absolute temporary style="position: fixed">
      <v-list dense>
        <v-list-item v-for="item in items" :key="item.title" link>
          <v-list-item-icon>
            <v-icon color="#000033">{{ item.icon }}</v-icon>
          </v-list-item-icon>

          <v-list-item-content>
            <v-list-item-title 
              color="#000033" class="mayeka" v-if="item.title !== 'INICIAR SESIÓN' && item.title !== 'REGISTRARSE'"
              @click="$vuetify.goTo( item.redirection, 0, 2000)">
              {{ item.title }}
            </v-list-item-title>

            <v-list-item-title 
              color="#000033" class="mayeka" v-else>
              {{ item.title }}
            </v-list-item-title>
          </v-list-item-content>
        </v-list-item>
      </v-list>
    </v-navigation-drawer>

    <v-app-bar app color="#000033" dark prominent>
      <div
        class="d-flex align-center"
        data-aos="fade-right"
        data-aos-duration="1000"
        data-aos-once="true"
        data-aos-easing="ease-in-out-sine"
      >
        <v-btn fab icon dark @click.stop="side_menu = !side_menu" class="d-md-none d-xl-flex">
          <v-icon>mdi-menu</v-icon>
        </v-btn>
        <v-img
          alt="Caribe apuesta logo"
          id="logoLogo"
          class="shrink mr-2 py-3"
          contain
          src="@/assets/images/ELEMENTO.png"
          transition="scale-transition"
          width="80"
          @click="$vuetify.goTo('#bloqueCasinoApuesta', 50, 2000)"
          style="cursor: pointer"
        />

        <v-img
          alt
          id="logoText"
          class="shrink mt-1 hidden-sm-and-down"
          contain
          min-width="100"
          src="@/assets/images/caribe_Mesa de trabajo 1.png"
          width="390"
        />
      </div>

      <v-spacer></v-spacer>

      <v-row id="menuOptions">
        <v-col cols="12" class="d-flex justify-end">
          <v-btn
            class="mt-7 mayeka"
            text
            data-aos="zoom-out-down"
            data-aos-duration="2750"
            data-aos-once="true"
            @click="$vuetify.goTo('#bloqueJuegos', 0, 2000)"
          >JUEGOS</v-btn>
          <v-btn
            class="mt-7 mayeka"
            text
            data-aos="zoom-out-down"
            data-aos-duration="3000"
            data-aos-once="true"
            @click="$vuetify.goTo('#bloqueComoJugar', 0, 2000)"
          >CÓMO JUGAR</v-btn>
          <v-btn
            class="mt-7 mayeka"
            text
            data-aos="zoom-out-down"
            data-aos-duration="3250"
            data-aos-once="true"
            @click="$vuetify.goTo('#bloquePagos', 0, 2000)"
          >PAGOS</v-btn>
          <v-btn
            class="mt-7 mayeka"
            text
            data-aos="zoom-out-down"
            data-aos-duration="3500"
            data-aos-once="true"
            @click="$vuetify.goTo('#resultados', 0, 2000)"
          >RESULTADOS</v-btn>
          <v-dialog v-model="regisrarse" width="700">
            <template v-slot:activator="{on,attrs}">
              <v-btn
                v-on="on"
                v-bind="attrs"
                class="mt-7 mayeka"
                outlined
                rounded
                data-aos="zoom-out-down"
                data-aos-duration="3750"
                data-aos-once="true"
              >REGISTRARSE</v-btn>
            </template>

            <v-card color="#000033" light elevation="12">
              <v-card-title class="justify-center">
                <img src="@/assets/images/logo.png" alt="Caribe Apuesta" width="150" />
              </v-card-title>
              <v-card-text class="pb-0">
                <v-container fluid class="px-4 pb-0">
                  <v-form>
                    <v-row >
                    <v-col cols="12" class="pb-0">
                    <v-text-field class="mayeka" rounded solo placeholder="USUARIO"></v-text-field>
                    </v-col>
                    <v-col cols="6" class="pb-0">
                    <v-text-field class="mayeka" rounded solo placeholder="NOMBRE"></v-text-field>

                    </v-col>
                    <v-col cols="6" class="pb-0">

                    <v-text-field class="mayeka" rounded solo placeholder="CÉDULA"></v-text-field>
                    </v-col>
                    <v-col cols="12" class="pb-0">
                    <v-text-field class="mayeka" rounded solo placeholder="CORREO"></v-text-field>
                    <v-text-field class="mayeka" rounded solo placeholder="REPETIR CORREO"></v-text-field>

                    </v-col>
                    <v-col cols="6" class="pb-0">
                    <v-text-field class="mayeka" rounded solo placeholder="CONTRASEÑA"></v-text-field>

                    </v-col>
                    <v-col cols="6" class="pb-0">
                    <v-text-field class="mayeka" rounded solo placeholder="REPETIR CONTRASEÑA"></v-text-field>

                    </v-col>
                    </v-row>
                  </v-form>
                </v-container>
              </v-card-text>
              <v-card-actions class="d-flex justify-center pt-0 pb-8">
                <v-btn rounded outlined color="white" large class="mayeka">CREAR USUARIO</v-btn>
              </v-card-actions>
            </v-card>
          </v-dialog>

          <v-dialog v-model="regisrarse" width="500">
            <template v-slot:activator="{on,attrs}">
              <v-btn
                v-on="on"
                v-bind="attrs"
                class="mt-7 mayeka"
                text
                data-aos="zoom-out-down"
                data-aos-duration="4000"
                data-aos-once="true"
              >INICIAR SESIÓN</v-btn>
            </template>

            <v-card color="#000033" light elevation="12">
              <v-card-title class="justify-center">
                <img src="@/assets/images/logo.png" alt="Caribe Apuesta" width="150" />
              </v-card-title>
              <v-card-text class="pb-0">
                <v-container fluid class="px-4 pb-0">
                  <v-form>
                    <v-text-field class="mayeka" rounded solo placeholder="USUARIO O EMAIL"></v-text-field>
                    <v-text-field class="mayeka" rounded solo placeholder="CONTRASEÑA"></v-text-field>
                  </v-form>
                </v-container>
              </v-card-text>
              <v-card-actions class="d-flex justify-center pt-0 pb-8">
                <v-btn rounded outlined color="white" class="mayeka">INICIAR SESIÓN</v-btn>
              </v-card-actions>
            </v-card>
          </v-dialog>
        </v-col>
      </v-row>
    </v-app-bar>

    <v-main>
      <bloque1></bloque1>
      <bloque2></bloque2>
      <bloque3></bloque3>
      <bloque4></bloque4>
      <bloque5></bloque5>
      <bloque6></bloque6>
      <bloque7></bloque7>
    </v-main>

    <v-footer padless app style="background-color: rgba(0,0,0,0);">
      <v-row class="text-right">
        <v-col>
          <v-dialog v-model="chat" hide-overlay>
            <template v-slot:activator="{on,attrs}">
              <v-btn v-on="on" v-bind="attrs" absolute right top v-model="fab" light class="mr-8">
                <span>CHAT EN VIVO</span>
              </v-btn>
            </template>
            <v-container fluid id="#box">
              <v-row>
                <v-col cols="12">
                  <v-card class="float-right mayeka" width="300" min-height="300">
                    <v-card-title>
                      CHAT EN VIVO
                      <v-spacer></v-spacer>
                      <v-btn icon @click="chat=false">
                        <v-icon>mdi-close</v-icon>
                      </v-btn>
                    </v-card-title>
                    <v-divider></v-divider>
                    <v-card-text>
                      Lorem ipsum dolor sit amet,
                      consectetur adipisicing elit. Illo dolorem doloremque deserunt
                      asperiores consequatur dolore, totam nam velit corrupti recusandae iste,
                      soluta earum obcaecati ex et hic tenetur, illum harum?
                      Lorem ipsum dolor sit, amet consectetur adipisicing elit. Accusamus, tempora molestiae. Ex magnam fugit
                      eaque vitae obcaecati modi ipsum natus commodi? Magni aliquid inventore,
                      mollitia neque porro vel eveniet soluta?
                    </v-card-text>
                    <v-divider></v-divider>
                    <v-card-actions>
                      <v-form>
                        <v-text-field outlined class="mayeka mt-6" placeholder="ESCRIBE AQUÍ"></v-text-field> 
                      </v-form>
                      
                      <v-btn icon fab right absolute>
                        <v-icon>mdi-send</v-icon>
                      </v-btn>
                    </v-card-actions>
                  </v-card>
                </v-col>
              </v-row>
            </v-container>
          </v-dialog>
        </v-col>
        <v-col class="pb-0 pt-2">
          <v-btn dark icon fab light>
            <v-icon size="35" v-on:click="redirectWapp">mdi-whatsapp</v-icon>
          </v-btn>
        </v-col>
        <v-col cols="12" style="background-color: #000033">
          <h4
            id="text-footer"
            class="d-flex justify-center white--text mayeka"
            style="font-size: 8px"
          >&copy; {{ new Date().getFullYear() }} MANUAL CODE - TODOS LOS DERECHOS RESERVADOS</h4>
        </v-col>
      </v-row>
    </v-footer>
  </v-app>
</template>

<script>
import bloque1 from "@/components/bloqueCasinoApuesta.vue";
import bloque2 from "@/components/bloqueJuegos.vue";
import bloque3 from "@/components/bloqueComoJugar.vue";
import bloque4 from "@/components/bloquePagos.vue";
import bloque5 from "@/components/bloqueQuienesSomos.vue";
import bloque6 from "@/components/bloqueParallax.vue";
import bloque7 from "@/components/bloqueContactos.vue";
import AOS from "aos";
export default {
  name: "App",

  components: {
    bloque1,
    bloque2,
    bloque3,
    bloque4,
    bloque5,
    bloque6,
    bloque7,
  },
  created() {
    AOS.init({});
  },
  data() {
    return {
      registrarse: false,
      chat: false,
      side_menu: false,
      items: [
        { title: "INICIAR SESIÓN", icon: "mdi-login-variant" },
        { title: "REGISTRARSE", icon: "mdi-account-plus-outline" },
        { title: "JUEGOS", icon: "mdi-poker-chip", redirection: "#bloqueJuegos" },
        { title: "¿CÓMO JUGAR?", icon: "mdi-help-circle-outline", redirection: "#bloqueComoJugar" },
        { title: "PAGOS", icon: "mdi-credit-card-multiple-outline", redirection: "#bloquePagos" },
        { title: "RESULTADOS", icon: "mdi-cards-playing-outline", redirection: "#resultados" },
      ],
    };
  },

  methods:{
    redirectWapp: function (event) {
      /* https://wa.me/584123010777?text=Buen día, tengo algunas dudas sobre Caribe Apuestas... */
      /* https://web.whatsapp.com/send?phone=584123010777 */
      window.open("https://web.whatsapp.com/send?phone=584123010777");
    }
  },
};
</script>

<style>
@font-face {
  font-family: "Mayeka";
  src: url("./assets/fonts/century-gothic.TTF");
}
@font-face {
  font-family: "Poiret";
  src: url("./assets/fonts/PoiretOne-Regular.ttf");
}
#box {
  box-shadow: 0 !important;
}
.img-fluid {
  max-width: 100%;
  max-height: 100%;
  margin: auto;
  display: block;
}
.poiret {
  font-family: "Poiret";
}
.mayeka {
  font-family: "Mayeka";
}
body[data-aos-duration="3250"] [data-aos],
[data-aos][data-aos][data-aos-duration="3250"] {
  transition-duration: 3250ms;
}

body[data-aos-duration="3500"] [data-aos],
[data-aos][data-aos][data-aos-duration="3500"] {
  transition-duration: 3500ms;
}

body[data-aos-duration="3750"] [data-aos],
[data-aos][data-aos][data-aos-duration="3750"] {
  transition-duration: 3750ms;
}
body[data-aos-duration="4000"] [data-aos],
[data-aos][data-aos][data-aos-duration="4000"] {
  transition-duration: 4000ms;
}
body[data-aos-duration="5000"] [data-aos],
[data-aos][data-aos][data-aos-duration="5000"] {
  transition-duration: 5000ms;
}
@media (max-width: 600px) {
  .letters,
  .letters3 {
    font-size: 8px !important;
  }
}
@media (max-width: 1300px) {
  #logoText {
    display: none;
  }
}

@media (max-width: 900px) {
  #logoText {
    display: block !important;
  }

  #menuOptions {
    display: none;
  }

  #logo {
    margin: auto;
  }
}

@media (max-width: 765px) {
  #logoText {
    display: none !important;
  }

  #logoLogo {
    margin: auto;
  }
}
</style>
