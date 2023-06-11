<template>
  <v-container>
    <div class="title mt-4">
      <h1>Acerca de mi:</h1>
    </div>

    <div class="content mt-3">
      <p class="aboutme">
        ¡Hola!, soy Ingeniero en Informática apasionado por la programación y el
        desarrollo de software tanto FrontEnd como BackEnd. Estoy dispuesto a
        tomar retos desafiantes para utilizar todas mis capacidades como
        desarrollador y lograr objetivos. Además, siempre estoy motivado a
        aprender cosas nuevas que me aporten a mi crecimiento profesional.
      </p>
    </div>
  </v-container>
</template>

<script>
export default {};
</script>

<style lang="css" scoped>
.title {
  text-align: center;
  background-color: rgba(84, 85, 170, 0.4);
  margin-right: 40%;
  margin-left: 40%;
  color: #f5f5dc;
  border-radius: 5%;
}

.content {
  text-align: justify;
  background-color: rgba(84, 85, 170, 0.4);
  margin-right: 20%;
  margin-left: 20%;
  border-radius: 10px;
  padding: 10px 10px 10px 10px;
}

.aboutme {
  color: #f5f5dc;
  font-size: 20px;
}

@media (max-width: 1000px) {
  .title {
    margin-right: auto;
    margin-left: auto;
  }
  .content {
    margin-right: auto;
    margin-left: auto;
  }
  .aboutme {
    font-size: 15px;
  }
}
</style>