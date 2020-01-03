<template>
    <header id="headerSection">
        <img :src="img" class="img-fluid" alt="">
        <div class="col-md-6 ml-5 headerFormDiv ">
            <form  class="form-inline  my-2 my-sm-0">
                <input class="form-control form-control-lg  mr-sm-0 forminput" type="search" placeholder="ne yemek istersin?" aria-label="Search">
                <button class="btn formbtn btn-lg my-2 my-sm-0" type="submit"><i class="fa fa-search"></i></button>
            </form>
        </div>
    </header>
</template>

<script>
    export default {
        name: "Giris",
        data(){
            return{
                img : "/src/images/kapak.jpg"
            }
        }
    }
</script>

<style scoped>

    #headerSection{
        background-size: cover;
        height: 100vh;
        display: flex;
        align-items: center;
    }
    .headerFormDiv{
        position: relative;
        margin-top: 200px;
    }
    .forminput{
        width: 360px !important;
        border-radius:.3rem 0 0 .3rem !important;
    }
    .formbtn{
        border-radius:0 .3rem .3rem 0 !important;
        background-color: green;
        color:white!important;
    }
    img{
        position: absolute;
        width: 100%;
        height: 100%;
    }
</style>