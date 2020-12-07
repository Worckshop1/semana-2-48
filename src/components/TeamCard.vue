<template>
    <div class="card text-white bg-info border-light">
    <div class="d-flex justify-content-center p-2">
      <div>
        <img :src="member.imagen" class="img-fluid rounded" alt="foto" >
      </div>
    </div>

    <div class="card-body">
      <h3 class="card-title">{{ member.nombre }}</h3>
      <p class="card-text"><span>Descripción: </span>{{ member.descripcion }}</p>
      <p class="card-text"><span>Rol: </span>{{ member.rol }}</p>
      <p class="card-text"><span>Código: </span>{{ member.codigo }}</p>
    </div>

    <div class="card-footer">
      <small class="text-white">Last updated 3 mins ago</small>
    </div>
  </div>
</template>

<script>
    export default {
        name: "TeamCard",
        props: ['member']
    }
</script>

<style scoped>

</style>
