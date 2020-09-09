<template>
  <div id="bloqueComoJugar">
    <v-card color="black" tile elevation="0" class="py-6">
      <v-card-title class="white--text justify-center mayeka letters">
        <ul>
          <li><a data-text="¿CÓMO JUGAR?" class="mayeka" style="letter-spacing:10px; font-size:20pt">¿CÓMO JUGAR?</a></li>
        </ul>
      </v-card-title>
    </v-card>
    <v-sheet color="#000033" >
      <v-container fluid class="pa-0 ma-0">
        <v-row no-gutters class="justify-center"
          data-aos="fade-down" 
          data-aos-duration="3500"
          data-aos-once="false">
          <v-col class="d-flex child-flex pa-0 ma-0 grid" cols="12" lg="3" md="3" sm="6" xs="12">
            <figure class="effect-marley">
              <v-card flat tile class="d-flex ">
                <img src="@/assets/images/j0.jpg" alt="como jugar 0" height="550" width="100%" />
                <figcaption class="mayeca">
                  <h2>REGISTRATE EN LA <span>WEB</span></h2>
                  <p>Lorem Ipsum es simplemente el ición, como por ejemplo Aldus PageMaker, el cual incluye versiones de Lorem Ipsum.</p>
                  <a href="#redireccion a un lugar">View more</a>
                </figcaption>	
              </v-card>
            </figure>
          </v-col>

          <v-col class="d-flex child-flex pa-0 ma-0 grid" cols="12" lg="3" md="3" sm="6" xs="12">
            <figure class="effect-marley">
              <v-card flat tile class="d-flex ">
                <img src="@/assets/images/j1.jpg" alt="como jugar 1" height="550" width="100%" />
                <figcaption class="mayeca">
                  <h2>CARGA TU <span>SALDO</span></h2>
                  <p>Lorem Ipsum es simplemente el ición, como por ejemplo Aldus PageMaker, el cual incluye versiones de Lorem Ipsum.</p>
                  <a href="#redireccion a un lugar">View more</a>
                </figcaption>	
              </v-card>
            </figure>
          </v-col>

          <v-col class="d-flex child-flex pa-0 ma-0 grid" cols="12" lg="3" md="3" sm="6" xs="12">
            <figure class="effect-marley">
              <v-card flat tile class="d-flex ">
              <img src="@/assets/images/j2.jpg" alt="como jugar 2" height="550" width="100%" />
                <figcaption class="mayeca">
                  <h2>INGRESA Y <span>JUEGA</span></h2>
                  <p>Lorem Ipsum es simplemente el ición, como por ejemplo Aldus PageMaker, el cual incluye versiones de Lorem Ipsum.</p>
                  <a href="#redireccion a un lugar">View more</a>
                </figcaption>	
              </v-card>
            </figure>
          </v-col>

          <v-col class="d-flex child-flex pa-0 ma-0 grid" cols="12" lg="3" md="3" sm="6" xs="12">
            <figure class="effect-marley">
              <v-card flat tile class="d-flex ">
              <img src="@/assets/images/j3.jpg" alt="como jugar 3" height="550" width="100%" />
                <figcaption class="mayeca">
                  <h2>RETIRA TU <span>DINERO</span></h2>
                  <p>Lorem Ipsum es simplemente el ición, como por ejemplo Aldus PageMaker, el cual incluye versiones de Lorem Ipsum.</p>
                  <a href="#redireccion a un lugar">View more</a>
                </figcaption>	
              </v-card>
            </figure>
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

<style >
img {
  width: 500;
}

.letters{
  display: flex;
  justify-content: center;
  align-items: center;
  overflow: hidden;
  padding: auto;
}

.letters ul{
  position: relative;
  display: flex;
  flex-direction: column;
}

.letters ul li{
  list-style: none;
  transition: 0.5s;
}

.letters ul li a{
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

.letters ul li a:before{
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

.letters ul li a:hover:before{
  transform: translateX(100%);
  opacity: 0;
}

.letters ul li a:after{
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

.letters ul li a:hover:after{
  transform: translateX(0);
  opacity: 1;
}

/* Anchor will cover the whole item by default */
/* For some effects it will show as a button */
.grid figure figcaption > a {
	z-index: 1000;
	text-indent: 200%;
	white-space: nowrap;
	font-size: 0;
	opacity: 0;
}

.grid figure h2 {
	font-weight: 300;
  font-size: 20px;
}

.grid figure h2 span {
	font-weight: 800;
}

.grid figure h2,
.grid figure p {
	margin: 0;
}

.grid figure p {
	letter-spacing: 1px;
	font-size: 90%;
}

/***** Marley *****/
/*---------------*/
figure.effect-marley img {
	opacity: 0.9;
	-webkit-transition: opacity 0.35s;
	transition: opacity 0.35s;
}

figure.effect-marley:hover img {
	opacity: 0.8;
}

figure.effect-marley figcaption {
	text-align: right;
}

figure.effect-marley h2,
figure.effect-marley p {
	position: absolute;
  text-align: center;
	right: 30px;
	left: 30px;
  color: white;
	padding: 10px 0;
}


figure.effect-marley p {
	bottom: 10px;
	line-height: 1.5;
	-webkit-transform: translate3d(0,0,0);
	transform: translate3d(0,0,0);
}

figure.effect-marley h2 {
	top: 30px;
	-webkit-transition: -webkit-transform 0.35s;
	transition: transform 0.35s;
	-webkit-transform: translate3d(0,225px,0);
	transform: translate3d(0,225px,0);
}

figure.effect-marley:hover h2 {
	-webkit-transform: translate3d(0,190px,0);
	transform: translate3d(0,190px,0);
}

figure.effect-marley h2::after,
figure.effect-marley p {
	opacity: 0;
	-webkit-transition: opacity 0.35s, -webkit-transform 0.35s;
	transition: opacity 0.35s, transform 0.35s;
}

figure.effect-marley:hover h2::after,
figure.effect-marley:hover p {
	opacity: 1;
	-webkit-transform: translate3d(0,-170px,0);
	transform: translate3d(0,-170px,0);
}

@media (max-width: 1150px) {
  figure.effect-marley:hover h2::after,
  figure.effect-marley:hover p {
    opacity: 1;
    -webkit-transform: translate3d(0,-150px,0);
    transform: translate3d(0,-150px,0);
  }
}

@media (max-width: 1000px) {
  figure.effect-marley:hover h2::after,
  figure.effect-marley:hover p {
    opacity: 1;
    -webkit-transform: translate3d(0,-130px,0);
    transform: translate3d(0,-130px,0);
  }
}

@media (max-width: 950px) {
  figure.effect-marley:hover h2::after,
  figure.effect-marley:hover p {
    opacity: 1;
    -webkit-transform: translate3d(0,-180px,0);
    transform: translate3d(0,-180px,0);
  }
}

@media (max-width: 670px) {
  figure.effect-marley:hover h2::after,
  figure.effect-marley:hover p {
    opacity: 1;
    -webkit-transform: translate3d(0,-170px,0);
    transform: translate3d(0,-170px,0);
  }
}

@media (max-width: 600px) {
  figure.effect-marley:hover h2::after,
  figure.effect-marley:hover p {
    opacity: 1;
    -webkit-transform: translate3d(0,-180px,0);
    transform: translate3d(0,-180px,0);
  }
}
</style>