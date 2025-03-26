<template>
  <v-container>
    <Title>
      <template v-slot:title><h1>Acerca de mi:</h1></template>
    </Title>

    <div class="content mt-3 mb-1">
      <p class="aboutme">
        Apasionado del desarrollo de aplicaciones, con experiencia en la creación de soluciones eficientes y funcionales utilizando tecnologías modernas. Enfocado en ofrecer experiencias de usuario excepcionales, optimizando el rendimiento y asegurando la calidad en cada proyecto. Comprometido con el aprendizaje continuo y la aplicación de buenas prácticas en el desarrollo.
        Además, cuento con amplio manejo en modelos de inteligencia artificial.
      </p>

      <v-row class="mt-5 mb-auto">
        <v-col lg="6" sm="6" md="6" xs="12">
          <v-sheet>
            <h3 class="text-center">Nacionalidad</h3>
            <v-img
              :width="100"
              cover
              src="images/chile-logo.png"
            ></v-img>
            <h4 class="text-center">Chileno</h4>
          </v-sheet>
        </v-col>
        <v-col lg="6" sm="6" md="6" xs="12">
          <v-sheet>
            <h3 class="text-center">Localidad</h3>
            <v-img
              :width="100"
              :height="100"
              cover
              src="images/location-logo.png"
            ></v-img>
            <h4 class="text-center">Séptima Región</h4>
          </v-sheet>
        </v-col>
      </v-row>
    </div>
  </v-container>
</template>

<script setup>
import Title from '@/components/Home/Title.vue'
</script>

<style lang="css" scoped>
.content {
  text-align: justify;
  background-color: rgba(84, 85, 170, 0.4);
  margin-right: 10%;
  margin-left: 10%;
  border-radius: 10px;
  padding: 30px 30px 30px 30px;
  box-shadow: 10px 10px 20px rgba(0, 0, 0, 0.55);
}

.aboutme {
  color: #f5f5dc;
  font-size: 20px;
}

.v-sheet{
  background-color: transparent !important;
  color: #f5f5dc;
}
.v-sheet h3{
  background-color: rgba(155, 128, 205, 0.4);
  margin-bottom: 10px;
  border-radius: 10px;
}

.v-img{
  margin: auto;    
}



@media (max-width: 1000px) {
  .content {
    margin-right: auto;
    margin-left: auto;
  }
  .aboutme {
    font-size: 15px;
  }
}
</style>