<template>
  <v-container >
    <Title>
    <template v-slot:title><h1>Experiencia</h1></template>
    </Title>
    <v-row class="mt-3 experience-box">
      <v-col cols="12">
        <v-row v-for="e in experiences"  :key="e.id">
          <v-col cols="4">
            <v-img width="70" height="70" :src="e.srcIcon"></v-img>
          </v-col>
          <v-divider color="white" vertical></v-divider>
          <v-col>
            <h3>{{ e.companyName }}, {{ e.typeContract }}</h3>
            <v-divider color="white" :thickness="2"></v-divider>
            <h4>{{ e.location }}, {{ e.type }}</h4>
            <h5>{{ e.initDate }} - {{ e.endDate }}</h5>
            <p><b>Descipción: </b> {{ e.description }}</p>
          </v-col>
        </v-row>
      </v-col>
    </v-row>
  </v-container>
</template>

<script setup>
import { ref } from "vue";
import experience from "@/data/experience.json";
import Title from '@/components/Home/Title.vue'
const experiences = ref(experience);
</script>

<style lang="css" scoped>
.v-row {
  background-color: rgba(84, 85, 170, 0.6);
  color: rgba(245, 245, 220, 0.9);
  
}

.experience-box{
  box-shadow: 10px 10px 20px rgba(0, 0, 0, 0.55);
}
.v-img{
  margin: auto;
}

.v-col h4{
  font-weight: 300;
}
</style>