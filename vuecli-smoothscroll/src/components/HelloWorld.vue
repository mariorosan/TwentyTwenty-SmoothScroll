<template>
  <div class="container">
      <nav class="navbar">
        <ul>
          <li><a href="#home">Home</a></li>
          <li><a href="#about">About</a></li>
          <li><a href="#service">Service</a></li>
          <li><a href="#contact">Contact</a></li>
        </ul>
      </nav>
      <section id="home">
        <h1>Welcome to the Home Section</h1>
        <p>This could be your Home section</p>
        <img src="../assets/logo.png" alt="">
      </section>
      <section id="about">
        <h1>Welcome to the About Section</h1>
        <p>This could be your About section</p> 
        <img src="../assets/logo.png" alt="">     
      </section>
      <section id="service">
        <h1>Welcome to the Services Section</h1>
        <p>This could be your Services section</p>
        <img src="../assets/logo.png" alt="">
      </section>
      <section id="contact">
        <h1>Welcome to the Contact section</h1>
        <p>This could be your Contact section</p>
        <img src="../assets/logo.png" alt="">
      </section>
    </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  
}
</script>


<style>
.container {
  width: 100%;
  height: 100%;
}
.navbar {
  position: fixed;
  top: 0;
  z-index: 1;
  display: flex;
  width: 100%;
  height: 50px;
  background: rgba(0,0,0,0.01);
}
.navbar ul {
  display: flex;
  list-style: none;
  width: 100%;
  justify-content: center;
}
.navbar ul li {
  margin: 0 1.5rem;
  padding: 1rem;
}
.navbar ul li a {
  text-decoration: none;
  text-transform: uppercase;
  color: #f4f4f4;
}
.navbar ul li a:hover {
  font-weight: 300;
}
section {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  text-align: center;
  width: 100%;
  height: 100vh;
  scroll-snap-align: center;
}
section h1 {
  font-size: 4rem;
  font-weight: 200;
}
section p {
  margin-top: 20px;
}
section img {
  margin-top: 20px;
  opacity: 0.9;
}
section#home {
  background: linear-gradient(to bottom, #f44881, #ec454f);
  
}
section#about {
  background: linear-gradient(to bottom,#21c8f6,#637bff);
}
section#service {
  background: linear-gradient(to bottom, #ffc73c, #f19a1a);
}
section#contact {
  background: linear-gradient(to bottom, #8b60ed, #b372bd);
}

@media screen and (max-width: 480px) {
  .navbar ul li {
    margin: 0 0.5rem;
    padding: 1rem;
  }
  section h1 {
  font-size: 3rem;
  font-weight: 200;
}
}
</style>
