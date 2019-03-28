<template>
<div class="app">
    <div class="container-fluid pl-5 pr-5 pt-2 pb-2 fixed-top" data-aos="fade-down" data-aos-delay="100" data-aos-duration="500">
        <div class="row">
            <div class="col">
                <nuxt-link to="/" id="logo">
                    <div class='sprite logo'></div> astro
                </nuxt-link>
                <nav id="nav">
                    <ul>
                        <li data-aos="fade" data-aos-delay="400" data-aos-duration="600">
                            <nuxt-link to="/solutions">Solutions</nuxt-link>
                        </li>
                        <li data-aos="fade" data-aos-delay="800" data-aos-duration="500">
                            <nuxt-link to="/company">Company</nuxt-link>
                        </li>
                        <li data-aos="fade" data-aos-delay="500" data-aos-duration="700">
                            <nuxt-link to="/quote">Contact</nuxt-link>
                        </li>
                        <div class="underbar"></div>
                    </ul>
                </nav>
                <ul id="meta" class="text-right nav-right">
                    <li><a href="https://medium.com/adeeley" target="_blank"><div class='sprite icon-medium'></div></a></li>
                    <li><a href="https://twitter.com/AstroWebio" target="_blank"><div class='sprite icon-twitter'></div></a></li>
                    <li><a href="https://www.facebook.com/Astroweb-391066608368824" target="_blank"><div class='sprite icon-facebook'></div></a></li>
                    <li><a href="#dashlogin" class="trigger-btn btn btn-purple mc-embedded-subscribe hvr-grow" data-toggle="modal">Dashboard</a></li>
                </ul>
            </div>
        </div>
    </div>
    <nuxt />
    <div class="container-fluid p-5" id="newsletter" data-aos="fade" data-aos-duration="1000" data-aos-delay="200">
        <div class="row pt-2 pl-5 pr-5">
            <div class="col text-center">
                <h3>Earn great deals, make connections and stay informed!</h3>
                <div class="mc_embed_signup clearfix">
                    <form action="https://adeeley.us13.list-manage.com/subscribe/post?u=4f64ea438f655b88ee5728d92&amp;id=cfed167a58" method="post" class="mc-embedded-subscribe-form" name="mc-embedded-subscribe-form validate" target="_blank" novalidate>
                        <div class="mc_embed_signup_scroll">
                            <input type="email" value="" name="EMAIL" class="email" id="mce-EMAIL" placeholder="Enter your email" required>
                            <div style="position: absolute; left: -5000px;" aria-hidden="true"><input type="text" name="b_4f64ea438f655b88ee5728d92_cfed167a58" tabindex="-1" value=""></div>
                                <div class="clear"><input type="submit" value="Join now" name="subscribe" class="mc-embedded-subscribe button hvr-buzz-out"></div>
                                </div>
                    </form>
                </div>
            </div>
        </div>
    </div>
    <footer>
        <div class="container-fluid p-5" data-aos="fade" data-aos-delay="300" data-aos-duration="1200">
            <div class="row">
                <div class="col text-center">
                    <div id="logo-bot">
                        <div class='sprite logo2'></div>
                        <h2>astro</h2>
                        <div class="logo-text">&copy; 2019 ASTRO</div>
                    </div>
                    <ul id="nav-bot" class="pt-5">
                        <li>
                            <nuxt-link to="/privacy">Privacy Policy</nuxt-link>
                        </li>
                        <li>
                            <nuxt-link to="/terms">Terms &amp; Conditions</nuxt-link>
                        </li>
                        <li>
                            <a href="https://dash.astroweb.io:8118" target="_blank">Dashboard</a>
                        </li>
                    </ul>
                </div>
            </div>
        </div>
    </footer>
    <div class="fixed-bottom">
        <div class="alert alert-light alert-dismissible fade show text-center" role="alert">
            We use cookies to tailor your experience and measure site performance. View <nuxt-link to="/privacy">our policies here</nuxt-link>.
            <button type="button" class="close" data-dismiss="alert" aria-label="Close">
            <span aria-hidden="true">&times;</span>
          </button>
        </div>
    </div>
    <div id="dashlogin" class="modal fade">
        <div class="modal-dialog modal-login">
            <div class="modal-content">
                <div class="modal-header">
                    <h4 class="modal-title">Dashboard Login</h4>
                    <button type="button" class="close" data-dismiss="modal" aria-hidden="true">&times;</button>
                </div>
                <form id="loginForm" name="loginForm" method="post" action="https://dash.astroweb.io:8118/login">
                <div class="modal-body">
                        <div class="form-group">
                            <i class="fa fa-user"></i>
                            <input type="text" class="form-control" placeholder="Username" required="required" name="login-username" id="login-username">
