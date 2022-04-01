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
          <div id="portfolio" class="rm-middle portfolio page">

            <!-- .rm-inner -->
            <div class="rm-inner">


              <!-- .antiscroll-wrap -->
              <div class="antiscroll-wrap">
                <!-- .antiscroll-inner -->
                <div class="antiscroll-inner">




                  <!-- CONTENT -->
                  <div class="content">


                    <h2><span>PORTFOLIO</span></h2>


                    <!--FILTERS-->
                    <ul id="filters">
                      <li class="current"><a href="index.html#" data-filter="*">ALL</a></li>
                      <li><a href="index.html#" data-filter=".design">DESIGN</a></li>
                      <li><a href="index.html#" data-filter=".coding">CODING</a></li>
                      <li><a href="index.html#" data-filter=".logo">LOGO</a></li>
                    </ul>
                    <!--FILTERS-->



                    <!-- PORTFOLIO -->
                    <div class="portfolio-items">



                      <!-- portfolio-item -->
                      <div class="design hentry">
                        <div class="media-box">
                          <img src="./assets/book/images/portfolio/01.jpg" alt="portfolio-post">
                          <div class="mask">
                            <a href="portfolio-item-01.html" class="ajax"></a>
                          </div>
                        </div>
                        <h4>Happy Bear</h4>
                        <p class="category">an illustration work</p>
                      </div>
                      <!-- portfolio-item -->


                      <!-- portfolio-item -->
                      <div class="coding hentry">
                        <div class="media-box">
                          <img src="./assets/book/images/portfolio/03.jpg" alt="portfolio-post">
                          <div class="mask">
                            <a href="portfolio-item-02.html" class="ajax"></a>
                          </div>
                        </div>
                        <h4>Old Guy Superman</h4>
                        <p class="category">illustration by Dave Mottram</p>
                      </div>
                      <!-- portfolio-item -->


                      <!-- portfolio-item - lightbox video -->
                      <div class="coding video hentry">
                        <div class="media-box">
                          <img src="images/portfolio/07.jpg" alt="portfolio-post">
                          <div class="mask">

                            <!-- lightbox - video -->
                            <a href="http://player.vimeo.com/video/37254322?badge=0&amp;color=ffffff" title="Paper by FiftyThree" data-lightbox-gallery="fancybox-item-03" class="lightbox iframe"></a>
                            <!-- lightbox - video -->

                          </div>
                        </div>
                        <h4>Paper by FiftyThree</h4>
                        <p class="category">Lightbox Video</p>
                      </div>
                      <!-- portfolio-item - lightbox video -->


                      <!-- portfolio-item - lightbox image -->
                      <div class="design image hentry">
                        <div class="media-box">
                          <img src="images/portfolio/06.jpg" alt="portfolio-post">
                          <div class="mask">

                            <!-- lightbox - image -->
                            <!--                            <a href="images/portfolio/lightbox-01.jpg" title="Animal with love" data-lightbox-gallery="fancybox-item-01" class="lightbox"></a>-->
                            <!-- lightbox - image -->

                          </div>
                        </div>
                        <h4>Lightbox Image</h4>
                        <p class="category">a booking mobile app</p>
                      </div>
                      <!-- portfolio-item - lightbox image -->


                      <!-- portfolio-item - lightbox soundcloud -->
                      <div class="coding audio hentry">
                        <div class="media-box">
                          <img src="images/portfolio/05.jpg" alt="portfolio-post">
                          <div class="mask">

                            <!-- lightbox - soundcloud -->
                            <!--                            <a href="http://w.soundcloud.com/player/?url=http%3A%2F%2Fapi.soundcloud.com%2Ftracks%2F207988&" title="Soundcloud embed" data-lightbox-gallery="fancybox-item-04" class="lightbox iframe"></a>-->
                            <!-- lightbox - soundcloud -->

                          </div>
                        </div>
                        <h4>Volume 2</h4>
                        <p class="category">Lightbox Soundcloud</p>
                      </div>
                      <!-- portfolio-item - lightbox soundcloud -->


                      <!-- portfolio-item - lightbox gallery -->
                      <div class="logo image hentry">
                        <div class="media-box">
                          <img src="images/portfolio/02.jpg" alt="portfolio-post">
                          <div class="mask">

                            <!-- lightbox - gallery -->
                            <a href="images/portfolio/lightbox-02.jpg" data-lightbox-gallery="fancybox-item-02" class="lightbox" title="Octopus is dangerous!"></a>
                            <a href="images/portfolio/lightbox-04.jpg" data-lightbox-gallery="fancybox-item-02" class="hidden lightbox"></a>
                            <a href="images/portfolio/lightbox-03.jpg" data-lightbox-gallery="fancybox-item-02" class="hidden lightbox" title="Dog have dreams"></a>
                            <!-- lightbox - gallery -->

                          </div>
                        </div>
                        <h4>Lightbox Gallery</h4>
                        <p class="category">Web Design, UI Design</p>
                      </div>
                      <!-- portfolio-item - lightbox gallery -->


                      <!-- portfolio-item - custom url -->
                      <div class="logo url hentry">
                        <div class="media-box">
                          <img src="images/portfolio/10.jpg" alt="portfolio-post">
                          <div class="mask">
                            <a href="http://themeforest.net/user/pixelwars" target="_blank"></a>
                          </div>
                        </div>
                        <h4>Character Sketches</h4>
                        <p class="category">illustration / sketch</p>
                      </div>
                      <!-- portfolio-item - custom url -->


                      <!-- portfolio-item -->
                      <div class="coding hentry">
                        <div class="media-box">
                          <img src="images/portfolio/16.jpg" alt="portfolio-post">
                          <div class="mask">
                            <a href="portfolio-item-03.html" class="ajax"></a>
                          </div>
                        </div>
                        <h4>Cross Browser</h4>
                        <p class="category">an illustration work</p>
                      </div>
                      <!-- portfolio-item -->


                      <!-- portfolio-item -->
                      <div class="design hentry">
                        <div class="media-box">
                          <img src="images/portfolio/14.jpg" alt="portfolio-post">
                          <div class="mask">
                            <a href="portfolio-item-01.html" class="ajax"></a>
                          </div>
                        </div>
                        <h4>404 Page</h4>
                        <p class="category">an illustration work</p>
                      </div>
                      <!-- portfolio-item -->


                      <!-- portfolio-item -->
                      <div class="design hentry">
                        <div class="media-box">
                          <img src="images/portfolio/15.jpg" alt="portfolio-post">
                          <div class="mask">
                            <a href="portfolio-item-02.html" class="ajax"></a>
                          </div>
                        </div>
                        <h4>Rat</h4>
                        <p class="category">an illustration work</p>
                      </div>
                      <!-- portfolio-item -->


                      <!-- portfolio-item -->
                      <div class="logo hentry x2">
                        <div class="media-box">
                          <img src="images/portfolio/11.jpg" alt="portfolio-post">
                          <div class="mask">
                            <a href="portfolio-item-03.html" class="ajax"></a>
                          </div>
                        </div>
                        <h4>Working Dudes</h4>
                        <p class="category">an illustration work</p>
                      </div>
                      <!-- portfolio-item -->



                    </div>
                    <!-- PORTFOLIO -->






                  </div>
                  <!-- CONTENT -->



                </div>
                <!-- .antiscroll-inner -->
              </div>
              <!-- .antiscroll-wrap -->


              <div class="rm-overlay"></div>

            </div><!-- /rm-inner -->
          </div><!-- /rm-middle -->
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

// import HelloWorld from './components/HelloWorld.vue'
// import bodyS from './components/book/bodyS.vue'
import home from './components/book/home.vue'
import resumePage from './components/book/resume-page'


export default {
  name: 'App',
  data: function (){
    return{
      isActive: false,
      isInactive: true
    }
  },
  components: {
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
