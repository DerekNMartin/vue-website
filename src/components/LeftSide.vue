<template>
  <div class="left-side">
    <div class="content">
      <div class="logo">
        <svg 
          version="1.1"
          xmlns="http://www.w3.org/2000/svg" 
          xmlns:xlink="http://www.w3.org/1999/xlink" 
          x="0px" 
          y="0px"
          width="40%" 
          viewBox="0 0 285.333 346.667" 
          enable-background="new 0 0 285.333 346.667"
          xml:space="preserve">
          <polyline 
            fill="none" 
            stroke="#FFFFFF" 
            stroke-width="40" 
            stroke-miterlimit="10"
            points="264,294 264,49 142.274,171.561 21.072,49 21.667,294.12 106.538,204.555 ">
            <animate attributeName="stroke"
                    attributeType="XML"
                    from="#ecf0f1"
                    to="#2ecc71"
                    dur="20s"
                    values="#ecf0f1; #2ecc71; #e74c3c; #9b59b6; #f1c40f; #3498db; #ecf0f1"
                    keyTimes="0; 0.15; 0.3; 0.45; 0.6; 0.75; 1"
                    repeatCount="indefinite"
            />
          </polyline>
        </svg>
      </div>
      <div class="intro">
        <h1>Derek Martin</h1>
        <p>Front-End developer at <a href="http://bioconnect.com">BioConnect</a>.</p>
        <p>Honours Digital Media graduate.</p>
        <p>Based in Toronto.</p>
      </div>
      <footer>
        <a target="_blank" href="https://www.instagram.com/derekmart.in/">
          <i class="fa fa-instagram" aria-hidden="true"></i>
        </a>
        <a target="_blank" href="https://twitter.com/_DerekMartin">
          <i class="fa fa-twitter" aria-hidden="true"></i>
        </a>
        <a target="_blank" href="https://github.com/DerekNMartin">
          <i class="fa fa-github" aria-hidden="true"></i>
        </a>
        <a target="_blank" href="https://codepen.io/derekmartian/">
          <i class="fa fa-codepen" aria-hidden="true"></i>
        </a>
      </footer>
    </div>
  </div>
</template>

<script>
export default {
  name: 'LeftSide',
  data () {
    return {
    }
  }
}
</script>
<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  .content {
    margin-top: 30%;
  }
  .left-side {
    position: absolute;
    width: 50%;
    left: 0;
  }
  .logo {
    margin: 0 auto;
    width: 33%;
  }
  .intro {
    font-family: 'Inconsolata', Helvetica, Arial, sans-serif;
  }
  a {
    transition: all 1000ms;
    color: #555555;
    text-decoration-skip: ink;
    text-decoration-color: #2ecc71;
  }
  a:hover {
    color: #2ecc71;
  }
  a i {
    padding: 0 0.5em;
  }
  footer a {
    border: none;
  }
</style>