</div>
                            <div class="form-group">
                                <i class="fa fa-lock"></i>
                                <input type="password" class="form-control" placeholder="Password" required="required" id="login-password" name="login-password">
</div>
                                <div class="form-group">
                                    <input type="submit" class="btn btn-primary btn-block btn-lg" value="Login">
</div>
                                </div>
                                <div class="modal-footer">
                                    <a href="https://dash.astroweb.io:8118" ta>Forgot Password?</a>
                                </div>
                    </form>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
  head () {
    return {
      script: [
        { src: 'https://cdnjs.cloudflare.com/ajax/libs/jquery/3.1.1/jquery.min.js' },
        { src: 'https://stackpath.bootstrapcdn.com/bootstrap/4.3.1/js/bootstrap.min.js' },
        { src: 'https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.14.7/popper.min.js' },
        { src: 'https://unpkg.com/aos@2.3.1/dist/aos.js' }
        
      ],
      link: [
        { rel: 'stylesheet', href: 'https://stackpath.bootstrapcdn.com/bootstrap/4.3.1/css/bootstrap.min.css' },
        { rel: 'stylesheet', href: 'https://cdnjs.cloudflare.com/ajax/libs/hover.css/2.3.1/css/hover-min.css' },
        { rel: 'stylesheet', href: 'https://fonts.googleapis.com/css?family=Rubik:300,400,400i,500,500i,700' },
        { rel: 'stylesheet', href: 'https://fonts.googleapis.com/css?family=Roboto+Mono' }
      ]
    }
  }
}

</script>

<style>

html {
    scroll-behavior: smooth;
}

html,
body {
    max-width: 100%;
    overflow-x: hidden;
}

.alert {
    margin-bottom: 0 !important;
}

body {
    font-family: 'Rubik', sans-serif !important;
    color: #5D5D69;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
}

a,
a:visited,
a:active,
a:hover {
    color: #7E57C2;
}

textarea:focus, input:focus{
    outline: none;
}

h1,
h2,
h3,
h4,
h5,
h6 {
    color: #7E57C2;
}

footer {
    margin: 40px 0;
}

#main {
  margin:0;
  padding:0;
}

.fixed-top {
    background: #fff;
}

.alert {
    font-size: 10pt;
    margin-bottom: 0;
    border-radius: 0;
    border-right: 0;
    border-left: 0;
    border-bottom: 0;
}

.alert a {
    text-decoration: underline;
}

#newsletter {
    background-image:url("~assets/bg2.jpg");
    background-repeat: no-repeat;
    padding: 100px 0 !important;
    margin-top:-45px;
    width: 100%;
    text-align: center;
    background-attachment: fixed;
    background-position: center;
}

#footer {
    padding: 60px;
}

#logo {
    float: left;
    color: #7E57C2;
    font-size: 24pt;
    font-weight: 500;
    vertical-align: middle;
}

#logo div {
    float: left;
    margin-right: 20px;
}

#logo {
    margin-right: 40px;
}

a#logo {
    color: #7E57C2;
    text-decoration: none;
}

#nav {
    margin-top: 14px;
    float:left;
}

