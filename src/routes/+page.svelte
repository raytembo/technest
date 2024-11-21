<script>

  function goToSigninPage() {
     window.location.href = '/signin';
  }

  function goToSignupPage() {
     window.location.href = '/signup';
  }

</script>


<nav>
  <a href="/"><img src="./src/Images/technest.png" alt="logo" id="logo" width="100" height="100"></a>
  <div id="navlinks">
    <a href="/">Home</a>
    <a href="/Cart">Cart</a>
    <a href="/Blog">Blog</a>
    <a href="/profile">Profile</a>
    <a href="/faq">FAQ</a>
    <a href="/about">About Us</a>
  </div>
  <div id="register">
    <button on:click={goToSigninPage}>
      Sign in
    </button>

    <button on:click={goToSignupPage}>
      Sign Up
    </button>

  </div>
</nav>

<div id="hero">
    <div id="hero-text">
        <h1>
          Welcome to TechNest
        </h1>
    
        <h3>
          Your one-stop shop for the latest tech gadgets, 
          accessories, 
          and smart solutions! At Tech Nest, 
          we bring innovation to your doorstep, 
          offering unbeatable deals and cutting-edge technology to enhance your lifestyle. 
          Shop smarter, live better—only at Tech Nest.
        </h3>

        <button>
          Get Started
        </button>
    </div>

    <div>
      <img src="../src/Images/headphone.jpg" alt="hero" width="80%" height="60%" id="hero-img">
    </div>
</div>

<footer>
  Tech nest 2024
</footer>

<style>

  nav{
    display: flex;
    justify-content: space-between;
    align-items: center;
    height: 80px;
  }
  #navlinks a{
    padding: 5px;
    font-weight: 600;
  }
  #navlinks a:hover{
    color: blue;
  }

  #hero-img{
    margin-left: 150px;
    margin-right: 100px;
    border-radius: 30px;
    filter: grayscale(50%);
    transition: filter 0.5s ease, transform 0.5s ease-in-out;
  }
  #hero-img:hover{
    filter: grayscale(0%);
    
  }
  #register{
    margin-right: 30px;
  }
  #register button{
    margin: 5px;
    padding: 10px;
    background-color: blue;
    color: white;
    border-radius: 30px;
  }
 #hero{
    display: flex;
    height: 90vh;
 }
 #hero h1{
    font-size: 40px;
    font-weight: 800;
 }
 #hero-text{
    display: flex;
    flex-direction: column;
    justify-content: center;
    width: 80%;
    padding-left: 30px;
 }
 #hero-text button{
    margin-top: 10px;
    padding: 10px;
    background-color: blue;
    color: white;
    border-radius: 30px;
    transition: all 0.5s ease, transform 0.5s ease-in-out;
 }
 #hero-text button:hover{
   background-color: white;
   color: blue;
   border: 1px solid blue;
 }
 
 footer{
   text-align: center;
 }

</style>