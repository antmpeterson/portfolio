<template>
<div class = "hello">



<nav>
  <ul>
    <li><a href="#section-1">About</a></li>
    <li><a href="#section-2">Education</a></li>
    <li><a href="#section-3">Projects</a></li>
    <li><a href="#section-4">Github</a></li>
    <li><a href="#section-5">Contact Me</a></li>
    
  </ul>
</nav>
<div class = "content">
<header>
  {{ msg }}
</header>
<main>
  <section id="section-1">
    <h1>About</h1>
    <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit. Officiis, blanditiis expedita? Earum eligendi pariatur quaerat quos expedita ab quibusdam ratione veniam in, mollitia fuga repudiandae?</p>
  </section>
  <section id="section-2">
    <h1>Education</h1>
    <p>Ratione nulla nam, ipsa dignissimos corrupti veniam nostrum, laudantium asperiores sequi numquam placeat velit voluptate in praesentium non labore unde incidunt laborum maxime quae magni.</p>
  </section>
  <section id="section-3">
    <h1>Projects</h1>
    <p>Soluta quibusdam ad nostrum vel voluptate delectus sequi dolores quia quaerat officia corrupti, aperiam fugit facere debitis repudiandae praesentium sapiente inventore repellendus, nemo commodi alias!</p>
  </section>
  <section id="section-4">
    <h1>Github</h1>
    <p>Aliquid aliquam magnam ducimus similique obcaecati, unde exercitationem laborum incidunt, quas in ipsum inventore nostrum? Blanditiis optio cumque earum iste odio! Alias sint accusamus repudiandae.</p>
  </section>
  <section id="section-5">
    <h1>Contact Me</h1>
    <p>Officia ipsum fugit iure eaque quisquam error tempore earum enim illum, delectus officiis incidunt corrupti aliquid nam quas perspiciatis eveniet doloremque quod labore? Doloremque, ipsum?</p>
  </section>
</main>
<footer>
    &copy;2019 Peterson 

</footer>
</div>


</div>

</template>

 
<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  }
}

</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style >
html {
  scroll-behavior: smooth;
  
}
.content, nav{
  height: 100vh;

}
.content{
  width: calc(100vw - 160px);
  height: fit-content;
  margin-left: 160px;
}
header {
  grid-column: 1 / 3;
  background: #455A64;
  color: white;
  padding: 4rem;
  text-align: center;
  font-size: 50px;
  
}
nav {
  list-style-type: none;
  position: fixed;
  top: 0px;
  left: 0px;
  background: #37474F;
  
  width: 160px; /* 0 width - change this with JavaScript */
  
  
  overflow-x: hidden; /* Disable horizontal scroll */
  padding-top: 20px;
  padding-bottom: 20px;
  padding-left: 0;
  
}
nav ul {
  list-style: none;
  margin: 0;
  padding: 0;
  
}
ul {
  position: fixed; /* Stay in place */
  top: 50%;
  width: 160px;
  transform: translate(0%,-50%);
}
/* Only stick if you can fit */
@media (max-height: 300px) {
  nav ul {
    position: sticky;
    top: 0;
  }
}
nav li a {
  display: block;
  padding: 8px 16px;
  color: white;
  text-decoration: none;
}
nav li a:hover {
  background: black;
}
main {
  text-align: left;
  margin-left: 45px;
}
section {
  padding: 2rem;
  margin: 0 0 2rem 0;
}
footer {
  grid-column: 1 / 3;
  background: #455A64;
  color: white;
  padding: 4rem;
  text-align: center;
  font-size: 20px;
}
</style>
