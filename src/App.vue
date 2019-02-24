<template class="everything">
    <div class = "giris">
      <div class="yazi">
        <p class="deli"><span class="deli-upper">DELİ</span> BİLİM &amp; SANAT</p>
                 <a class="button" href="https://www.instagram.com/delifestival/?hl=tr">
                  <h2 class="icon-yazi">Deli Festival</h2>
                  <i class="color-text-flow fab fa-instagram icon"></i>
                </a>
              </div>
            </div>
          </div>
          <div class="first">
            <div class="icons">
              <div class="container">
                <a class="button" href="https://www.instagram.com/deliteknolojicom/">
                  <h2 class="icon-yazi">Deli Teknoloji</h2>
                  <i class="color-text-flow fab fa-instagram icon"></i>
                </a>
              </div>
              <div class="container">
                <a class href="https://www.instagram.com/delifestival/"="button">
                  <h2 class="icon-yazi">Deli Store</h2>
                  <i class="color-text-flow fab fa-instagram icon"></i>
                </a>
              </div>
            </div>
          </div>
          <div class="first">
            <div class="icons">
              <div class="container">
                <a class="button" href="https://www.instagram.com/delikitapcom/d">
                  <h2 class="icon-yazi">Deli Kitap</h2>
                  <i class="color-text-flow fab fa-instagram icon"></i>
                </a>
              </div>
              <div class="container">
                <a href="https://www.instagram.com/firatilhanortaokulu/" class="button">
                  <h2 class="icon-yazi"><span class="insta-okul">Firat Ilhan Ortaokulu</span></h2>
                  <i class="color-text-flow fab fa-instagram icon"></i>
                </a>
              </div>
            </div>
          </div>
        </div>
      </div>-->
      <div class="iletisim" v-show="show_item">
        <div class="allMap">
          <div class="iletisim_ilet" @click="toggle_show()" v-show="show_item">
            <p>İ<br>L<br>E<br>T<br>İ<br>Ş<br>İ<br>M</p>
          </div>
          <transition name="fade">
            <div class="iletisim_iletisim">
              <h3 class="ilet_h3">İletisim:</h3>
              <h3 class="ilet_h3">Tel No: 0(312) 427 72 27</h3>
              <h3 class="ilet_h3">Tahran Caddesi No:24 <br> GOP/ANKARA</h3>
              <h3 class="ilet_h3"><a class="map" href="https://www.google.com/maps/place/Gaziosmanpa%C5%9Fa+Mahallesi,+Tahran+Cd.+No:22,+06700+%C3%87ankaya%2FAnkara/@39.9029511,32.8643831,17z/data=!4m13!1m7!3m6!1s0x14d34fa32dbbf34d:0x8f52889754b69f90!2sGaziosmanpa%C5%9Fa+Mahallesi,+Tahran+Cd.+No:22,+06700+%C3%87ankaya%2FAnkara!3b1!8m2!3d39.902809!4d32.864617!3m4!1s0x14d34fa32dbbf34d:0x8f52889754b69f90!8m2!3d39.902809!4d32.864617"><br>Buraya Tiklayarak <br> Yol Tarifine Ulasabilirsiniz.</a></h3>
            </div>
          </transition>
        </div>
        <!--<div class="acilis">
          <h3> (  Sitemiz 26 Subat Pazartesi Gunu Acilacaktir   )</h3
        </div>-->
      </div>
      <div class="ilet" @click="toggle_show()" v-show="show_ilet">
        <p>İ<br>L<br>E<br>T<br>İ<br>Ş<br>İ<br>M</p>
      </div>
      <div class="All_insta">
        <div class="instaJ">
          <div class="insta button">
                <img class="icon" src="./assets/insta2.svg" @mouseover="show_insta1 = true" @mouseleave="show_insta1 = false">
                <p class="parag" v-show="show_insta1">DELİ Bilim Sanat<br>Instagram Sayfasi Icin Tiklayiniz</p>
          </div>
        </div>
        <div class="instaJ">
          <div class="insta button">
                <p class="parag" v-show="show_insta2">DELİ Festival<br>Instagram Sayfasi Icin Tiklayiniz</p>
                <img class="icon" src="./assets/insta2.svg" @mouseover="show_insta2 = true" @mouseleave="show_insta2 = false">

          </div>
        </div>
        <div class="instaJ">
          <div class="insta button">
                <img class="icon" src="./assets/insta2.svg" @mouseover="show_insta3 = true" @mouseleave="show_insta3 = false">
                <p class="parag" v-show="show_insta3">DELİ Teknoloji<br>Instagram Sayfasi Icin Tiklayiniz</p>
          </div>
        </div>
        <div class="instaJ">
          <div class="insta button">
                <img class="icon" src="./assets/insta2.svg" @mouseover="show_insta4 = true" @mouseleave="show_insta4 = false">
                <p class="parag" v-show="show_insta4">DELİ Store<br>Instagram Sayfasi Icin Tiklayiniz</p>
          </div>
        </div>
        <div class="instaJ">
          <div class="insta button">
                <img class="icon" src="./assets/insta2.svg" @mouseover="show_insta5 = true" @mouseleave="show_insta5 = false">
                <transition name="fade">
                  <p class="parag" v-show="show_insta5">DELİ Kitap<br>Instagram Sayfasi Icin Tiklayiniz</p>
                </transition>
          </div>
        </div>
        <div class="instaJ">
          <div class="insta button">
                <p class="parag" v-show="show_insta6">Firat İlhan Ortaokulu <br>Instagram Sayfasi Icin Tiklayiniz</p>
                <img class="icon" src="./assets/insta2.svg" @mouseover="show_insta6 = true" @mouseleave="show_insta6 = false">

          </div>
        </div>
      </div>
    </div>

