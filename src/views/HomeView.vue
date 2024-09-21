<template>
  <v-app id="home">
  <NavBar/>
  <v-container fluid>
    <div class="head">
    <v-row>
      <v-col cols="5">
        <div style="position: relative;" class="mt-16">
        <h1 class="text-green">Holys</h1>
        <h1 class="text-green">Soy Miguel Ángel</h1>
        <span class="text-green">Soy profesionista y ejerzo en la DPPNNAF</span><br>
        <v-btn tile dark class="text-red" variant="outlined">Contactame</v-btn>
      </div>
      </v-col>
      <v-col cols="2">
        <div style="position: absolute;z-index: 9999;bottom:0;margin-left:auto; margin-right: auto;left: 0;right:0;text-align:center">
          <v-icon>fas fa-single-double-down</v-icon>
        </div>
      </v-col>
      <v-col cols="5">
        <div style="position: absolute; z-index: 9999;" class="mt-16"></div>
        <v-img src="../assets/MiguelAngelKD.jpeg" contain max-height="300"></v-img>
      </v-col>
    </v-row>
  </div>
  <v-col cols="12" class="mt-16" id="about">
    <div>
      <v-row>
        <v-col cols="12" sm="6">
          <div class="egg">
            <v-img src="../assets/buhoyo.png" max-height="300"></v-img>
          </div>
        </v-col>
        <v-col cols="12" sm="6">
          <h2 class="mt-16">About Me</h2>
          <div style="width: 120px">
            <v-slider v-model="slider2" color="black" label="">
            </v-slider>
          </div>
          <h4 class="mt-n4">Tengo 18 años dando asesorias jurídicas y salvaguardando la protección, y la integridad física y emocional de los NNA: profesión</h4>
          <h4> Así mismo dando asesorías a las familias que tienen controversias familiares.</h4>
          <p class="text-gray"> De igual manera he llevado juicios familiares y en materia penal.</p>
          <br>
          <p class="text-gray">También tengo conocimiento sobre otras materias en Derecho; como laborales, sindicatos, empresarial entre otros.</p>
          <v-btn titl dark color="green" class="mt-4">
            Descargar CV
          </v-btn>
        </v-col>
      </v-row>
    </div>
  </v-col>
  <div class="text-center mt-4">
    <h1>Lo que hago.</h1>
    <div style="width: 120px; margin: 0 auto">
      <v-slider v-model="slider2" color="black" label=""></v-slider>
    </div>
  </div>
  <v-col cols="12" class="padd" id="portfolio">
    <div class="first" id="project">
      <v-row>
        <v-col cols="12">
          <div class="child">
            <v-btn icon="fas fa-laptop" color="green" class="text-white"></v-btn>
            <h3 class="ml-3 mt-4">Ley de NNA</h3>
            <p class="text-grey ml-3 mt-4 text-caption"></p>
            Dentro de la ley de los NNA menciona <br> todos sus derechos, así como la <br>
            protección integral ante la violencia familiar <br> o de algún delito de indole sexual, 
          </div>
          <div class="child">
            <v-btn icon="fas fa-laptop" color="green" class="text-white"></v-btn>
            <h3 class="ml-3 mt-4">Código Penal</h3>
            <p class="text-grey ml-3 mt-4 text-caption"></p>
            Cualquier delito cometido en contra de las <br> personas, es importante denunciar<br>
            o acudir ante la Fiscalía General del Estado
          </div>
          <div class="child">
            <v-btn icon="fas fa-laptop" color="green" class="text-white"></v-btn>
            <h3 class="ml-3 mt-4">Código Civil</h3>
            <p class="text-grey ml-3 mt-4 text-caption"></p>
            En esta código nos señala los derechos que tienen<br> la familia para demandar controversias como<br>
            divorcios, guarda y custodia, alimentos de los hijos.
          </div>
        </v-col>
      </v-row>
      <v-divider></v-divider>
    </div>
  </v-col>
  <v-col cols="12" sm="12" id="services">
    <div class="d-flex justify-center mb-6">
      <v-btn color="green" class="mr-2">Materias</v-btn>
      <v-btn class="mr-2" variant="tonal">Ley de NNA</v-btn>
      <v-btn class="mr-2" variant="tonal">Código Civil</v-btn>
      <v-btn class="mr-2" variant="tonal">Código Penal</v-btn>
      <v-btn class="mr-2" variant="tonal">Sindicatos</v-btn>
      <v-btn class="mr-2" variant="tonal">Personas Jurídicas</v-btn>
  </div>
    </v-col>
    <v-col cols="12" class="imgHover">
      <v-row class="fill-height" align:="center" justify="center">
          <v-col cols="12" md="4" v-for="(items, i) in items" :key="i">
            <v-hover v-slot="{isHovering, props}">
              <v-card :elevation="isHovering ? 12: 2" :class="{'on-hover' : isHovering}" v-bind="props">
                <v-img :src="item" height="255px" cover></v-img>
              </v-card>
              </v-hover>
          </v-col>
      </v-row>
    </v-col>
    <v-col cols="12" sm="12">
      <div class="d-flex justify-center mb-6">
      <v-btn color="green" class="mt-4">Conocer más</v-btn>
    </div>
    </v-col>
    <v-col cols="12" id="page">
      <div class="pre">
        <v-row>
          <v-card class="mw-auto" max-width="344" height="">
            <v-img src="..//assets/buhoyo.png" height="100px" cover></v-img>
            <v-card-title>Angelín</v-card-title></v-card>
            <v-card-subtitle>Angelín es el Sr. sabio</v-card-subtitle>
            <v-card-text>El búho es un símbolo importante en Derecho. Representa la sabiduría y la comprensión de la ley. Significa que los abogados tienen que estar versados en el conocimiento de la ley y que tienen que ser capaces de aplicarla con inteligencia y justicia.
          </v-card-text>
        </v-row>
      </div>
    </v-col>
    <v-col cols="12" id="biog">
      <div class="hire">
        <v-row>
          <v-col cols="12" sm="8">
            <h1 Contratame para tus proyectos></h1>
            <p>Los servicios de un abogado es importante, cuando las personas se encuentran en alguna controversia o se han equivocado al estar involucrados en algún delito</p>
          </v-col>
          <v-col cols="12" sm="4">
            <v-btn color="green" class="mt-15"> Contratame</v-btn>
          </v-col>
          </v-row>
          </div>
    </v-col>
    <v-col cols="12" sm="12" class="px-16" id="contact">
      <v-row>
        <v-col cols="12" sm="4">
          <div class="child">
          <h1>Información de contacto</h1>
          <v-btn icon="fas fa-map-marker-alt" class="mt-10" variant=”outlined”></v-btn><br />
          <span class="text-caption">Mi dirección; Dirección: 5a Av. entre calles 2 y 4, Col. Centro</span><br />
	<v-btn icon=fas fa-phone-alt” class=”mt-10” variant=”outlined”></v-btn><br />
	<span class=”text-caption”>984 136 1384</span><br />
	<span class=”text-caption”>984 136 1384</span><br />
       	<v-btn icon=fas fa-envelope” class=”mt-10” variant=”outlined”></v-btn><br />
	<span class=”text-caption”>milicangelkuyoc@gmail.com </span><br />
	<span class=”text-caption”>milicangelkuyoc@gmail.com </span><br />
          </div>
        </v-col>
    <v-col cols="12" sm="8">
      <h1 class="mt-8">Send your message!!!</h1>
      <divider></divider>
      <span class="text-caption">Lorem</span>
      <v-row class="mt-10">
        <v-col cols="12" sm="6">
          <v-text-field label="Nombre" persistent-hint variant=”outlined”></v-text-field>
        </v-col>
        <v-col cols="12" sm="6">
          <v-text-field label="Apellidos" persistent-hint variant=”outlined”></v-text-field>
        </v-col>
        <v-col cols="12" sm="6">
          <v-text-field label="Teléfono" persistent-hint variant=”outlined”></v-text-field>
        </v-col>
        <v-col cols="12" sm="6">
          <v-text-field label="Email" persistent-hint variant=”outlined”></v-text-field>
        </v-col>
    </v-row>
        <v-textarea label="Mensaje" persistent-hint variant=”outlineded”></v-textarea>
    <v-btn color="green" class="mt-2">Submit Now</v-btn>
            </v-col>
            </v-row>
          </v-col>
        </v-container>
     </v-app>
