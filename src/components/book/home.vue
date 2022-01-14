<template>
  <div class="cover">

    <div class="cover-image-holder">
      <img src="./../../assets/book/images/site/cover.jpg" alt="cover-image">
    </div>

    <h1>{{ title }}</h1>

    <h2>{{ subtitle }}</h2>

    <list-home v-for="list in lists" :key="list.id" v-bind:title="list.title" v-bind:text="list.text"></list-home>

    <a href="javascript:void 0" class="rm-button-open ribbon" v-on:click="$emit('openBook')">
      <span class="ribbon-stitches-top"></span>
      <strong class="ribbon-content">{{ btnName }}</strong>
      <span class="ribbon-stitches-bottom"></span>
    </a>


    <div class="latest-from-blog">
      <h3>{{ bottomText }}
        <a class="button2" href="blog.html">All Posts</a></h3>
      <div class="blog-bar">
        <h2><a href="blog-single.html">{{ linkText }}</a></h2>
      </div>
    </div>

    <aside class="widget widget-twitter">
      <a href="https://twitter.com/envato" class="twitter-link" target="_blank" ></a>
      <div id="twitter-list"></div>
    </aside>

  </div>
</template>

<script>
import listHome from './list-home'


export default {
  name: "home",
  data: function (){
    return {
      title: 'JOHNNY DOE',
      subtitle: 'Freelance UI/UX Designer & writer',
      lists: [
        {title: 'I AM FROM', text: 'EARTH'},
        {title: 'I CREATE', text: 'HTML5 websites'},
        {title: 'I LIKE', text: 'minimalistic design'},
        {title: 'FREELANCE', text: 'Available'},
      ],
      btnName: 'OPEN',
      bottomText: 'LATEST FROM THE BLOG ALL POSTS',
      linkText: 'Runaway A Road Adventure'
    }
  },
  components: {
    listHome
  }

}

</script>

<style scoped>
.cover{
  background-image: url('./../../assets/book/images/site/cover.jpg');
}
</style>