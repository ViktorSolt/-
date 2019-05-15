<template lang="html">
  <header>

    <div class="container">
     <div class="headerbar">
       <div class="logo">
         <img class="tiny" src="./../assets/fingerprint@3x.png" alt="">
         <h1>tinyone</h1>
         <div class="active">
           <nuxt-link to="#">Features</nuxt-link>
           <nuxt-link to="#">Support</nuxt-link>
           <nuxt-link to="#">Blog</nuxt-link>
         </div>
       </div>
       <div class="headerbar_links">
         <nuxt-link to="#">Features</nuxt-link>
         <nuxt-link to="#">Support</nuxt-link>
         <nuxt-link to="#">Blog</nuxt-link>
         <img class="bar" onclick="show(event)" src="./../assets/Menu@New.png" alt="">
        <img class="hidebar" onclick="hide(event)"   src="./../assets/Symbol 302 – 1.svg" alt="">
       </div>
     </div>
    <div class="notmain">
      <div class="main_text">
        <h1>Inspire your inspiration</h1>
        <h3>Simple to use for your app, products<br>
        showcase and your inspiration</h3>
        <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit.<br>
        Praesent vitae eros eget tellus tristique bibendum. Donec<br>
        rutrum sed sem quis venenatis. Proin viverra risus a eros<br>
        volutpat tempor. In quis arcu et eros porta lobortis sit </p>
      <div class="images">
        <img src="./../assets/icon-fa-apple.png" alt="">
        <img src="./../assets/icon-fa-android.png" alt="">
        <img src="./../assets/icon-fa-windows.png" alt="">
      </div>
    </div>
    <div class="phone">
     <img src="./../assets/fingerprint@y3x.png" alt="">
     <h3>tinyone</h3>
    </div>
    </div>
  </div>
   <div class="but">
     <button type="button" name="button"></button>
     <button type="button" name="button"></button>
     <button type="button" name="button"></button>
   </div>

 </header>
</template>

<script>
export default {
}
</script>

<style lang="sass" scoped>
@import '../assets/variables'
header
  background: $sunflower-yellow
  font-family: PTSans
  word-spacing: 0.01em
.container
.headerbar
  display: flex
  width: 100%
  padding-top: 3%
  justify-content: space-around
.tiny
  margin-right: $logo_right
  height: 43px
  margin-bottom: $logo_bottom
.bar,
.hidebar
  display: none
.logo
  display: flex
  width: 39%
  margin-left: 14%
.active
  position: absolute
  top: 70px
  margin-left: -55%
  display: flex
  flex-direction: column
  transition: ease 2s
.active a
  text-decoration: none
  font-size: 20px
  font-weight: bold
  color: $black
  border-bottom: 1px solid black
  margin-bottom: 2%
.logo h1
  margin-top: 1%
.headerbar_links
  display: flex
  width: 40%
.headerbar_links a
  margin-top: 1%
  margin-right: 10%
  text-decoration: none
  font-size: 20px
  font-weight: bold
  color: $black
.main_text
  display: flex
  flex-direction: column
  justify-content: space-around
  margin-top: 6%
  margin-bottom: 9%
  margin-left: 14%
  width: 39%
  transition: ease 2s
.main_text h1
  display: flex
  font-size: 24px
  color: $black
.main_text h3
  font-size: 17px
  color: $charcoal-grey
  font-weight: 200
.main_text p
  font-size: 13px
  color: $greyish-brown
.notmain
  display: flex
  width: 100%
  justify-content: space-around
.phone
  display: flex
  width: $phone_width
  background: $black
  border-top: 44px solid $white
  border-right: 14px solid $white
  border-left: 14px solid $white
  border-bottom: 44px solid $white
  border-radius: 18px
  justify-content: center
  margin:
     right: 18%
  padding:
     top: 11%
     bottom: 13%
.phone h3
    color: #fcdb00
    font-size: 30px
@media screen and (max-width: 1024px)
  .logo
    margin-left: 12%
  .phone
    width: $adapt_phone_width
    margin-right: 0%
  .phone h3
    font-size: 24px
  .notmain
    justify-content: flex-start
  .main_text
    width: 51%
    margin-left: 13%
  .headerbar_links a
    display: none
  .bar
    margin-top: 1%
    display: flex
    margin-left: 60%
    height: 26px
@media screen and (max-width: 830px)
  .logo
    margin-left: 5%
  .main_text
    position: relative
    margin-left: 8%
    width: 90%
    height: 20%
  .phone
    display: none
.images
  margin-top: $images_top
.images img
  margin-right: $images_margin_right
.phone img
  height: 43px
  margin-right: 4%
.but
  display: flex
  justify-content: center
  margin:
    top: 3%
  padding-bottom: 3%
.but button
  background: $white
  border: none
  padding: 7px
  border-radius: 10px
  margin: 2px
</style>
