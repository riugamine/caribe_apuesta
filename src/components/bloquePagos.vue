<template>
  <div id="bloquePagos">
    <v-card color="white" light tile elevation="0" class="py-6">
      <v-card-title class="justify-center mayeka letters3">
        <ul>
          <li>
            <a
              data-text="MÉTODO DE PAGO"
              class="mayeka"
              style="letter-spacing:10px; color:#ffff; font-size:20pt"
            >MÉTODO DE PAGO</a>
          </li>
        </ul>
        <ul>
          <li>
            <a
              data-text="Y COBRO"
              class="mayeka"
              style="letter-spacing:10px; color:#ffff; font-size:20pt"
            >Y COBRO</a>
          </li>
        </ul>
      </v-card-title>
    </v-card>
    <v-sheet color="#000033" class="py-12">
      <v-container fluid class="py-12 px-15">
        <v-row no-gutters class="justify-center">
          <v-col color="#000033" class="d-flex child-flex" col lg="2" md="4" sm="4">
            <v-card color="#000033" class="text-center" elevation="0">
              <img
                src="@/assets/images/iconos/bs.png"
                width="150"
                data-aos="flip-right"
                data-aos-duration="2000"
                data-aos-once="false"
                data-aos-anchor-placement="bottom-bottom"
              />
              <v-card-text
                class="white--text mayeka forma-pago"
                data-aos="fade-right"
                data-aos-duration="3000"
                data-aos-anchor-placement="bottom-bottom"
                data-aos-once="false"
              >
                <v-expansion-panels flat class="panel" dark>
                  <v-expansion-panel>
                    <v-expansion-panel-header style="font-size:14pt; line-height:20pt">
                      BANCOS
                      <br />NACIONALES
                    </v-expansion-panel-header>
                    <v-expansion-panel-content>
                      <!-- Varias cuentas de bancos aca -->
                      <v-expansion-panels flat class="panel" dark>
                        <v-expansion-panel>
                          <v-expansion-panel-header style="font-size:14pt; line-height:20pt">BOD</v-expansion-panel-header>
                          <v-expansion-panel-content>
                            A NOMBRE DE: OPERADORA LOTO ORIENTE C.A
                            <br />RIF: PREGUNTAR
                            <br />CUENTA: 0116-0118-92-0029087988
                          </v-expansion-panel-content>
                        </v-expansion-panel>
                        <v-expansion-panel>
                          <v-expansion-panel-header style="font-size:14pt; line-height:20pt">BANESCO</v-expansion-panel-header>
                          <v-expansion-panel-content>
                            A NOMBRE DE: COMERCIALIZADORA GLOBAL 1618, C.A.
                            <br />RIF: J-40301941-0
                            <br />CUENTA: 0134-1200-670001002284
                          </v-expansion-panel-content>
                        </v-expansion-panel>
                      </v-expansion-panels>
                    </v-expansion-panel-content>
                  </v-expansion-panel>
                </v-expansion-panels>
              </v-card-text>
            </v-card>
          </v-col>
          <v-col color="#000033" class="d-flex child-flex" col lg="2" md="4" sm="4">
            <v-card color="#000033" class="text-center" elevation="0">
              <img
                src="@/assets/images/iconos/pm.png"
                width="150"
                data-aos="flip-right"
                data-aos-duration="2000"
                data-aos-once="false"
                data-aos-anchor-placement="bottom-bottom"
              />
              <v-card-text
                class="white--text mayeka forma-pago"
                data-aos="fade-right"
                data-aos-duration="3000"
                data-aos-anchor-placement="bottom-bottom"
                data-aos-once="false"
              >
                <v-expansion-panels flat class="panel" dark>
                  <v-expansion-panel>
                    <v-expansion-panel-header style="font-size:14pt">PAGO MÓVIL</v-expansion-panel-header>
                    <v-expansion-panel-content>datos pago movil</v-expansion-panel-content>
                  </v-expansion-panel>
                </v-expansion-panels>
              </v-card-text>
            </v-card>
          </v-col>
          <v-col color="#000033" class="d-flex child-flex" col lg="2" md="4" sm="4">
            <v-card color="#000033" class="text-center" elevation="0">
              <img
                src="@/assets/images/iconos/sk.png"
                width="150"
                data-aos="flip-right"
                data-aos-duration="2000"
                data-aos-once="false"
                data-aos-anchor-placement="bottom-bottom"
              />
              <v-card-text
                class="white--text mayeka forma-pago"
                data-aos="fade-right"
                data-aos-duration="3000"
                data-aos-anchor-placement="bottom-bottom"
                data-aos-once="false"
              >
                <v-expansion-panels flat class="panel" dark>
                  <v-expansion-panel>
                    <v-expansion-panel-header style="font-size:14pt">SKRILL</v-expansion-panel-header>
                    <v-expansion-panel-content>correo de skrill</v-expansion-panel-content>
                  </v-expansion-panel>
                </v-expansion-panels>
              </v-card-text>
            </v-card>
          </v-col>
          <v-col color="#000033" class="d-flex child-flex" col lg="2" md="4" sm="4">
            <v-card color="#000033" class="text-center" elevation="0">
              <img
                src="@/assets/images/iconos/pp.png"
                width="150"
                data-aos="flip-right"
                data-aos-duration="2000"
                data-aos-once="false"
                data-aos-anchor-placement="bottom-bottom"
              />
              <v-card-text
                class="white--text mayeka forma-pago"
                data-aos="fade-right"
                data-aos-duration="3000"
                data-aos-anchor-placement="bottom-bottom"
                data-aos-once="false"
              >
                <v-expansion-panels flat class="panel" dark>
                  <v-expansion-panel>
                    <v-expansion-panel-header style="font-size:14pt">PAYPAL</v-expansion-panel-header>
                    <v-expansion-panel-content>
                      <a href="http://paypal.me/facilapuesta" class="link">PAYPAL.ME</a>
                    </v-expansion-panel-content>
                  </v-expansion-panel>
                </v-expansion-panels>
              </v-card-text>
            </v-card>
          </v-col>
          <v-col color="#000033" class="d-flex child-flex" col lg="2" md="4" sm="4">
            <v-card color="#000033" class="text-center" elevation="0">
              <img
                src="@/assets/images/iconos/cm.png"
                width="150"
                data-aos="flip-right"
                data-aos-duration="2000"
                data-aos-once="false"
                data-aos-anchor-placement="bottom-bottom"
              />
              <v-card-text
                class="white--text mayeka forma-pago"
                data-aos="fade-right"
                data-aos-duration="3000"
                data-aos-anchor-placement="bottom-bottom"
                data-aos-once="false"
              >
                <v-expansion-panels flat class="panel" dark>
                  <v-expansion-panel>
                    <v-expansion-panel-header style="font-size:14pt">CRIPTOMONEDAS</v-expansion-panel-header>
                    <v-expansion-panel-content>
                      <v-expansion-panels flat class="panel" dark>
                        <v-expansion-panel>
                          <v-expansion-panel-header style="font-size:14pt">BITCOIN</v-expansion-panel-header>
                          <v-expansion-panel-content>1Khp38HUAaM6BrxVukxnRnCMz5XVEUvc88</v-expansion-panel-content>
                        </v-expansion-panel>
                      </v-expansion-panels>
                    </v-expansion-panel-content>
                  </v-expansion-panel>
                </v-expansion-panels>
              </v-card-text>
            </v-card>
          </v-col>
        </v-row>
      </v-container>
    </v-sheet>
  </div>
