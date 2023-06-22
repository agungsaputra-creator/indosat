<template>
  <div class="akses">
    <div class="container px-lg-5 px-3">
      <div class="row">
        <div
          class="col-xl-5 col-lg-6 px-lg-5 py-xl-0 py-3 d-flex flex-column justify-content-xl-center justify-content-start align-items-center"
        >
          <video class="video-akses" controls>
            <source src="movie.mp4" type="video/mp4" />
            <source src="movie.ogg" type="video/ogg" />
            Your browser does not support the video tag.
          </video>
          <div class="d-flex flex-xl-row text-center flex-column mt-xl-5 mt-3 mb-xl-0 mb-3">
            <AtomSubtitle class="fw-bold mb-0 me-2" text="Langsung play tanpa registrasi" />
            <a href="" class="text-decoration-none fw-bold font-primary">im3ooredoo.com/viu</a>
          </div>
        </div>
        <div class="col-xl-7 col-lg-6 pt-5 d-flex justify-content-center align-items-end">
          <img src="../../assets/images/viu_person.webp" alt="icon postpaid" class="img-premium" />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import AtomSubtitle from "../atoms/AtomSubtitle.vue";

export default {
  components: {
    AtomSubtitle,
  },
};
</script>

<style scoped>
.video-akses {
  height: 300px;
  width: 100%;
  border-radius: 16px;
}
@media only screen and (max-width: 992px) {
  .img-premium {
    width: 100%;
  }
}
</style>
