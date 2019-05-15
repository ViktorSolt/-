<template lang="html">
  <div class="Content">
    <div class="title">
      <h1>Tinyone features</h1>
      <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Praesent vitae eros eget tellus<br>
        tristique bibendum. Donec rutrum sed sem quis venenatis.</p>
    </div>
    <div class="con">
      <div class="first ContentBar">
        <div class="image">
          <div class="lol">
            <img src="./../assets/icon-font-1.png" alt="">
          </div>
          <h3>Fully Responsive</h3>
        </div>
        <div class="text">
          <p>Lorem ipsum dolor sit amet,<br>
            consectetur adipiscing elit.<br>
            Praesent vitae eros eget tellus<br>
            tristique bibendum.</p>
          </div>
        </div>
          <div class="first ContentBar">
            <div class="image">
              <div class="lol">
                <img src="./../assets/icon-font-3.png" alt="">
              </div>
              <h3>Fully Layered PSD</h3>
            </div>
            <div class="text">
              <p>Lorem ipsum dolor sit amet,<br>
                consectetur adipiscing elit.<br>
                Praesent vitae eros eget tellus<br>
                tristique bibendum.</p>
              </div>
          </div>
      <div class="first ContentBar2">
        <div class="image">
          <div class="lol">
            <img src="./../assets/icon-font-2.png" alt="">
          </div>
          <h3>Font Awesome Icons</h3>
        </div>
        <div class="text">
          <p>Lorem ipsum dolor sit amet,<br>
            consectetur adipiscing elit.<br>
            Praesent vitae eros eget tellus<br>
            tristique bibendum.</p>
          </div>
        </div>
         <div class="second ContentBar2">
           <div class="image">
             <div class="lol">
               <img src="./../assets/icon-font-4.png" alt="">
             </div>
             <h3>HTML3 & CSS3</h3>
           </div>
           <div class="text">
             <p>Lorem ipsum dolor sit amet,<br>
               consectetur adipiscing elit.<br>
               Praesent vitae eros eget tellus<br>
               tristique bibendum.</p>
             </div>
         </div>
         <div class="second ContentBar3">
           <div class="image">
             <div class="lol">
               <img src="./../assets/icon-font-3-.png" alt="">
             </div>
             <h3>Email Template</h3>
           </div>
           <div class="text">
             <p>Lorem ipsum dolor sit amet,<br>
               consectetur adipiscing elit.<br>
               Praesent vitae eros eget tellus<br>
               tristique bibendum.</p>
             </div>
           </div>
           <div class="second ContentBar3">
           <div class="image">
             <div class="lol">
               <img src="./../assets/icon-font-2-.png" alt="">
             </div>
             <h3>Free to download</h3>
           </div>
           <div class="text">
             <p>Lorem ipsum dolor sit amet,<br>
               consectetur adipiscing elit.<br>
               Praesent vitae eros eget tellus<br>
               tristique bibendum.</p>
             </div>
         </div>
       </div>
    </div>
</template>

<script>
export default {
}
</script>

<style lang="sass" scoped>
@import './assets/variables'
.Content
  font-family: PTSans
.title
  text-align: center
.title h1
  font-family: PTSans
  font-size: 26px
  font-weight: bold
  color: $black
  margin:
    top: 8%
    bottom: 1%
.title p
  font-size: 17px
  margin-bottom: 6%
  color: #313841
  line-height: 1.4
.text p
  font-size: 13px
  color: $warm-grey
.first,
.second
  display: inline-flex
  flex-direction: column
  margin-bottom: 6%
  margin-right: 2%
  width: 20%
.second
  margin-bottom: 12%
.first:nth-child(1),
.second:nth-child(4)
  margin-left: 17%
.first:nth-child(3),
.second:nth-child(6)
  margin-right: 15%
.lol
  display: block
  width: 60px
.text
  display: flex
  margin-left: 60px
.image
  display: flex
.image h3
  font-size: 16px
  color: $black
  margin-bottom: 2%
@media screen and (max-width: 1024px)
  .first,
  .second
    width: 0
    margin-right: 0%
    margin-bottom: 0%
  .first:nth-child(3),
  .second:nth-child(6)
    margin-right: 0%
  .second:nth-child(4)
    margin-left: 0%
  .ContentBar,
  .ContentBar2,
  .ContentBar3
    display: inline-flex
    flex-direction: column
    width: 40%
    margin-top: 2%
  .ContentBar:nth-child(1),
  .ContentBar2:nth-child(3),
  .ContentBar3:nth-child(5)
    margin-left: 14%
  .ContentBar:nth-child(2),
  .ContentBar2:nth-child(4)
    margin-right: 5%
  .ContentBar3:nth-child(6)
    margin-right: 5%
    margin-bottom: 12%
@media screen and (max-width: 600px)
  .ContentBar,
  .ContentBar2,
  .ContentBar2:nth-child(4),
  .ContentBar3
     display: flex
     flex-direction: column
     width: 86%
     margin-left: 14%
</style>