#nav li a,
#nav-bot li a {
    color: #5D5D69;
    font-size: 11pt;
    font-weight: 500;
    text-decoration: none;
    padding-bottom: 4px;
    transition: .1s ease-in-out;
}

#nav li a:hover,
#nav-bot li a:hover {
    border-bottom: 3px solid rgb(233, 233, 238);
}

#nav li a.nuxt-link-active,
#nav-bot li a.nuxt-link-active {
    color: #7E57C2;
    border-bottom: 3px solid #7E57C2;
}

h1,
h2 {
    font-weight: normal;
}

ul {
    list-style-type: none;
    padding: 0;
}

li {
    display: inline-block;
    margin: 0 10px;
}

.vh {
    height:100vh;
}

.text-right {
    text-align: right;
}

.text-left {
    text-align: left;
}

.text-center {
    text-align: center;
}

.big.text-center {
    max-width: 800px;
    margin: 0 auto !important;
}

nav {
    display: inline-block;
}

.nav-right {
    float: right;
    font-size: 9pt;
    color: #5D5D69;

}

.btn {
    border-radius: 100px !important;
    padding: 12px 22px !important;
}

.btn-purple {
    background: rgb(141, 102, 225) !important;
    color: #fff !important;
}

.btn-purple:hover {
    background: rgb(151, 112, 235);
}

.nav-right .btn {
    font-weight: 500 !important;
    font-size: 11p !important;
}

.paragraph p {
    margin-bottom: 35px !important;
    clear: both;
}

.paragraph h4 {
    margin: 35px 0;
}

.paragraph li {
    clear: both !important;
    float: none !important;

}

#logo-bot {
    color: #7E57C2;
    text-decoration: none;
    margin: 0 auto;
    width: 200px;
    text-align: center;
    float: none;
}

#logo-bot .sprite {
    float: left;
    margin-right: 20px;
}

#logo-bot h2 {
    font-size: 28pt;
    font-weight: 500;
    padding: 0;
    margin: 5px 0 0 0;
}

#logo-bot .logo-text {
    font-size: 9pt;
    color: #5D5D69;
    letter-spacing: 1px;
    margin: -2px 0 0 0;
    padding: 0;
}

#nav-bot li {
    margin-left: 30px;
}

#nav-bot li a {
    text-decoration: none;
    color: #7E57C2;
    font-size: 12pt;
}

#meta {
    margin: 5px 0 0 0;
}

#meta-bot {
    font-size: 9pt;
    color: #5D5D69;
}

#newsletter h3 {
    padding-bottom: 45px;
    font-size:26pt;
    font-weight:300;
    color:#fff;
}

#newsletter label {
    float: left;
}

.mc_embed_signup_scroll {
    display:block;
    background:#fff;
    border-radius: 100px 100px 100px 100px;
    padding:12px;
    margin-top:30px;
    max-width:400px;
    height:70px;
    -webkit-box-shadow: 0 3px 68px rgba(0,0,0,.1);
    box-shadow: 0 3px 68px rgba(0,0,0,.1);
}

#newsletter .mc_embed_signup_scroll {
    margin:0 auto;
}

.mc_embed_signup_scroll input {
    border: none;
    width: 60%;
    padding: 10px 20px;
    color: #5D5D69;
    text-align: left;
    float:left;
}

input.mc-embedded-subscribe {
    background:#7E57C2;
    border-radius: 100px 100px 100px 100px;
    font-size:13pt;
    height:55px;
    float:right;
    width:40%;
    color:#fff;
    text-align:center;
    margin-top:-5px;
    cursor:pointer;
    transition: all .5s;
}

.mc_embed_signup_scroll:hover input.mc-embedded-subscribe {
    background:#9D78DE;
}

.header-img {
    float: right;
}

.caption {
    margin-top: 90px;
}

.caption .btn {
    border-radius: 0px;
}

.header img {
    width: 100%;
    height: auto;
}

.bg {
    background: #fff;
}

.bg2 {
    background: #FBFBFB;
}

