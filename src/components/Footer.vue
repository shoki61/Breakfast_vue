<template>
    <section id="iletişim" class="pt-5 pb-1">
        <div class="container-fluid">
            <div class="row">
                <div class="col-lg-6">
                    <h2>Bizimle iletişime geçin</h2>
                    <h4>Adres</h4>
                    <p>Trabzon</p>
                    <h4>E-mail</h4>
                    <p>Kahvaltı@gmail.com</p>
                    <h4>Telefon</h4>
                    <p>0151 264 2500</p>
                    <div class="d-flex flex-row link-div">
                        <div class="p-2">
                            <a href="#"><i class="fa fa-facebook fa-2x"></i></a>
                        </div>
                        <div class="p-2">
                            <a href="#" ><i class="fa fa-twitter fa-2x"></i></a>
                        </div>
                        <div class="p-2">
                            <a href="#" ><i class="fa fa-instagram fa-2x"></i></a>
                        </div>
                        <div class="p-2">
                            <a href="#" ><i class="fa fa-youtube fa-2x"></i></a>
                        </div>
                    </div>
                </div>

                <div class="col-lg-6">
                    <form>
                        <div class="form-group">
                            <div class="input-group input-group-lg">
                                <div class="input-group-prepend">
                              <span class="input-group-text">
                                 <i class="fa fa-user" style="color:white"></i>
                              </span>
                                </div>
                                <input class="form-control" type="text" placeholder="Ad">
                            </div>
                        </div>

                        <div class="form-group">
                            <div class="input-group input-group-lg">
                                <div class="input-group-prepend">
                              <span class="input-group-text">
                                 <i class="fa fa-envelope" style="color:white;" ></i>
                              </span>
                                </div>
                                <input class="form-control" type="text" placeholder="E-mail">
                            </div>
                        </div>

                        <div class="form-group">
                            <div class="input-group input-group-lg">
                                <div class="input-group-prepend">
                              <span class="input-group-text">
                                 <i class="fa fa-pencil" style="color:white;"></i>
                              </span>
                                </div>
                                <textarea class="form-control" rows="5" placeholder="Mesaj"></textarea>
                            </div>
                        </div>

                        <input type="submit" value="Gönder" class="btn  btn-block" >

                    </form>
                </div>
            </div>
            <p style="font-family: sans-serif;color:#606060;margin-top: 45px" align="center">
                Sohrat Jumadurdyyew ©2019
                <a href="https://github.com/shoki61/Breakfast_vue.git" target="_blank">
                    <i class="fa fa-github ml-4" style="color:#606060;font-size: 20px"></i>
                </a>
            </p>
        </div>

    </section>
</template>

<script>
    export default {
    }
</script>

<style scoped>
    span{
        background-color: green!important;
        width: 52px;
    }
    .btn-block{
        border:1px solid green!important;
        color:green;
    }
    .btn-block:hover{
        background-color: green;
        color:white;
    }
    #iletişim{
        background-color: #efefef;
    }
    #iletişim i{
        color:green;
    }
    .fa-github:hover{
        color: #8f8f8f!important;
        border-bottom : #8f8f8f 1px solid;
    }
</style>