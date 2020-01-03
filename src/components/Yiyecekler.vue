<template>
    <section class="pt-5 pb-5" id="menüler">
        <div class="container mt-3">
            <div class="row"><h2>Menüler</h2></div>

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
                    {name:"Zeytinli Simit",     price : 9.99,  img : "/src/images/yemek1.jpg"},
                    {name:"Meyve Karışımı",     price : 12.99,  img : "/src/images/yemek2.jpg"},
                    {name:"Yumurta ve Avokado",     price : 9.99,  img : "/src/images/yemek3.jpg"},
                    {name:"Salam ve Yumurta",     price : 14.99,  img : "/src/images/yemek4.jpg"},
                    {name:"Bol Sebzeli Yumurta",     price : 7.99,  img : "/src/images/yemek5.jpg"},
                    {name:"Meyveli Yulaf",     price : 9.99,  img : "/src/images/yemek6.jpg"},
                    {name:"Çikolatalı Kek",     price : 8.99,  img : "/src/images/yemek7.jpg"},
                    {name:"Meyve Karışımı",     price : 7.99 ,  img : "/src/images/yemek8.jpg"},
                    {name:"Salam ve Yumurta",     price : 14.99,  img : "/src/images/yemek9.jpg"},
                    {name:"Meyve Karışımı",     price : 7.99,  img : "/src/images/yemek10.jpg"},
                    {name:"Meyve Karışımı",     price : 19.99 ,  img : "/src/images/yemek11.jpg"},
                    {name:"Meyveli Yoğurt",     price : 9.99 ,  img : "/src/images/yemek12.jpg"},
                    {name:"Patatesli Yumurta",     price : 6.99,  img : "/src/images/yemek13.jpg"},
                    {name:"Meyve Karışımı",     price : 7.99,  img : "/src/images/yemek14.jpg"},
                    {name:"Meyveli Omlet",     price : 13.99,  img : "/src/images/yemek15.jpg"}
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

</style>