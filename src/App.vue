<template>
<div>
  <app-header></app-header>
  <app-giris></app-giris>
  <app-tanitim></app-tanitim>
  <app-icecekler></app-icecekler>
  <app-yiyecekler></app-yiyecekler>
  <app-footer></app-footer>
</div>
</template>

<script>
  import Header from "./components/Header"
  import Footer from "./components/Footer";
  import Giris from "./components/Giris";
  import Tanitim from "./components/Tanitim";
  import Icecekler from "./components/Icecekler";
  import Yiyecekler from "./components/Yiyecekler";
export default {
components : {
  appHeader : Header,
  appFooter : Footer,
  appGiris : Giris,
  appTanitim : Tanitim,
  appIcecekler : Icecekler,
  appYiyecekler : Yiyecekler,

}

}
</script>

<style>
  ::placeholder{
    color:green!important;
  }
  body{
    font-family: monospace !important;
  }
  h2{
    color:green!important;
    margin:auto;
    border-bottom: 2px solid green;
  }
  h4{
    color:green!important;
  }
  p{
    font-size:16px
  }
  .fade-enter{
      opacity: 0;
  }
  .fade-enter-active{
      transition: opacity .3s;
  }
  .fade-leave{
  }
  .fade-leave-active{
      transition: opacity .3s;
      opacity: 0;
  }
  .container{
    min-height: 100vh;
  }

</style>