</template>
<script>
import { defineComponent } from 'vue';

import NavBar from '../components/NavBar.vue';

export default defineComponent({
  name: 'HomeView',
  setup () {
    return {
      slider2: 50,
      items : [
        { img: "MiguelAngelKD.jpeg"},
        { img: "buhoyo.png"},
      ]
    }
  },

  components: {
    NavBar,
  },
});
</script>

<style scoped>
.v-container {
  padding-top: 16px;
}
.head {
  position: relative;
  text-align: center;
  padding: 12px;
  margin-bottom: 6px;
  height: 400px;
  width: 100;
  color: white;
} 
.head:before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  height: 100%;
  width: 50%;
  background: rgb(0, 0, 0);
  transform: skew(0deg, 6deg);
}
.head:after {
  content: '';
  position: absolute;
  top: 0;
  right: 0;
  height: 100%;
  width: 50%;
  background: rgb(0, 0, 0);
  transform: skew(0deg, -6deg);
}
.egg {
  display: block;
  margin-left: 100px;
  margin-top: 50px;
  width: 365px;
  height: 300px;
  background-color: green;
  border-radius: 50% 50% 50% 50% / 60% 60% 40% 0%;
}
.first{
  width: 100%;
  height: 280px;
  text-align: center;
  padding: 2rem 2rem;
}
.child{
display: inline-block;
padding: 2rem 1rem;
vertical-align: middle;
text-align: center;
margin-right: 8px;
}
.imgHover{
padding: 0 200px;
}
.pre{
  width: 100%;
  height: 280px;
  text-align: center;
  padding: 0 200px;
  background-color: aliceblue;
}
.hire{
  width: 100%;
  height: 200px;
  padding: 0 200px;
  background-color: #c9c9c9;
  margin-top: -24px;
}

</style>
