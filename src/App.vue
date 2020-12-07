<template>
  <div id="app">
    <module-banner></module-banner>
    <div class="container-fluid">
      <module-api></module-api>
    </div>
    <hr />
    <div class="alert alert-dark">
      <h2>Miembros del Equipo</h2>
    </div>
    <hr />
    <div class="container-fluid">
      <div class="row justify-content-center mb-5">
        <div class="col mt-4" v-for="(item, index) of team" :key="index">
          <team-card v-bind:member="item"></team-card>
        </div>
      </div>
    </div>
    <module-footer></module-footer>
  </div>
</template>

<script>
import ModuleBanner from "./components/ModuleBanner.vue";
import ModuleApi from "./components/ModuleApi.vue";
import TeamCard from "./components/TeamCard.vue";
import ModuleFooter from "./components/ModuleFooter.vue";

export default {
  name: "App",
  components: {
    ModuleApi,
    ModuleFooter,
    ModuleBanner,
    TeamCard,
  },
  data() {
    return {
      team: [
        {
          codigo: 1,
          nombre: "Giovany Andres Angel Avila",
          descripcion:
            "Licenciado en Física (incompleto) de la Universidad Pedagógica Nacional, con 35 años de edad. Le gusta practicar natación e interpretar la guitarra.",
          rol: "Desarrollador frontend.",
          imagen: "img/fotoG.jpg",
        },
        {
          codigo: 2,
          nombre: "Juan Sebastian Ariza Gonzalez",
          descripcion:
            "Profesional en Geología de la Universidad Nacional de Colombia, con 26 años de edad. Le gusta hacer equitacion, jugar tenis y ver series.",
          rol: "Desarrollador backend.",
          imagen: "img/fotoJ.jpg",
        },
        {
          codigo: 3,
          nombre: "Liyeira Anaya Amaya",
          descripcion:
            "Profesional en Ingenieria Química de la Universidad de los Andes, con 21 años de edad. Le gusta ver series, resolver juegos matemáticos y escuchar musica.",
          rol: "Arquitecta de software.",
          imagen: "img/fotoL.jpg",
        },
      ],
    };
  },
};
</script>