.big h3 {
    font-size: 25pt;
    font-weight: 400;
    line-height: 1.5;
    margin: 0 auto;
    color: #333;
    font-weight: 500;
}

.big p {
    font-size: 14pt;
    margin: 0 auto;
    line-height: 1.9;
    color: #5D5D69;
}

.split .text {
    margin-top: 100px;
}

.split .text img {
    width: 36px;
    height: auto;
}

.split .text h4 {
    color: #333;
    font-size: 19pt;
    margin-top: 10px;
}

.split .text p {
    font-size: 15pt;
    color: #5D5D69;
}
#card-nav {
    margin: 0 auto;
    padding: 0;
    max-width: 800px;
}

#card-nav.contact {
    max-width: 400px;
}

#card-nav li {
    width: 25%;
    margin: 0;
}

#card-nav.contact li {
    width: 50% !important;
}

#card-nav li a {
    width: 100%;
    text-align: center;
    display: block;
    padding: 16px 0;
    background: #E9EAED;
    color: rgb(176, 173, 182);
    text-decoration: none;
    font-size: 11pt;
    font-weight: 500;
}

#card-nav li:first-child a {
    border-radius: 8px 0 0 8px;
}

#card-nav li:last-child a {
    border-radius: 0 8px 8px 0;
}

#card-nav li a:hover {
    color: #fff;
    background: rgb(134, 94, 204);
}

#card-nav li a.active {
    color: #fff;
    background: #7E57C2;
}

#card-content .cd {
    width: 30%;
    border: none;
    border-radius: 8px;
    background: #F7F6F6;
    margin-bottom: 40px;
    margin-right: 3%;
    height: 240px;
    float: left;
}

.vh100 {
    height: 100vh;
}

.overflow {
    overflow: hidden;
    max-height: 600px;
}

.overflow.override {
    max-height: 100%;
}

.overflow img {
    height: 100% !important;
    width: auto !important;
    float: right;
}

#card-content .cd .outer {
    background: #E9EAED;
    float: left;
    display: block;
    height: 100%;
    padding: 30px 15px 0 15px;
    border-radius: 8px 0 0 8px;
    margin-right: 15px;
}

#card-content .cd h5 {
    padding-top: 30px;
    font-size: 10pt;
    text-transform: uppercase;
}

#card-content .cd h3 {
    color: #5D5D69;
    margin: 10px 0;
    font-size:14pt;
}

#card-content .cd p {
    color: #717171;
    font-size:12pt;
    font-weight: 200;
    padding-right: 25px;
}

.caption h1 {
    font-size: 26pt;
    color: #333;
    font-weight: 500;
    margin-bottom: 20px;
}

.caption p {
    font-size: 13pt;
    line-height: 1.7;
}

.highlight {
    font-size: 10pt;
    color: #aaa;
    margin-bottom: 10px;
}

.highlight span {
    background: #1E88E5;
    font-weight: 600;
    color: #fff;
    border-radius: 100px;
    padding: 2px 8px;
    font-size: 8pt;
    margin-right: 3px;
}

#solutions h5 {
    color: #333;
    text-align: center;
    margin-bottom: 55px;
}

.mini-card {
    float: right;
    width: 50%;
    text-align: center;
    margin-bottom: 20px;
    font-size: 10pt;
}

.mini-card div {
    margin: 0 auto;
    margin-top: 5px;
}

.card-left .mini-card {
    float: left !important;
}

.modal-login {
    color: #636363 !important;
    width: 350px !important;
    margin-top: 100px;
}

.modal-login .modal-content {
    padding: 20px !important;
    border-radius: 5px !important;
    border: none !important;
}

.modal-login .modal-header {
    border-bottom: none;
    position: relative;
    justify-content: center;
}

.modal-login h4 {
    text-align: center;
    font-size: 26px;
}

.modal-login .form-group {
    position: relative;
}

.modal-login i {
    position: absolute;
    left: 13px;
    top: 11px;
    font-size: 18px;
}

