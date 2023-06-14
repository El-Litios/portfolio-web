<template>
  <v-container>
    <div class="title mt-4">
      <h1>Proyectos:</h1>
    </div>

    <v-row class="mt-3">
      <v-col lg="4" sm="4" md="4" xs="12" v-for="p in projects" :key="p.id">
        <v-card class="mx-auto" max-width="400">
          <v-img class="align-end" height="200" :src="p.photo" cover> </v-img>

          <v-card-subtitle class="pt-4">{{ p.name }}</v-card-subtitle>

          <v-card-text>
            {{ p.description }}

            <v-row class="icons mt-1" no-gutters>
              <v-col
                class="mr-1"
                lg="4"
                sm="4"
                md="4"
                xs="12"
                v-for="i in p.icons"
                :key="i.id"
              >
                <v-img :src="i.src" height="25" :title="i.name"></v-img>
              </v-col>
            </v-row>
          </v-card-text>

          <v-card-actions>
            <v-row class="text-center">
                <v-col cols="6">
                    <v-btn> Ir <v-icon end icon="mdi-open-in-new"></v-icon></v-btn>
                </v-col>
                <v-col cols="6">
                    <v-btn> GitHub <v-icon end icon="mdi-github"></v-icon></v-btn>
                </v-col>
            </v-row>
            
          </v-card-actions>
        </v-card>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
import { ref } from "vue";
import project from "@/data/projects.json";
export default {
  setup() {
    const projects = ref(project);

    return { projects };
  },
};
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

.icons {
  width: 80px;
}

.icons .v-img {
  background-color: rgba(155, 128, 205, 0.4);
  border-radius: 100%;
}

.v-card {
  background-color: rgba(84, 85, 170, 0.4);
  color: #f5f5dc;
}

.v-card-subtitle {
  font-size: 20px;
}

.v-card-text {
  font-size: 15px;
}

.v-card-actions .v-row .v-col{
    background-color: rgba(127, 93, 185, 0.7);
}
.v-card-actions .v-row .v-col:hover{
    background-color: rgba(127, 93, 185, 0.3);
}

@media (max-width: 1000px) {
  .title {
    margin-right: auto;
    margin-left: auto;
  }
}
</style>