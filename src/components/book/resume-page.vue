<template>
  <div id="resume" class="rm-back page">

    <!-- .antiscroll-wrap -->
    <div class="antiscroll-wrap">
      <!-- .antiscroll-inner -->
      <div class="antiscroll-inner">

        <!-- CONTENT -->
        <div class="content">


          <h2><span>{{ title }}</span></h2>

          <h4 class="about-text">{{ about }}</h4>

          <h3><span>{{ subtitle }}</span></h3>

          <!-- EMPLOYMENT -->
          <div class="history-group">

            <div v-for="item in history" v-bind:key="item.key" class="history-unit">
              <h4 class="work-time">{{item.date}}</h4>
              <div class="work-desc">
                <h4>{{item.title}}</h4>
                <h5>{{item.inc}}</h5>
                <p>{{item.text}}</p>
              </div>
            </div>

          </div>
          <!-- EMPLOYMENT -->



          <h3><span>{{subtitle2}}</span></h3>

          <!-- EDUCATION -->
          <div class="history-group">

            <div v-for="item in educations" v-bind:key="item.key" class="history-unit">
              <h4 class="work-time">{{item.date }}</h4>
              <div class="work-desc">
                <h4>{{item.title}}</h4>
                <h5>{{item.inc}}</h5>
                <p>{{item.text}}</p>
              </div>
            </div>

          </div>
          <!-- EDUCATION -->



          <!-- DOWNLOAD BUTTON -->
          <div class="launch">
            <a href="javascript:void 0" class="btn">DOWNLOAD</a>
          </div>
          <!-- DOWNLOAD BUTTON -->



          <h3><span>{{subtitle3}}</span></h3>

          <!-- DEV SKILLS -->
          <div class="skill-group">

            <!-- .skill-unit -->
            <div v-for="item in skills" v-bind:key="item.key" v-bind:v-text="item" class="skill-unit">
              <h4>{{item}}</h4>
              <div class="bar" data-percent="100">
                <div class="progress"></div>
              </div>
            </div>
            <!-- .skill-unit -->

          </div>
          <!-- DEV SKILLS -->


          <h3><span>{{subtitle4}}</span></h3>

          <!-- DESIGN SKILLS -->
          <div class="skill-group">

            <!-- .skill-unit -->
            <div v-for="item in design_skills" v-bind:key="item.key" class="skill-unit">
              <h4>{{item}}</h4>
              <div class="bar" data-percent="90">
                <div class="progress"></div>
              </div>
            </div>
            <!-- .skill-unit -->

          </div>
          <!-- DESIGN SKILLS -->




          <h3><span>{{subtitle5}}</span></h3>


          <!-- TESTIMONIALS -->
          <div class="testo-group">
            <!-- Testimonial -->
            <div v-for="item in testimonials" v-bind:key="item.key" v-bind:img="item.img" class="testo">
              <img :src="item.img" alt="someone">
              <div class="text">
                <h4>{{item.text}} <span>{{item.subtitle}}</span></h4>
                <p>{{item.text}}</p>
              </div>
            </div>
            <!-- Testimonial -->
          </div>
          <!-- TESTIMONIALS -->



          <h3><span>{{ subtitle6 }}</span></h3>

          <!-- SERVICES -->
          <div class="service-group">

            <!-- service -->
            <div v-for="item in services" v-bind:key="item.key" class="service">
              <i class="icon-laptop"></i>
              <h4>{{item.title}}</h4>
              <p>{{item.text}}</p>
            </div>
            <!-- service -->
          </div>
          <!-- SERVICES -->
        </div>
        <!-- CONTENT -->

      </div>
      <!-- .antiscroll-inner -->
    </div>
    <!-- .antiscroll-wrap -->

    <div class="rm-overlay"></div>
  </div>
</template>

<script>
export default {
  name: "resume-page",
  data: function (){
    return{
      title: 'RESUME',
      about: 'I am a theoretical physicist developed the general theory of relativity, effecting a revolution in physics.',
      subtitle: 'EMPLOYMENT',
      history:[
        { title: 'Lead UX Designer', date: 'since 2011', inc: 'Apple Inc.', text: 'Worked in so many projects for best clients around the world and i get so many experiences based on my job.' },
        { title: 'Level Designer', date: '2007 - 2011', inc: 'Crytek Inc.', text: 'Also i have designed levels of some cool games everyone plays.' },
        { title: 'Web Developer', date: '2002 - 2007', inc: 'Creative Agency', text: 'Worked in so many projects for best clients around the world.' },
      ],
      subtitle2: 'EDUCATION',
      educations:[
        { title: 'Phd Computer Science', date: '2000 - 2002', inc: 'MIT', text: 'Studied Phd. in MIT on Computer Science.' },
        { title: 'Physics', date: '1996 - 2000', inc: 'Princeton University', text: 'I get my Bachelor Degree in Princeton University.' }
      ],
      subtitle3: 'DEVELOPMENT SKILLS',
      skills:[
        'HTML5',
        'CSS3',
        'jQuery',
        'Wordpress',
      ],
      subtitle4: 'DESIGN SKILLS',
      design_skills:[
          'Fireworks',
          'Photoshop',
          'Illustrator'
      ],
      subtitle5: 'TESTIMONIALS',
      testimonials:[
        { title: 'Albert Einstein', img: require('./../../assets/book/images/site/testo-01.jpg'), subtitle: 'CEO / Gravity Inc.', text: 'He is a great and hardworking guy. I am so proud of i have him as my asistant. He helped me so much.' },
        { title: 'Walter White', img: require('./../../assets/book/images/site/testo-02.jpg'), subtitle: 'Chemist / Freelancer', text: 'He was a great co-worker and a friend. I would\'t be where i am without his support.' },
        { title: 'Dexter Morgan',img: require('./../../assets/book/images/site/testo-03.jpg'), subtitle: 'Lab Geek / Miami Metro', text: 'He is ok.' },
      ],
      subtitle6: 'SERVICES',
      services:[
        { title: 'Web Design', img: require('./../../assets/book/images/site/testo-01.jpg'),text: 'I design super cool websites. It is a long established fact that a reader will be distracted by the readable content.' },
        { title: 'Mobile Development', img: require('./../../assets/book/images/site/testo-02.jpg'),text: 'I can develop iOS and Android apps. It is a long established fact that a reader will be distracted by the readable content.' },
        { title: 'Social Media', img: require('./../../assets/book/images/site/testo-02.jpg'),text: 'I am a social media expert. It is a long established fact that a reader will be distracted by the readable content.\n' +
              '\n' +
              'PORTFOLIO\n' +
              'ALLDESIGNCODINGLOGO\n' }

      ],
    }
  }
}
</script>

<style scoped>

</style>