.modal-login .form-control {
    padding-left: 40px;
}

.modal-login .form-control:focus {
    border-color: #00ce81;
}

.modal-login .form-control,
.modal-login .btn {
    min-height: 40px;
    border-radius: 3px;
}

.modal-login .hint-text {
    text-align: center;
    padding-top: 10px;
}

.modal-login .close {
    position: absolute;
    top: -5px;
    right: -5px;
}

.modal-login .btn {
    background: #00ce81 !important;
    border: none;
    line-height: normal;
}

.modal-login .btn:hover,
.modal-login .btn:focus {
    background: #00bf78 !important;
}

.modal-login .modal-footer {
    background: #ecf0f1;
    border-color: #dee4e7;
    text-align: center;
    margin: 0 -20px -20px;
    border-radius: 5px;
    font-size: 13px;
    justify-content: center;
}

.modal-login .modal-footer a {
    color: #999;
}

.modal-title {
    color: #333;
}

.fullsplit .col {
    padding: 0 !important;
}

.fullsplit img {
    width: 100%;
    height: auto;
}

.fullsplit h2,
.fullsplit h3,
.fullsplit h4,
.fullsplit h5 {
    margin: 0 0 0 40px;
}

.fullsplit h4 {
    font-size: 15pt;
    color: #333;
}

.fullsplit h2 {
    color: #333;
    line-height: 1.8;
    max-width: 600px;
    margin: 0 auto;
    padding: 0 40px;
}

.fullsplit p {
    margin: 20px 40px 20px 40px;
}

.fullsplit h2 p {
    margin: 0 !important;
}

.split-right {
    flex-direction: row-reverse;
}

.lister {
    color: #7E57C2;
    font-size: 24pt;
    line-height: 1.9;
    list-style-type: decimal !important;
}

.lister li {
    list-style-type: decimal !important;
    display: list-item;
    float: none;
    clear: both;
    margin: 10px 0;
}

.stay {
    margin: 0;
    text-align: left;
}

.company-p {
    font-size: 18pt !important;
    text-align: left;
    max-width: 100% !important;
    margin: 0 !important;
    line-height: 1.9;
}

.fluid-img {
    max-width: 100%;
    height: auto;
}

.sprite {
    background: url('~assets/sprite-min.png') no-repeat top left;
    width: 94px;
    height: 100px;
}

.sprite.angular {
    background-position: 0 0;
    width: 50px;
    height: 53px;
}

.sprite.architecture {
    background-position: 0 -55px;
    width: 36px;
    height: 40px;
}

.sprite.babel {
    background-position: 0 -97px;
    width: 63px;
    height: 25px;
}

.sprite.bootstrap {
    background-position: 0 -124px;
    width: 58px;
    height: 55px;
}

.sprite.cloudflare {
    background-position: 0 -181px;
    width: 57px;
    height: 27px;
}

.sprite.conception {
    background-position: 0 -210px;
    width: 40px;
    height: 45px;
}

.sprite.contact-backend {
    background-position: 0 -257px;
    width: 76px;
    height: 74px;
}

.sprite.contact-design {
    background-position: 0 -333px;
    width: 80px;
    height: 80px;
}

.sprite.contact-frontend {
    background-position: 0 -415px;
    width: 80px;
    height: 80px;
}

.sprite.contact-mobileapp {
    background-position: 0 -497px;
    width: 80px;
    height: 84px;
}

.sprite.contact-other {
    background-position: 0 -583px;
    width: 80px;
    height: 68px;
}

.sprite.contact-webdev {
    background-position: 0 -653px;
    width: 72px;
    height: 72px;
}

.sprite.contentful {
    background-position: 0 -727px;
    width: 45px;
    height: 51px;
}

.sprite.development {
    background-position: 0 -780px;
    width: 38px;
    height: 38px;
}

.sprite.digitalocean {
    background-position: 0 -820px;
    width: 49px;
    height: 49px;
}

