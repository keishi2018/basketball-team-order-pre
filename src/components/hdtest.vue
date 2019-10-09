<!-- header - start -->
<div id="headerWrap">
    <div class="js-modal-bk" @click="modalBkClick" :class="{active:modal_bk}"></div>
    <header class="header">
        <div class="headerInner">
            <div id="js-open-menu" class="header__menu" @click="mainMenuToggle" :class="{active:headerMenu_state}">
                <span class="header__menu__line"></span>
                <span class="header__menu__line"></span>
                <span class="header__menu__line"></span>
            </div>
            <!-- header__menu -->
       
<!-- MENU INNER - start --------------------------------------------------------------------------------------------->
            <div class="header__menu__inner" :class="{active:headerMenu_state}">
                <ul class="header__menuList">
                    <li><a href="">
                            <span>
                                sample
                            </span>
                        </a></li>
                    <li><a href="">
                            <span>
                                sample
                            </span>
                        </a></li>
                </ul><!-- header__menuList -->
            </div><!-- header__menu__inner -->
            <!-- MENU INNER - end --------------------------------------------------------------------------------------------->
            <h1 class="header__logo">logo</h1>
        </div>
        <!-- headerInner -->
    </header>
</div>
<!-- header - end -->

<style>
/* ------------------------------------ */
//  リセット
/* ------------------------------------ */

html, body, div, span, applet, object, iframe,
h1, h2, h3, h4, h5, h6, p, blockquote, pre,
a, abbr, acronym, address, big, cite, code,
del, dfn, img, ins, kbd, q, s, samp,
small, strike, strong, sub, sup, tt, var,
b, u, i, center,
dl, dt, dd, ol, ul, li,
fieldset, form, label, legend,
table, caption, tbody, tfoot, thead, tr, th, td,
article, aside, canvas, details, embed,
figure, figcaption, footer, header, hgroup,
menu, nav, output, ruby, section, summary,
time, mark, audio, video
  margin: 0
  padding: 0
  border: 0
  color: #333333
  font-size: 100%
  vertical-align: baseline
  box-sizing: border-box

h1, h2, h3, h4, h5, h6
  font-weight: 500
  line-height: 1.4

article, aside, details, figcaption, figure,
footer, header, hgroup, menu, nav, section
  display: block

li
  list-style: none


/* ------------------------------------ */
//  mixin
/* ------------------------------------ */

@mixin afterContent($top,$right,$bottom,$left,$widh,$height)
  position: absolute
  top: $top
  right: $right
  bottom: $bottom
  left: $left
  width: $widh
  height: $height
  content: ""

 
/* ------------------------------------ */
//  header
/* ------------------------------------ */

.js-modal-bk
  opacity: 0
  visibility: hidden
  position: fixed
  z-index: 12
  top: 0
  left: 0
  width: 100%
  height: 100%
  background: rgba(0, 0, 0, 0.4)
  transition: all .3s

.js-modal-bk.active
  opacity: 1
  visibility: visible
  height: 100vh
  overflow: hidden

.header
  position: fixed
  z-index: 12
  top: 0
  right: 0
  left: 0
  width: 100%
  margin: 0 auto
  background: #fff
  border: 2px solid #ccc

.headerInner
  display: flex
  align-items: center
  justify-content: space-between

.header__menu
  display: flex
  align-items: center
  justify-content: center
  flex-wrap: wrap
  position: relative
  width: 44px
  height: 46px
  padding: 13px 10px
  transition: all .4s
  .header__menu__line
    display: block
    width: 15px
    height: 2px
    margin: 0 auto 0 0
    background: #0257BD
    transition: all .4s
    &:nth-child(3)
      width: 10px

.header__menu.active
  .header__menu__line
    position: relative
    width: 17px
    &:nth-of-type(1)
      top: -2px
      transform: translateY(5px) rotate(-45deg)
    &:nth-of-type(2)
      opacity: 0
    &:nth-of-type(3)
      top: 0
      width: 17px
      transform: translateY(-10px) rotate(45deg)

.header__notice
  display: flex
  align-items: center
  justify-content: center
  position: absolute
  top: 7px
  right: -5px
  min-width: 20px
  min-height: 20px
  padding: 2px
  box-sizing: border-box
  background: rgb(233, 84, 93)
  border-radius: 50%
  color: #fff
  font-size: 10px
  span
    display: inline-block
    margin-left: 2px
    color: #fff

.header__logo
  display: flex
  align-items: center
  justify-content: center
  position: absolute
  top: 0
  right: 0
  bottom: 0
  left: 0
  width: 32%
  margin: auto

.header__iconWrap
  display: flex

.header__icon
  display: block
  padding: 10px 11px
  img
    width: 100%

.header__menu__inner
  position: fixed
  top: 50px
  left: 0
  width: 82%
  height: calc(100vh - 46px)
  background: #fff
  font-size: 14px
  transform: translateX(-100%)
  transition: all .3s

.header__menu__inner.active
  transform: translateX(0)

.header__menuList
  margin-bottom: 20px
  >li
    position: relative
    border-bottom: 1px solid rgb(240, 243, 246)
    &:after
      @include afterContent(0, 18px, 0, auto, 0, 0)
      margin: auto
      border-top: 6px solid transparent
      border-bottom: 6px solid transparent
      border-left: 6px solid rgb(2, 87, 189)
  a
    display: block
    padding: 15px 45px 15px 15px
    line-height: 1.5
    span
      position: relative
      .header__notice
        top: 0
        right: -30px
        bottom: 0
        margin: auto
</style>

<script>
new Vue({
  el: '#headerWrap',
  data: {
    headerMenu_state: false,
    modal_bk: false,
  },
  methods: {
    mainMenuToggle: function () {
      if (this.headerMenu_state == true) {
        this.headerMenu_state = false;
        this.modal_bk = false;
        return;
      }
      this.headerMenu_state = true;
      this.modal_bk = true;
    },
    modalBkClick: function () {
      this.headerMenu_state = false;
      this.modal_bk = false;
    },
  }
});
</script>
