<template>
    <main class="home-page">
        <h1 class="home-page-h1">Welcome To Vue js Website</h1>
        <p class="home-page-p">
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Obcaecati in 
        </p>
    </main>
    <!-- <div class="container p-5">
      <h1 class="mb-5">therichpost.com</h1>
      <button type="button" class="btn btn-secondary me-2" data-bs-container="body" data-bs-toggle="popover" data-bs-placement="top" data-bs-content="Top popover">
        Popover on top
      </button>
      <button type="button" class="btn btn-secondary me-2" data-bs-container="body" data-bs-toggle="popover" data-bs-placement="right" data-bs-content="Right popover">
        Popover on right
      </button>
      <button type="button" class="btn btn-secondary me-2" data-bs-container="body" data-bs-toggle="popover" data-bs-placement="bottom" data-bs-content="Bottom popover">
        Popover on bottom
      </button>
      <button type="button" class="btn btn-secondary me-2" data-bs-container="body" data-bs-toggle="popover" data-bs-placement="left" data-bs-content="Left popover">
        Popover on left
      </button>
    </div> -->
</template>
<script>
import { Popover } from 'bootstrap/dist/js/bootstrap.esm.min.js'
export default {
  mounted() {
     //inti Popover
      Array.from(document.querySelectorAll('button[data-bs-toggle="popover"]'))
    .forEach(popoverNode => new Popover(popoverNode))
}
}
</script>
<style lang="scss" scoped>
.home-page-h1{
    text-align: center;
    color:  #0000FF;
}
.home-page-p
{
    color: #3A3B3C;
    font-size: 32px;
    text-align: center;
}
</style>