.sprite.drupal {
    background-position: 0 -871px;
    width: 50px;
    height: 57px;
}

.sprite.elixir {
    background-position: 0 -930px;
    width: 40px;
    height: 60px;
}

.sprite.enduro {
    background-position: 0 -992px;
    width: 54px;
    height: 59px;
}

.sprite.erlang {
    background-position: 0 -1053px;
    width: 57px;
    height: 37px;
}

.sprite.favicon {
    background-position: 0 -1092px;
    width: 32px;
    height: 32px;
}

.sprite.gatsby {
    background-position: 0 -1126px;
    width: 62px;
    height: 62px;
}

.sprite.ghost {
    background-position: 0 -1190px;
    width: 39px;
    height: 40px;
}

.sprite.github {
    background-position: 0 -1232px;
    width: 66px;
    height: 64px;
}

.sprite.icon-facebook {
    background-position: 0 -1298px;
    width: 15px;
    height: 14px;
}

.sprite.icon-github {
    background-position: 0 -1314px;
    width: 17px;
    height: 16px;
}

.sprite.icon-phone {
    background-position: 0 -1332px;
    width: 15px;
    height: 16px;
}

.sprite.icon-twitter {
    background-position: 0 -1350px;
    width: 18px;
    height: 14px;
}

.sprite.icon-medium {
    background-position: 0 -5948px;
    width:14px;
    height:11px;
}

.sprite.icon-bolt {
    background-position: 0 -5928px;
    width:11px;
    height:18px;
}

.sprite.keystone {
    background-position: 0 -1366px;
    width: 45px;
    height: 46px;
}

.sprite.laravel {
    background-position: 0 -1414px;
    width: 54px;
    height: 37px;
}

.sprite.linode {
    background-position: 0 -1453px;
    width: 45px;
    height: 53px;
}

.sprite.logo {
    background-position: 0 -1508px;
    width: 55px;
    height: 51px;
}

.sprite.logo2 {
    background-position: 0 -1561px;
    width: 68px;
    height: 70px;
}

.sprite.magento {
    background-position: 0 -1633px;
    width: 47px;
    height: 54px;
}

.sprite.maintenance {
    background-position: 0 -1689px;
    width: 38px;
    height: 38px;
}

.sprite.mongodb {
    background-position: 0 -1729px;
    width: 24px;
    height: 54px;
}

.sprite.nginx {
    background-position: 0 -1785px;
    width: 51px;
    height: 57px;
}

.sprite.node {
    background-position: 0 -1844px;
    width: 52px;
    height: 58px;
}

.sprite.phoenix {
    background-position: 0 -1904px;
    width: 56px;
    height: 38px;
}

.sprite.php {
    background-position: 0 -1944px;
    width: 54px;
    height: 26px;
}

.sprite.postgresql {
    background-position: 0 -1972px;
    width: 46px;
    height: 47px;
}

.sprite.react {
    background-position: 0 -2021px;
    width: 53px;
    height: 49px;
}

.sprite.redis {
    background-position: 0 -2072px;
    width: 56px;
    height: 48px;
}

.sprite.ruby {
    background-position: 0 -2122px;
    width: 45px;
    height: 45px;
}

.sprite.spina {
    background-position: 0 -2169px;
    width: 55px;
    height: 42px;
}

.sprite.symfony {
    background-position: 0 -2213px;
    width: 57px;
    height: 56px;
}

.sprite.ubuntu {
    background-position: 0 -2271px;
    width: 49px;
    height: 51px;
}

.sprite.uiux {
    background-position: 0 -2324px;
    width: 36px;
    height: 36px;
}

.sprite.varnish {
    background-position: 0 -2362px;
    width: 45px;
    height: 45px;
}

.sprite.vue {
    background-position: 0 -2409px;
    width: 47px;
    height: 41px;
}

.sprite.webpack {
    background-position: 0 -2452px;
    width: 50px;
    height: 58px;
}

.sprite.wordpress {
    background-position: 0 -2512px;
    width: 51px;
    height: 51px;
}

