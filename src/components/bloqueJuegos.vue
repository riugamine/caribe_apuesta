<template>
  <div id="bloqueJuegos" class="my-0">
    <v-sheet color="#000033">
      <v-card color="#000033" elevation="0">
        <!--         <v-card-title class="white--text justify-center letters">
          <ul>
            <li>
              <a
                data-text="JUEGOS"
                class="mayeka"
                style="letter-spacing:10px; font-size:20pt"
              >JUEGOS</a>
            </li>
          </ul>
        </v-card-title>-->

        <v-row class="ma-0" style="overflow-x: hidden; overflow-y: hidden;">
          <v-col cols="12">
            <v-carousel cycle interval="6000">
              <v-carousel-item>
                <v-img src="@/assets/images/c-1.jpg"></v-img>
              </v-carousel-item>
              <v-carousel-item>
                <v-img src="@/assets/images/c-2.jpg"></v-img>
              </v-carousel-item>
              <v-carousel-item>
                <v-img src="@/assets/images/c-3.jpg"></v-img>
              </v-carousel-item>
            </v-carousel>
          </v-col>

          <v-row>
            <v-col cols="4" sm="6" md="8" lg="12" xl="12">
              <v-sheet color="#000033" max-width="1400" class="mx-auto">
                <v-slide-group show-arrows="desktop" dark v-model="slider" class="pa-4">
                  <!-- Juego 1 (Para realizar con un ciclo for se deben obtener las imagenes del servidor por medio de axios) -->
                  <v-hover v-slot:default="{ hover }">
                    <v-slide-item>
                      <v-card class="ma-4" width="300">
                        <v-img src="@/assets/images/juegos/j1.jpg">
                          <v-expand-transition>
                            <v-overlay v-if="hover" absolute color="#000033" opacity="0.5">
                              <v-btn large color="#000033">JUGAR</v-btn>
                            </v-overlay>
                          </v-expand-transition>
                        </v-img>
                      </v-card>
                    </v-slide-item>
                  </v-hover>
                  <!-- Juego 2 -->
                  <v-hover v-slot:default="{ hover }">
                    <v-slide-item>
                      <v-card class="ma-4" width="300">
                        <v-img src="@/assets/images/juegos/j2.jpg">
                          <v-expand-transition>
                            <v-overlay v-if="hover" absolute color="#000033" opacity="0.5">
                              <v-btn large color="#000033">JUGAR</v-btn>
                            </v-overlay>
                          </v-expand-transition>
                        </v-img>
                      </v-card>
                    </v-slide-item>
                  </v-hover>
                  <!-- Juego 3 -->
                  <v-hover v-slot:default="{ hover }">
                    <v-slide-item>
                      <v-card class="ma-4" width="300">
                        <v-img src="@/assets/images/juegos/j3.jpg">
                          <v-expand-transition>
                            <v-overlay v-if="hover" absolute color="#000033" opacity="0.5">
                              <v-btn large color="#000033">JUGAR</v-btn>
                            </v-overlay>
                          </v-expand-transition>
                        </v-img>
                      </v-card>
                    </v-slide-item>
                  </v-hover>
                  <!-- Juego 4 -->
                  <v-hover v-slot:default="{ hover }">
                    <v-slide-item>
                      <v-card class="ma-4" width="300">
                        <v-img src="@/assets/images/juegos/j4.jpg">
                          <v-expand-transition>
                            <v-overlay v-if="hover" absolute color="#000033" opacity="0.5">
                              <v-btn large color="#000033">JUGAR</v-btn>
                            </v-overlay>
                          </v-expand-transition>
                        </v-img>
                      </v-card>
                    </v-slide-item>
                  </v-hover>
                  <!-- Juego 5 -->
                  <v-hover v-slot:default="{ hover }">
                    <v-slide-item>
                      <v-card class="ma-4" width="300">
                        <v-img src="@/assets/images/juegos/j5.jpg">
                          <v-expand-transition>
                            <v-overlay v-if="hover" absolute color="#000033" opacity="0.5">
                              <v-btn large color="#000033">JUGAR</v-btn>
                            </v-overlay>
                          </v-expand-transition>
                        </v-img>
                      </v-card>
                    </v-slide-item>
                  </v-hover>
                  <!-- Juego 6 -->
                  <v-hover v-slot:default="{ hover }">
                    <v-slide-item>
                      <v-card class="ma-4" width="300">
                        <v-img src="@/assets/images/juegos/j6.jpg">
                          <v-expand-transition>
                            <v-overlay v-if="hover" absolute color="#000033" opacity="0.5">
                              <v-btn large color="#000033">JUGAR</v-btn>
                            </v-overlay>
                          </v-expand-transition>
                        </v-img>
                      </v-card>
                    </v-slide-item>
                  </v-hover>
                </v-slide-group>
              </v-sheet>
            </v-col>
          </v-row>
        </v-row>
        <!--         <v-row class="ma-0" style="overflow-x: hidden; overflow-y: hidden;">
          <v-col
            cols="12"
            xl="8"
            lg="8"
            md="8"
            sm="8"
            xs="12"
            class="post"
            data-aos="fade-down-right"
            data-aos-duration="2000"
            data-aos-once="false"
          >
            <v-img class="imgJuegos" src="@/assets/images/la-granjita.jpg" max-height="300"></v-img>
            <div class="post-s mayeka">
              <h2>Animalitos</h2>
            </div>
          </v-col>

          <v-col
            cols="12"
            xl="4"
            lg="4"
            md="4"
            sm="4"
            xs="12"
            class="post"
            data-aos="fade-down-left"
            data-aos-duration="2000"
            data-aos-once="false"
          >
            <v-img class="imgJuegos" src="@/assets/images/juego-4.jpg" max-height="300"></v-img>
            <div class="post-s mayeka">
              <h2>Caballos</h2>
            </div>
          </v-col>

          <v-col
            cols="12"
            xl="4"
            lg="4"
            md="4"
            sm="4"
            xs="12"
            class="post"
            data-aos="fade-up-right"
            data-aos-duration="2000"
            data-aos-once="false"
          >
            <v-img class="imgJuegos" src="@/assets/images/juego-3.jpg" max-height="300"></v-img>
            <div class="post-s mayeka">
              <h2>Parley</h2>
            </div>
          </v-col>

          <v-col
            cols="12"
            xl="8"
            lg="8"
            md="8"
            sm="8"
            xs="12"
            class="post"
            data-aos="fade-up-left"
            data-aos-duration="2000"
            data-aos-once="false"
          >
            <v-img class="imgJuegos" src="@/assets/images/juego-2.jpg" max-height="300"></v-img>
            <div class="post-s mayeka">
              <h2>Casino</h2>
            </div>
          </v-col>
        </v-row>-->
      </v-card>
    </v-sheet>
  </div>
