<template>
<div id="carouselExampleAutoplaying" class="carousel slide" data-bs-ride="carousel">
  <div class="carousel-inner">
    <div class="carousel-item active d-flex justify-content-center align-items-center">
      <img src="@/assets/bg.jpg" class="d-block" alt="img1">
    </div>
    <div class="carousel-item d-flex justify-content-center align-items-center">
      <img src="@/assets/imagen1.jpg" class="d-block" alt="img2">
    </div>
    <div class="carousel-item d-flexalign-items-center">
      <img src="@/assets/background.jpg" class="d-block" alt="img3">
    </div>
    </div>
  <button class="carousel-control-prev" type="button" data-bs-target="#carouselExampleAutoplaying" data-bs-slide="prev">
    <span class="carousel-control-prev-icon" aria-hidden="true"> </span>
    <span class="visually-hidden">Previous </span>
    </button>
  <button class="carousel-control-next" type="button" data-bs-target="#carouselExampleAutoplaying" data-bs-slide="next">
    <span class="carousel-control-next-icon" aria-hidden="true"> </span>
    <span class="visually-hidden">Next </span>
  </button>
</div>
</template>

<script>
export default {

}
</script>

<style>
head,body{
    background-color: aquamarine;
}
.d-block{
    height: 20%;
    width: 20%;
    align-items: center;
}
</style>