.sprite.cards-angular {
    background-position: 0 -2565px;
}

.sprite.cards-babel {
    background-position: 0 -2667px;
}

.sprite.cards-bootstrap {
    background-position: 0 -2769px;
}

.sprite.cards-cloudflare {
    background-position: 0 -2871px;
}

.sprite.cards-contentful {
    background-position: 0 -2973px;
}

.sprite.cards-digitalocean {
    background-position: 0 -3075px;
}

.sprite.cards-drupal {
    background-position: 0 -3177px;
}

.sprite.cards-elixir {
    background-position: 0 -3279px;
}

.sprite.cards-enduro {
    background-position: 0 -3381px;
}

.sprite.cards-erlang {
    background-position: 0 -3483px;
}

.sprite.cards-gatsby {
    background-position: 0 -3585px;
}

.sprite.cards-ghost {
    background-position: 0 -3687px;
}

.sprite.cards-github {
    background-position: 0 -3789px;
}

.sprite.cards-keystone {
    background-position: 0 -3891px;
}

.sprite.cards-laravel {
    background-position: 0 -3993px;
}

.sprite.cards-linode {
    background-position: 0 -4095px;
}

.sprite.cards-magento {
    background-position: 0 -4197px;
}

.sprite.cards-mongodb {
    background-position: 0 -4299px;
}

.sprite.cards-nginx {
    background-position: 0 -4401px;
}

.sprite.cards-node {
    background-position: 0 -4503px;
}

.sprite.cards-phoenix {
    background-position: 0 -4605px;
}

.sprite.cards-php {
    background-position: 0 -4707px;
}

.sprite.cards-postgresql {
    background-position: 0 -4809px;
}

.sprite.cards-react {
    background-position: 0 -4911px;
}

.sprite.cards-redis {
    background-position: 0 -5013px;
}

.sprite.cards-ruby {
    background-position: 0 -5115px;
}

.sprite.cards-spina {
    background-position: 0 -5217px;
}

.sprite.cards-symfony {
    background-position: 0 -5319px;
}

.sprite.cards-ubuntu {
    background-position: 0 -5421px;
}

.sprite.cards-varnish {
    background-position: 0 -5523px;
}

.sprite.cards-vue {
    background-position: 0 -5625px;
}

.sprite.cards-webpack {
    background-position: 0 -5727px;
}

.sprite.cards-wordpress {
    background-position: 0 -5829px;
}

@media only screen and (max-width: 900px) {
    .mini-card {
        width: 100%;
    }

    #card-content .cd p {
        display: none;
    }

    #card-content .cd {
        height: 140px;
    }

    #card-content .cd h3 {
        font-size: 11pt;
    }

    #card-content .cd h5 {
        font-size: 8pt;
    }

    #card-content .cd {
        height: 120px;
    }
    #solutions .col {
        clear: both;
    }

    .fullsplit .col {
        margin: 40px 0;
    }

    .col-6 {
        flex: 0 0 100% !important;
        max-width: 100% !important;
    }

    #logo {
        margin-right: 0 !important;
    }

    #nav * {
        font-size: 10pt !important;
    }

    #nav li {
        margin: 0 5px !important;
    }

    #nav ul {
        margin: 0px 0 0 20px;
    }

    #logo {
        font-size: 0pt !important;
    }

    .overflow {
        display: none !important;
    }

    .nav-right .btn {
        display: none;
    }

    .nav-right {
        display: none;
    }

    #card-content .cd {
        width: 45%;
        margin-right: 5%;
    }

    #logo div {
        margin-right: 0 !important;
    }

    .lister li {
        font-size: 18pt !important;
        line-height: 1.7;
    }

    .stay {
        margin: 80px 0 0 0 !important;
    }

    #card-nav li a {
        font-size:9pt !important;
    }
}

@media only screen and (max-width: 500px) {

    #card-content .cd {
        width: 100%;
    }
}
</style>

