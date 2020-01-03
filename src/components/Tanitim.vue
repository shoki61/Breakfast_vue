<template>
    <section class="container pt-5" id="tanitimSection">
        <div class="row mt-5">
            <div class="col-lg-6 mb-4">
                <img :src="img" class="img-fluid">
            </div>
            <div class="col-lg-6" id="hakkimizda">
                <h3 class="mb-3">{{title}}</h3>
                <p class="mt-5">{{description}}</p>
                <button class="btn"><b>daha fazla bilgi...</b></button>
            </div>
        </div>
    </section>
</template>

<script>
    export default {
        data(){
            return{
                title : "Restaurantımız",
                img : "/src/images/tanitim.jpg",
                description : "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Mauris metus ante, auctor eget dui quis, ullamcorper tincidunt massa. Vestibulum vestibulum mauris dui, quis imperdiet dolor gravida eleifend. Mauris a gravida ex, et accumsan mi. Duis tincidunt diam pellentesque ligula porttitor, et lacinia odio molestie. Duis justo urna, facilisis in rutrum ut, auctor ut libero. Nam congue nunc vel tempus rhoncus. Sed ultrices urna eget orci tristique imperdiet. Aenean eleifend mauris purus, fermentum placerat velit porttitor at."

            }
        }
    }
</script>

<style scoped>
    #hakkimizda h3{
        padding-left: 20px;
        border-left: 5px solid green;
        color: green;
    }
    #hakkimizda p {
        line-height: 20px;
        font-size: 15px;
        color: #5a5a5a;
    }
    #hakkimizda .btn{
        border: none;
        background-color: transparent;
        color: green
    }
    #hakkimizda .btn:hover {
        background-color: transparent;
        color: black;
    }
</style>