</template>

<script>
export default {
  name: "bloqueComoJugar",
};
</script>

<style>
.letters3 {
  display: flex;
  justify-content: center;
  align-items: center;
  text-overflow: ellipsis;
  white-space: nowrap;
  overflow: hidden;
  padding: auto;
}

.letters3 ul {
  position: relative;
  display: flex;
  flex-direction: column;
}

.letters3 ul li {
  list-style: none;
  transition: 0.5s;
}

.letters3 ul li a {
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

.letters3 ul li a:before {
  content: attr(data-text);
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  padding: 0 10px;
  -webkit-text-stroke: 1.5px #000033;
  transform: translateX(0);
  transition: 0.5s;
  pointer-events: none;
}

.letters3 ul li a:hover:before {
  transform: translateX(100%);
  opacity: 0;
}

.letters3 ul li a:after {
  content: attr(data-text);
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  padding: 0 10px;
  color: #000033;
  transform: translateX(-100%);
  transition: 0.5s;
  opacity: 0;
  pointer-events: none;
}

.letters3 ul li a:hover:after {
  transform: translateX(0);
  opacity: 1;
}
.link {
  text-decoration: none;
  color: white !important;
}
.theme--dark.v-expansion-panels .v-expansion-panel {
  background-color: #000033 !important;
  color: white !important;
}

@media (max-width: 1282px) {
  .forma-pago {
    font-size: 13pt !important;
  }
}

@media (max-width: 1263px) {
  .forma-pago {
    font-size: 14pt !important;
  }
}

@media (min-width: 700px) {
  .letters3 ul {
    padding-left: 0px !important;
  }
}
</style>