</template>

<script>
export default {
  name: "bloqueJuegos",
  data() {
    return {
      slider: null,
    };
  },
};
</script>

<style>
.letters {
  display: flex;
  text-overflow: ellipsis;
  justify-content: center;
  align-items: center;
  overflow: hidden;
  padding: auto;
}

.letters ul {
  position: relative;
  display: flex;
  flex-direction: column;
}

.letters ul li {
  list-style: none;
  transition: 0.5s;
}

.letters ul li a {
  text-align: center;
  color: transparent;
  text-decoration: none;
  text-transform: uppercase;
  font-weight: 900;
  letter-spacing: 2px;
  font-size: 2em;
  padding: 0 10px;
  line-height: 1.2em;
}

.letters ul li a:before {
  content: attr(data-text);
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  padding: 0 10px;
  -webkit-text-stroke: 1.5px #ffffff;
  transform: translateX(0);
  transition: 0.5s;
  pointer-events: none;
}

.letters ul li a:hover:before {
  transform: translateX(100%);
  opacity: 0;
}

.letters ul li a:after {
  content: attr(data-text);
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  padding: 0 10px;
  color: #ffffff;
  transform: translateX(-100%);
  transition: 0.5s;
  opacity: 0;
  pointer-events: none;
}

.letters ul li a:hover:after {
  transform: translateX(0);
  opacity: 1;
}

/* ANIMACION DE LAS IMAGENES */
.post {
  position: relative;
  cursor: pointer;
}

.post:hover .post-s {
  width: 100%;
  height: 100%;
  box-sizing: content-box;
}

.post .imgJuegos {
  display: block;
}

.post-s {
  width: 0px;
  height: 100%;
  box-sizing: content-box;
  background: rgba(0, 0, 51, 0.8);
  position: absolute;
  top: 0;
  display: flex;
  justify-content: center;
  align-items: center;
  overflow: hidden;
  transition: 0.7s;
}

.post-s h2 {
  color: white;
  font-size: 25px;
  border: 2px solid white;
  padding: 10px 30px;
  box-shadow: -1px 2px 30px 5px rgba(255, 255, 255, 0.35);
}
.fondo {
  align-items: center;
  bottom: 0;
  justify-content: center;
  opacity: 0.5;
  position: absolute;
  width: 100%;
}
@media (max-width: 600px) {
  .post {
    padding-right: 0px !important;
    padding-left: 0px !important;
  }
}
</style>