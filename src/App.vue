<template>

  <div id="app">

    <section class="main">
      <!-- .rm-container -->
      <div id="rm-container" class="rm-container" v-bind:class="[{'rm-open' : isActive}, {'rm-closed' : isInactive}]">


        <!-- HEADER -->
        <header id="header">

          <!-- NAV MENU -->
          <nav>
            <ul>
              <li><a href='index.html#/home'></a></li>
              <li><a href='index.html#/resume'></a></li>
              <li><a href='index.html#/portfolio'></a></li>
              <li><a href='index.html#/contact'></a></li>
            </ul>
          </nav>
          <!-- NAV MENU -->

        </header>
        <!-- HEADER -->




        <!-- .rm-wrapper -->
        <div class="rm-wrapper" style="height: 570px">

          <!-- .rm-cover -->
          <div class="rm-cover">
            <!-- COVER PAGE -->
            <div id="home" class="rm-front page" v-on:click="openedBook">
              <!-- .antiscroll-wrap -->
              <div class="antiscroll-wrap">
                <!-- .antiscroll-inner -->
                <div class="antiscroll-inner">

                  <!-- COVER IMAGE -->
                  <home></home>
                  <!-- COVER IMAGE -->
                </div>
                <!-- .antiscroll-inner -->
              </div>
              <!-- .antiscroll-wrap -->
            </div>
            <!-- COVER PAGE -->

            <!-- RESUME PAGE -->
            <resume-page></resume-page>
            <!-- RESUME PAGE -->
          </div><!-- /rm-cover -->


          <!-- PORTFOLIO PAGE -->
          <portfolio></portfolio>
          <!-- PORTFOLIO PAGE -->



          <!-- RIGHT SIDE -->
          <div class="rm-right">



            <!-- .rm-front -->
            <div class="rm-front">

              <!-- BACK COVER IMAGE -->
              <div class="cover">

                <!-- cover-image-holder -->
                <div class="cover-image-holder">
                  <img src="images/site/cover-2.jpg" alt="cover-image">
                </div>
                <!-- cover-image-holder -->

              </div>
              <!-- BACK COVER IMAGE -->

            </div>
            <!-- .rm-front -->




            <!-- CONTACT PAGE -->
            <div id="contact" class="rm-back page">





              <!-- .antiscroll-wrap -->
              <div class="antiscroll-wrap">
                <!-- .antiscroll-inner -->
                <div class="antiscroll-inner">


                  <!-- CONTENT -->
                  <div class="content">


                    <h2><span>CONTACT</span></h2>


                    <!--<h3>Where am I in this world?</h3>
                    <div class="map">

                            <iframe src="https://maps.google.com/maps?source=s_q&amp;f=q&amp;hl=en&amp;geocode=&amp;q=little+italy&amp;aq=&amp;sll=36.558188,-86.709595&amp;sspn=3.878053,8.453979&amp;ie=UTF8&amp;hq=&amp;hnear=Little+Italy,+New+York&amp;t=p&amp;ll=40.84706,-73.125&amp;spn=6.647611,26.367188&amp;z=5&amp;output=embed"></iframe>

                    </div>-->


                    <p class="center">Please feel free to contact me about anything.</p>

                    <h3><span>LET'S SOCIALIZE</span></h3>

                    <!-- SOCIAL -->
                    <ul class="social">
                      <li><a class="facebook" href="index.html#"></a></li>
                      <li><a class="twitter" href="index.html#"></a></li>
                      <li><a class="linkedin" href="index.html#"></a></li>
                      <li><a class="google" href="index.html#"></a></li>
                      <li><a class="pinterest" href="index.html#"></a></li>
                      <li><a class="github" href="index.html#"></a></li>
                      <li><a class="behance" href="index.html#"></a></li>
                      <li><a class="dribble" href="index.html#"></a></li>
                      <!--<li><a class="instagram" href="#"></a></li>
                      <li><a class="lastfm" href="#"></a></li>
                      <li><a class="rss" href="#"></a></li>
                      <li><a class="vimeo" href="#"></a></li>
                      <li><a class="forrst" href="#"></a></li>
                      <li><a class="skype" href="#"></a></li>
                      <li><a class="picassa" href="#"></a></li>
                      <li><a class="youtube" href="#"></a></li>
                      <li><a class="flickr" href="#"></a></li>
                      <li><a class="tumblr" href="#"></a></li>
                      <li><a class="blogger" href="#"></a></li>
                      <li><a class="delicious" href="#"></a></li>
                      <li><a class="digg" href="#"></a></li>
                      <li><a class="friendfeed" href="#"></a></li>
                      <li><a class="wordpress" href="#"></a></li>-->
                    </ul>
                    <!-- SOCIAL -->


                    <h3><span>DROP ME A LINE!</span></h3>

                    <!-- .contact-form -->
                    <div class="contact-form">


                      <!-- LETTER -->
                      <div class="letter cf">

                        <div class="stamp">
                          <img src="images/site/stamp-image.png" alt="stamp">
                        </div>

                        <div class="letter-info">
                          <h4>Johhny Doe</h4>
                          <p><a href="index.html#"><i>johhny@gmail.com</i></a></p>
                          <p> - Planet Earth</p>
                        </div>

                      </div>
                      <!-- LETTER -->


                      <form id="contact-form" action="https://themes.pixelwars.org/bookcard/send-mail.php" method="post">

                        <!-- enter your e-mail address here -->
                        <input type="hidden" id="to" name="to" value="jonhdoeeee@jonhdoe.com">

                        <p>
                          <label for="name">Name</label>
                          <input type="text" name="name" id="name" class="required">
                        </p>

                        <p>
                          <label for="email">Email</label>
                          <input type="text" name="email" id="email" class="required email">
                        </p>

                        <p>
                          <label for="subject">Subject</label>
                          <input type="text" name="subject" id="subject" class="required">
                        </p>

                        <p>
                          <label for="message">Message</label>
                          <textarea name="message" id="message" class="required"></textarea>
                        </p>

                        <p>
                          <img class="ajax-loader" src="images/bckg/loader_light.gif" alt="Sending ...">
                          <input type="submit" class="btn submit" value="SEND">
                        </p>

                      </form>

                    </div>
                    <!-- .contact-form -->

                  </div>
                  <!-- CONTENT -->




                </div>
                <!-- .antiscroll-inner -->
              </div>
              <!-- .antiscroll-wrap -->


              <!-- close link -->
              <a class="rm-close" v-on:click="closedBook"><span></span></a>
              <!-- close link -->


            </div><!-- /rm-back -->
            <!-- CONTACT PAGE -->



          </div><!-- /rm-right -->
          <!-- RIGHT SIDE -->




        </div><!-- /rm-wrapper -->

      </div><!-- /rm-container -->

    </section>
  </div>

</template>

<script>

import home from './components/book/home.vue'
import resumePage from './components/book/resume-page.vue'
import Portfolio from "./components/book/portfolio.vue";


export default {
  name: 'App',
  data: function (){
    return{
      isActive: false,
      isInactive: true
    }
  },
  components: {
    Portfolio,
    home,
    resumePage
  },
  methods:{
    openedBook: function (){
      this.isActive = true
      this.isInactive = false
    },
    closedBook: function () {
      this.isActive = false
      this.isInactive = true

    }
  }
}

</script>

<style>
@import url("http://fonts.googleapis.com/css?family=Lato:100,300,400,700,900,100italic,300italic,400italic,700italic,900italic");
@import url("http://fonts.googleapis.com/css?family=Alfa+Slab+One|Nixie+One|Raleway:200,800");
@import url("http://fonts.googleapis.com/css?family=Tulpen+One|Sacramento");
/*@import "assets/style.scss";*/
@import "assets/style.css";


</style>
