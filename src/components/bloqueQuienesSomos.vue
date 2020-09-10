<template>
  <div id="bloqueQuienesSomos">
    <v-sheet color="white">
      <v-container fluid class="pa-0 ma-0">
        <v-row no-gutters style="overflow-x: hidden">
          <v-col class="d-flex child-flex" cols="12" sm="6">
            <v-card class="text-center mayeka" elevation="0">
              <div  class="center">
                <h1 style="letter-spacing:10px; color:#000033; "  class="whoTitle"
                    data-aos="fade-down-right"
                    data-aos-duration="2000"
                    data-aos-once="false"
                    data-aos-easing="linear"
                    data-aos-anchor-placement="bottom-bottom">¿QUIÉNES SOMOS?</h1>

                <p class="pt-lg-12 pt-md-6 pt-sm-4 px-12 whoText" 
                    data-aos="fade-up-left"
                    data-aos-duration="2000"
                    data-aos-once="false"
                    data-aos-easing="linear"
                    data-aos-anchor-placement="bottom-bottom">Lorem ipsum dolor sit amet
                    consectetur adipisicing elit. A, iste reprehenderit. Autem officia consequatur 
                    vel deleniti necessitatibus quas iusto! Consequuntur veniam dolor facilis est nulla,
                     dignissimos at in dolores ex.</p>
              </div>
            </v-card>
          </v-col>
          <v-col class="d-flex child-flex pa-0 ma-0"  cols="12" sm="6">
            <v-card elevation="0" tile>
              <img class="img-fluid whoImage" src="@/assets/images/qs.png" />
            </v-card>
          </v-col>


          <v-col class="d-flex child-flex pa-0 ma-0"  cols="12" sm="6">
            <v-card elevation="0" tile>
              <img class="img-fluid whoImage" src="@/assets/images/qs2.png" />
            </v-card>
          </v-col>

          <v-col class="d-flex child-flex" cols="12" sm="6">
            <v-card class="text-center mayeka" elevation="0">
              <div  class="center">

                <p class="py-6 px-12 whoText" 
                    data-aos="fade-up-right"
                    data-aos-duration="2000"
                    data-aos-once="false"
                    data-aos-easing="linear"
                    data-aos-anchor-placement="bottom-bottom">Lorem ipsum dolor sit amet
                    consectetur adipisicing elit. A, iste reprehenderit. Autem officia consequatur 
                    vel deleniti necessitatibus quas iusto! Consequuntur veniam dolor facilis est nulla,
                     dignissimos at in dolores ex.</p>
              </div>
            </v-card>
          </v-col>


        </v-row>
      </v-container>
    </v-sheet>
  </div>
</template>

<script>
export default {
  name: "bloqueQuienesSomos",
};
</script>

<style>
.center{
    width:100%;
    height:100%;
    box-sizing:content-box;
    position:absolute;
    text-align: center;
    top:0;
    display:flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
}

@media (max-width: 960px) {
  .whoTitle {
    font-size: 20px !important;
  }

  .whoText {
    font-size: 15px !important;
  }

  .center{
      width:100%;
      height:100%;
      box-sizing:content-box;
      position:absolute;
      text-align: center;
      top:0;
      display:flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
  }
}

@media (max-width: 800px) {
  .whoTitle {
    font-size: 15px !important;
  }

  .whoText {
    font-size: 10px !important;
  }
  
  .center{
      width:100%;
      height:100%;
      box-sizing:content-box;
      position:absolute;
      text-align: center;
      top:0;
      display:flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
  }
}

@media (max-width: 600px) {
  .whoTitle {
    font-size: 25px !important;
  }

  .whoText {
    font-size: 20px !important;
  }

  .center{
    width:100%;
    height:100%;
    box-sizing:content-box;
    position:static;
    padding: 10px 0px;
    text-align: center;
  }

  .whoImage{
    background: black;
  }
}
</style>