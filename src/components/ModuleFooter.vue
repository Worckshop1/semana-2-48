<template>
  <!-- Footer -->
  <footer class="page-footer bg-secondary text-white pt-2" id="footersection">
    <div class="container-fluid text-left">
      <div class="row">
        <div class="col-md-6 mt-md-3 mt-3">
          <h5 class="text-uppercase font-weight-bold">Noticias API</h5>
          <p>
            Portal informativo de noticias de negocios, entretenimiento,
            deportes, tecnología y más a nivel nacional.
          </p>
          <p>
            Enlace al repositorio de GitHub:
            https://github.com/Worckshop1/semana-1-48.git
          </p>
        </div>
        <hr class="clearfix w-100 d-md-none pb-3" />
        <div class="col-md-6 mb-md-0 mb-3">
          <form>
            <div class="row">
              <div class="form-group p-2 flex-fill bd-highlight">
                <label for="FormControlInput1">Nombre</label>
                <input
                  type="text"
                  class="form-control"
                  id="FormControlInput1"
                />
              </div>
              <div class="form-group p-2 flex-fill bd-highlight">
                <label for="FormControlInput1"
                  >Dirección de correo electrónico</label
                >
                <input
                  type="email"
                  class="form-control"
                  id="FormControlInput1"
                />
              </div>
            </div>
            <div class="form-group">
              <label for="FormControlTextarea1">Escribe tu mensaje</label>
              <textarea
                class="form-control"
                id="exampleFormControlTextarea1"
                rows="3"
              ></textarea>
            </div>
            <button type="submit" class="btn btn-primary">Submit</button>
          </form>
        </div>
      </div>
    </div>
    <div class="footer-copyright text-center py-3">© 2020 Copyright</div>
  </footer>
</template>

<script>
export default {
  name: "ModuleFooter",
};
</script>

<style scoped>
div {
  background-color: black;
}
</style>