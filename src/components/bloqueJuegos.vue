<template>
  <div id="bloqueJuegos" class="my-0">
    <v-sheet color="#000033">
      <v-card color="#000033" elevation="0">
        <v-card-title class="white--text justify-center letters">
          <ul>
            <li><a data-text="JUEGOS" class="mayeka" style="letter-spacing:10px; font-size:20pt">JUEGOS</a></li>
          </ul>
        </v-card-title>

        <v-row>
          <v-col cols="12" xl="8" lg="8" md="8" sm="8" xs="12" class="post" 
        data-aos="fade-down-right" 
        data-aos-duration="2000"
        data-aos-anchor-placement="center-bottom"
        data-aos-once="false">
            <v-img class="imgJuegos" src="@/assets/images/la-granjita.jpg" max-height="300"></v-img>
            <div class="post-s mayeka">
              <h2>Animalitos</h2>
            </div>
          </v-col>
          <v-col cols="12" xl="4" lg="4" md="4" sm="4" xs="12" class="post" data-aos="fade-down-left" 
        data-aos-duration="2000"
        
        data-aos-once="false">
            <v-img class="imgJuegos" src="@/assets/images/juego-4.jpg" max-height="300"></v-img>
            <div class="post-s mayeka">
              <h2>Caballos</h2>
            </div>
          </v-col>
          <v-col cols="12" xl="4" lg="4" md="4" sm="4" xs="12" class="post" data-aos="fade-up-right" 
        data-aos-duration="2000"
        
        data-aos-once="false">
            <v-img class="imgJuegos" src="@/assets/images/juego-3.jpg" max-height="300"></v-img>
            <div class="post-s mayeka">
              <h2>Parley</h2>
            </div>
          </v-col>
          <v-col cols="12" xl="8" lg="8" md="8" sm="8" xs="12" class="post" data-aos="fade-up-left" 
        data-aos-duration="2000"
        
        data-aos-once="false">
            <v-img class="imgJuegos" src="@/assets/images/juego-2.jpg" max-height="300"></v-img>
            <div class="post-s mayeka">
              <h2>Casino</h2>
            </div>
          </v-col>
        </v-row>
      </v-card>
    </v-sheet>
  </div>
</template>

<script>

export default {
  name: "bloqueJuegos",
};
</script>

<style>

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

/* ANIMACION DE LAS IMAGENES */
.post{
  position: relative;
  cursor: pointer;
}

.post:hover .post-s{
  width: 100%;
  height: 100%;
  box-sizing: content-box;
}

.post .imgJuegos{
  display: block;
}

.post-s{
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

.post-s h2{
  color: white;
  font-size: 25px;
  border: 2px solid white;
  padding: 10px 30px;
  box-shadow: -1px 2px 30px 5px rgba(255, 255, 255, 0.35);
}
</style>