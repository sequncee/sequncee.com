<template>
  <header id="header" class="header-white type-2">
    <div class="header-holder">
      <div class="logo">
        <a aria-label="logo-link to homepage" href="/" class="icon-xe"></a>
      </div>
      <nav class="main-nav">
        <a href="#" aria-label="Open the menu" class="nav-opener"
          ><span>menu</span></a
        >

        <div class="nav-holder">
          <ul class="nav-list list">
            <li><a aria-label="Work" href="/work.html" class="">Work</a></li>
            <li>
              <a aria-label="Capabilities" href="/capabilities.html" class=""
                >Capabilities</a
              >
            </li>
            <li><a aria-label="About" href="/about.html" class="">About</a></li>
            <li><a aria-label="News" href="/news.html" class="">News</a></li>
            <!-- <li>
              <a aria-label="Blog" href="https://blog.thegnar.co" class=""
                >Blog</a
              >
            </li> -->
            <li>
              <a aria-label="Hire Us" href="/hire-us.html" class="">Hire Us</a>
            </li>
          </ul>

          <img src="/images/mobile-menu-img.png" alt="image descripton" />
        </div>
      </nav>
    </div>
  </header>
</template>
<script>
export default {
  name: "Header"
};
</script>

<style scoped>
#header {
  display: block;
}
/* @font-face {
  font-family: "icomoon";
  src: url("../fonts/icomoon/icomoon.eot?h39hva");
  src: url("../fonts/icomoon/icomoon.eot?h39hva#iefix")
      format("embedded-opentype"),
    url("../fonts/icomoon/icomoon.ttf?h39hva") format("truetype"),
    url("../fonts/icomoon/icomoon.woff?h39hva") format("woff"),
    url("../fonts/icomoon/icomoon.svg?h39hva#icomoon") format("svg");
  font-weight: normal;
  font-style: normal;
} */
[class^="icon-"],
[class*=" icon-"] {
  /* use !important to prevent issues with browser extensions that change fonts */
  font-family: "icomoon" !important;
  /* speak: none; */
  font-style: normal;
  font-weight: normal;
  font-variant: normal;
  text-transform: none;
  line-height: 1;
  /* Better Font Rendering =========== */
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}

.icon-xe:before {
  content: "\e900";
}

[id="header"].header-white .logo .icon-xe {
  color: #fff;
}
[id="header"].header-white .nav-holder a {
  color: #fff;
}
[id="header"].header-white .nav-holder a:before {
  background: #fff;
}
[id="header"].header-white .nav-opener span,
[id="header"].header-white .nav-opener:before,
[id="header"].header-white .nav-opener:after {
  background: #fff;
}
[id="header"].type-2 {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
}
[id="header"] .header-holder {
  position: relative;
  display: -ms-flexbox;
  display: flex;
  -ms-flex-align: center;
  align-items: center;
  -ms-flex-pack: justify;
  justify-content: space-between;
  padding: 37px 34px;
  z-index: 2;
}
@media (min-width: 768px) {
  [id="header"] .header-holder {
    padding: 30px 40px;
    max-width: 1360px;
    margin: 0 auto;
  }
}
[id="header"] .logo {
  position: relative;
  z-index: 1;
  line-height: 1;
}
[id="header"] .logo .icon-xe {
  color: #3f3f41;
  font-size: 25px;
  text-decoration: none;
  transition: color 0.6s;
}
@media (min-width: 768px) {
  [id="header"] .logo .icon-xe {
    font-size: 36px;
  }
}
.nav-active [id="header"] .logo .icon-xe {
  color: #fff;
}
.primary-bg [id="header"] .logo .icon-xe {
  color: #fff;
}

.main-nav.color-white .nav-holder a {
  color: #fff;
}
.main-nav .nav-holder {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  padding: 157px 0 13px;
  background: #f86249;
  opacity: 0;
  visibility: hidden;
  transition: opacity 0.6s, visibility 0.6s;
  text-align: center;
  font-size: 24px;
  font-weight: 600;
  line-height: 2.416;
}
@media (min-width: 768px) {
  .main-nav .nav-holder {
    position: relative;
    display: -ms-flexbox;
    display: flex;
    padding: 0;
    opacity: 1;
    visibility: visible;
    background: transparent;
    text-align: left;
  }
}
.nav-active .main-nav .nav-holder {
  opacity: 1;
  visibility: visible;
}
.main-nav .nav-holder a {
  color: #fff;
  text-decoration: none;
}
@media (min-width: 768px) {
  .main-nav .nav-holder a {
    color: #3f3f41;
    font-size: 16px;
  }
}
@media (min-width: 768px) {
  .main-nav .nav-holder img {
    display: none;
  }
}
.main-nav .nav-list {
  margin: 0 0 60px;
}
@media (min-width: 768px) {
  .main-nav .nav-list {
    margin: 0;
  }
}
@media (min-width: 768px) {
  .main-nav .nav-list li {
    display: inline-block;
  }
}
@media (min-width: 768px) {
  .main-nav .nav-list li + li {
    margin-left: 20px;
  }
}
.main-nav .nav-list a {
  position: relative;
}
.main-nav .nav-list a:before {
  content: "";
  position: absolute;
  bottom: -3px;
  left: -5px;
  right: -5px;
  height: 2px;
  background: #3f3f41;
  opacity: 0;
  transition: opacity 0.3s;
}
.main-nav .nav-list a.is-active:before {
  opacity: 1;
}
.main-nav .nav-list a:hover:before {
  opacity: 1;
}
.main-nav .nav-list .active {
  font-weight: 700;
}
.main-nav .nav-list .active a:before {
  opacity: 1;
}

.nav-opener {
  width: 40px;
  height: 40px;
  position: relative;
  display: block;
  overflow: hidden;
  z-index: 1;
  text-indent: -9999px;
}
@media (min-width: 768px) {
  .nav-opener {
    display: none;
  }
}
.nav-opener:before,
.nav-opener:after,
.nav-opener span {
  background: #3f3f41;
  position: absolute;
  top: 18px;
  left: 10%;
  right: 10%;
  height: 2px;
  margin-top: -2px;
  transition: all 0.3s linear;
}
.nav-opener:before,
.nav-opener:after {
  content: "";
  top: 10px;
}
.nav-opener:after {
  top: 26px;
  right: 40%;
}
.nav-active .nav-opener span {
  opacity: 0;
}
.nav-active .nav-opener:after,
.nav-active .nav-opener:before {
  transform: rotate(35deg);
  top: 20px;
  left: 10%;
  right: 10%;
}
.nav-active .nav-opener:after {
  transform: rotate(-35deg);
}
</style>
