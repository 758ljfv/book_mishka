<template>
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
              <li class="current"><a href="#" data-filter="*">ALL</a></li>
              <li><a href="#" data-filter=".design">DESIGN</a></li>
              <li><a href="#" data-filter=".coding">CODING</a></li>
              <li><a href="#" data-filter=".logo">LOGO</a></li>
            </ul>
            <!--FILTERS-->

            <!-- PORTFOLIO -->
            <div class="portfolio-items">

              <!-- portfolio-item -->
              <div v-for="item in posts"  v-bind:key="item.key" class="hentry" v-bind:class="item.filter">
                <div class="media-box">
                  <img :src="item.img" alt="portfolio-post">
                  <div class="mask">
                    <a href="javascript:void 0" class="ajax"></a>
                  </div>
                </div>
                <h4>{{item.title}}</h4>
                <p class="category">{{item.subtitle}}</p>
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
</template>

<script>
export default {
  name: "portfolio",
  data: function (){
    return{
      posts:[
        { title: 'Happy Bear', subtitle: 'an illustration work', img: require('./../../assets/book/images/portfolio/01.jpg'), filter: 'design'},
        { title: 'Old Guy Superman', subtitle: 'Old Guy Superman', img: require('./../../assets/book/images/portfolio/03.jpg'), filter: 'coding'},
        { title: 'Paper by FiftyThree', subtitle: 'Lightbox Video', img: require('./../../assets/book/images/portfolio/07.jpg'), filter: 'coding video'},
        { title: 'Lightbox Image', subtitle: 'a booking mobile app', img: require('./../../assets/book/images/portfolio/06.jpg'), filter: 'design image'},
        { title: 'Volume 2', subtitle: 'Lightbox Soundcloud', img: require('./../../assets/book/images/portfolio/05.jpg'), filter: 'coding audio'},
        { title: 'Lightbox Gallery', subtitle: 'Web Design, UI Design', img: require('./../../assets/book/images/portfolio/02.jpg'), filter: 'logo image'},
        { title: 'Character Sketches', subtitle: 'illustration / sketch', img: require('./../../assets/book/images/portfolio/10.jpg'), filter: 'logo url'},
        { title: 'Cross Browser', subtitle: 'an illustration work', img: require('./../../assets/book/images/portfolio/16.jpg'), filter: 'coding'},
        { title: '404 Page', subtitle: 'an illustration work', img: require('./../../assets/book/images/portfolio/14.jpg'), filter: 'design'},
        { title: 'Rat', subtitle: 'an illustration work', img: require('./../../assets/book/images/portfolio/15.jpg'), filter: 'design'},
        { title: 'Working Dudes', subtitle: 'an illustration work', img: require('./../../assets/book/images/portfolio/11.jpg'),filter: 'logo x2'},

      ]
    }
  }
}
</script>

<style scoped>

</style>