<template>
  <header>
    <div>
      <nav class="navbar navbar-expand-md navbar-dark bg-dark">
        <a class="navbar-brand" href="#">
          <img
            src="../../public/img/SCRUM.png"
            width="40"
            height="30"
            class="d-inline-block align-top"
            alt=""
          />
          Sprint 2
        </a>
        <div
          class="collapse navbar-collapse justify-content-end"
          id="navbarNavAltMarkup"
        >
          <div class="navbar-nav">
            <a class="nav-item nav-link active" href="#"
              >Home <span class="sr-only">(current)</span></a
            >
            <a class="nav-item nav-link" href="#newssection">Noticias</a>
            <a class="nav-item nav-link" href="#">Miebros</a>
            <a class="nav-item nav-link" href="#footersection">Contáctanos</a>
          </div>
        </div>
        <div class="pos-f-t">
          <div class="collapse" id="navbarToggleExternalContent">
            <div>
              <div class="navbar-nav">
                <a class="nav-item nav-link active" href="#"
                  >Home <span class="sr-only">(current)</span></a
                >
                <a class="nav-item nav-link" href="#">Noticias</a>
                <a class="nav-item nav-link" href="#">Miebros</a>
                <a class="nav-item nav-link" href="#">Contáctanos</a>
              </div>
            </div>
          </div>
          <nav class="navbar navbar-dark bg-dark">
            <button
              class="navbar-toggler"
              type="button"
              data-toggle="collapse"
              data-target="#navbarToggleExternalContent"
              aria-controls="navbarToggleExternalContent"
              aria-expanded="false"
              aria-label="Toggle navigation"
            >
              <span class="navbar-toggler-icon"></span>
            </button>
          </nav>
        </div>
      </nav>
    </div>
  </header>
</template>

<script>
export default {
  name: "ModuleHeader",
};
</script>

<style scoped>
</style>