</template>

<script>

export default {
    data () {
        return {
          show_item: false,
          show_ilet: true,
          show_parag: false,
          show_insta1: false,
          show_insta2: false,
          show_insta3: false,
          show_insta4: false,
          show_insta5: false,
          show_insta6: false,
        }
    },
    methods:{
      toggle_show() {
        this.show_item = !this.show_item
        this.show_ilet = !this.show_ilet
      },
      show_insta(){
        this.show
      }
    }
}
</script>

<style>
.everything {
  margin-top: -80px;
}

.giris{
  background-image:url(assets/ana.jpg);
  height: 800px;
  background-position: center;
  background-size: cover;
  margin: -40px;
}

h2{
  font-size: 20px;
  color: rgb(242, 185, 12);
  font-family: 'Courgette', cursive;
}

h3{
  margin-left: 400px;
  font-family: 'Courgette', cursive;
  margin-left: -50px;
  text-align: center;
}

.button {
  display: inline-block;
  text-decoration: none;
  border-radius: 30px;
  background: none;
  width: 80px;
  height: 80px;
  text-align: center;
  margin-left: 20px;
  background-color: linear-gradient(to right, red,orange,yellow,green,blue,indigo,violet);
}

.icon {
  align-items:center;
  justify-content:center;
  text-transform:uppercase;
  color: rgb(242, 185, 12);
  float: left;
  margin-left: 40px;
  width: 50px;
  height:50px;
}

.icon-yazi{
  font-size: 20px;
  margin-top: 25px;

}

.ilet{
  position: fixed;
  left: 0;
  background-color: rgb(70, 70, 70);
  margin-top: 80px;
  color: black;
  width: 30px;
  text-align: center;
  background: rgba(14, 247, 65, 0.61);
  border-radius: 10px;
  font-family: 'Open Sans Condensed', sans-serif;
}

.iletisim{
  position: fixed;
  width: 20%;
  left: 0px;
  margin-left: 200px;
  margin-top: 69px;

}

.iletisim_ilet {
  float: left;
  background-color: rgba(4, 88, 23, 0.61);
  color: white;
  width: 30px;
  text-align: center;
  margin-top: 25px;
  height: 10%;
  margin-left: 50px;
  text-align: center;
  border-radius: 10px;
  font-family: 'Open Sans Condensed', sans-serif;
  cursor: pointer;
}

.iletisim_iletisim{
  float: left;
  width: 250px;
  position: fixed;
  left:0;
  border-radius: 10px;
  background: rgba(7, 194, 3, 0.7);
  color: black;
}

.ilet_h3 {
  margin-left: 7px;
}

.first{
  float: left;
}

.container {
  margin-top: 20px;
}

.All_insta {
  margin-top: -40px;
  position: fixed;
  right: 0px;
  margin-right: 10px;
}

.parag {
  color: white;
  margin-top: 3px;
  font-size: 12px;
  margin-left: -150px;
  padding-top: 7px;
  position: fixed;
}

.insta p {
    width: 200px;
    height: 36px;
    background-color: rgba(112, 112, 112, 0.71);
    border: 1px solid rgb(4, 66, 10);
    border-radius: 40px;
    margin-left: -200px;
    font-family: 'Courgette', cursive;
}

.map{
  text-decoration: none;
  display: block;
  color: black;
}
.map:hover{
  color: rgb(60, 60, 60);
}

.deli {
    text-align: center;
    padding-top: 161px;
    font-family: 'Raleway', sans-serif;
    font-size: 40px;
    transform: rotate(-34deg);
    margin-left: -700px;
    color: rgb(2, 46, 6);
}

.deli-upper {
  font-size: 60px;
}

.yazi{
  margin-top: -60px;
}

.insta-okul {
  font-size: 15px;
}

.firat {
    text-align: center;
    font-family: 'Raleway', sans-serif;
    font-size: 30px;
    margin-top: -90px;
    margin-left: 370px;
    transform: rotate(33deg);
    color: rgb(2, 46, 6);}

.fade-enter-active, .fade-leave-active {
  transition: opacity .5s;
}

</style>
