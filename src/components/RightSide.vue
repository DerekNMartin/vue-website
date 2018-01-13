<template>
  <div class="right-side" v-bind:style="{ 'background-color': randomColor }">
    <div class="content">
      <h1>Projects</h1>
      <hr>
      <ul>
        <li>
          <h3>
            <a 
              @mouseover="randomizeColor"
              @mouseleave="resetColor"
              href="movies.html">Movie List</a>
          </h3>
          <p class="date">Summer 2017 [Vue.js web app]</p>
        </li>        
        <li>
          <h3>
            <a @mouseover="randomizeColor"
               @mouseleave="resetColor"
               href="time.html">Time</a>
          </h3>
              <p class="date">July 2015 - [web app]
        <li>
          <h3>
            <a @mouseover="randomizeColor"
               @mouseleave="resetColor" 
               href="https://codepen.io/derekmartian/pen/YqaJzY">Primordial Soup</a>
          </h3>
          <p class="date">2016 - present [class project]</p>
        </li>    
        <li>
          <h3>
            <a @mouseover="randomizeColor"
               @mouseleave="resetColor"
               href="http://dmstudents.ca/">Digital Media Student Association</a>
          </h3>
          <p class="date">2014 - present [website]</p>
        </li>    
        <li>
          <h3>
            <a @mouseover="randomizeColor"
               @mouseleave="resetColor"
               href="design">Graphic Design</a>
          </h3>
          <p class="date">2014 - present [Freelance]</p>
        </li>
        <li>
          <h3>
            <a @mouseover="randomizeColor"
               @mouseleave="resetColor" 
               href="http://dmgallery.apps01.yorku.ca/">AMPD's Digital Media Gallery</a>
          </h3>
          <p class="date">January 2016 - May 2016 [website]</p>
        </li>
        <li>
          <h3>
            <a @mouseover="randomizeColor"
               @mouseleave="resetColor" 
               href="https://medium.com/@_DerekMartin/redesigning-presto-24e7960c8ecd#.dsq7l9ded">Redesigning Presto</a>
          </h3>
          <p class="date">Summer 2016 [case study]</p>
        </li>
        <li>
          <h3>
            <a @mouseover="randomizeColor"
               @mouseleave="resetColor" 
               href="couchCosmos">Couch Cosmos</a>
          </h3>
          <p class="date">October 2014 - [installation]</p>
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: 'RightSide',
  data () {
    return {
      randomColor: 'rgba(0,0,0,0.87)',
    }
  },
  methods: {
    resetColor() {
      this.randomColor = "rgba(0,0,0,0.87)"
    },
    randomizeColor() {
      const colors = [
        "#16a085",
        "#27ae60",
        "#2980b9",
        "#8e44ad",
        "#f39c12",
        "#d35400",
        "#c0392b"
      ]
      const _randomNumber = (Math.floor(Math.random() * colors.length));
      let _randomColor = colors[_randomNumber];
      this.randomColor = _randomColor;
    },
  },
}
</script>
<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  h3 {
    margin-bottom: 0;
    font-weight: 400;
  }
  ul, li {
    list-style: none;
    padding: 0.5em 0;
  }
  a {
    color: #FFF;
    text-decoration: none;
  }
  a:hover {
    text-decoration: underline;
    text-decoration-skip: ink;
  }
  a i {
    padding: 0 0.5em;
  }
  footer a {
    border: none;
  }
  hr {
    width: 80%;
  }
  .content {
    margin-top: 10%;
  }
  .right-side {
    transition: all 1000ms;
    color: #FFF;
    height: 100%;
    background-color: rgba(0,0,0,0.87);
    position: absolute;
    width: 50%;
    right: 0;
  }
  .logo {
    margin: 0 auto;
    width: 33%;
  }
  .date {
    color: #666666;
    margin: 0; 
    font-family: 'Inconsolata', Helvetica, Arial, sans-serif;
    font-size: 0.8em;
  }
</style>