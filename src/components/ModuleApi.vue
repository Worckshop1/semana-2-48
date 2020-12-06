<template>
  <div>
        <div class="row mt-md-5 mt-sm-5 mt-xs-5">
      <div
        class="col-lg-6 col-xs-12"
        v-for="(noticia, index) of news"
        :key="index"
      >
        <div class="d-flex justify-content-center align-items-center">
          <div class="p-3">
            <img :src="noticia.urlToImage" alt="Front movie" width="250px" height="200px">
          </div>
          <div class="p-2">
            <h3>{{noticia.title}}</h3>
            <h6>{{noticia.description}}</h6>
          </div>
        </div>
        <div class="d-flex container-fluid justify-content-end pb-2 mt-n2">
          <a :href="noticia.url" target="_blank" class="btn btn-outline-info">Ver noticia completa</a>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import axios from "axios";

export default {
  name: "ModuleApi",
  data() {
    return {
      news: null,
    };
  },
  mounted() {
    axios
      .get("http://newsapi.org/v2/top-headlines?country=co&apiKey=ffd679cf7799424d9203015e479d5b5c")
      .then((response) => {
        this.news = response.data.articles.slice(0,4);
        console.log(this.news);
      });
  },
};
</script>

<style scoped>
  div  {
    background-color: rgb(200, 213, 226);
  }
</style>