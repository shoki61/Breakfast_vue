<template>
    <section class="pt-5 pb-5" id="içecekler">
        <div class="container mt-3" >
            <div class="row text-center"><h2>Içecekler</h2></div>
            <div class="row p-1">

                <div class="col-md-3 p-2" v-for="list in lists">
                    <div class="imgContainer">
                        <img :src="list.img" class="img-fluid">
                        <div class="imgOverlay">
                            <div class="imgText">
                                <h4>{{list.name}}</h4>
                                <p>{{list.price}}₺</p>
                            </div>
                        </div>
                    </div>
                </div>

            </div>

        </div>
    </section>
</template>

<script>
    export default {
        data(){
            return{
                lists : [
                    {name:"Filtre Kahve",     price : 7.99,  img : "/src/images/içecek1.jpg"},
                    {name:"Kapuçino",         price : 3.99,  img : "/src/images/içecek2.jpg"},
                    {name:"Sıcak Çikolata",   price : 4.99,  img : "/src/images/içecek3.jpg"},
                    {name:"Çay",              price : 1.99,  img : "/src/images/içecek4.jpg"},
                    {name:"Esspreso",         price : 6.49,  img : "/src/images/içecek5.jpg"},
                    {name:"Yeşil Çay",        price : 1.49,  img : "/src/images/içecek6.jpg"},
                    {name:"Türk Kahvesi",     price : 4.99,  img : "/src/images/içecek7.jpg"},
                    {name:"Mayve Çayı",       price : 2.49,  img : "/src/images/içecek8.jpg"},
                    {name:"Sıcak Çikolata",   price : 3.99,  img : "/src/images/içecek9.jpg"},
                    {name:"Portakal",         price : 3.49,  img : "/src/images/içecek10.jpg"},
                    {name:"Limonlu Yeşi Çay", price : 1.99,  img : "/src/images/içecek11.jpg"},
                    {name:"Latte",            price : 3.49,  img : "/src/images/içecek12.jpg"}
                ]
            }
        }
    }
</script>

<style scoped>
    .imgContainer{
        cursor: pointer;
    }

    .imgOverlay{
        position: absolute;
        top: 0;
        left: 0;
        bottom: 0;
        right: 0;
        width: 100%;
        height: 100%;
        background-color: rgba(255, 255, 255, 0.85);
        opacity: 0;
        transition: .5s ease;
    }
    .imgContainer:hover .imgOverlay{
        opacity: .8;
    }
    .imgText{
        color:green;
        position: absolute;
        top:50%;
        left: 50%;
        transform: translate(-50%,-50%);
        text-align: center;
    }
    .imgText p{
        font-size: 20px;
    }
</style>.