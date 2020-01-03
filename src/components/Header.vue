<template>
    <nav class="navbar navbar-expand-lg navbar-light  fixed-top">
        <a class="navbar-brand ml-5 font-weight-bold" href="#">Kahvaltı</a>

        <ul class="navbar-nav mx-auto">
            <li class="nav-item">
                <a class="nav-link ml-2" href="#tanitimSection">Hakkımızda</a>
            </li>
            <li class="nav-item">
                <a class="nav-link ml-2" href="#içecekler">Içecekler</a>
            </li>
            <li class="nav-item">
                <a class="nav-link ml-2" href="#menüler">Menüler</a>
            </li>
            <li class="nav-item">
                <a class="nav-link ml-2" href="#iletişim">Iletişim</a>
            </li>
        </ul>
    </nav>
</template>

<script>
    export default {
        name: "Header"
    }
</script>

<style scoped>
    .navbar{
        background-color: rgba(255, 255, 255, 0.88);
        height: 70px;
    }
    .navbar-brand{
        font-size: 30px !important;
        display: flex !important;
        align-items: center !important;
        color: green !important;
    }
    .nav-item a{
        color: green!important;
        font-size: 15px;
    }
    .nav-item a:hover{
        color:black !important;
    }
</style>