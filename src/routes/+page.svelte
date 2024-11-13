<script>

  function goToSigninPage() {
     window.location.href = '/signin';
  }

  function goToSignupPage() {
     window.location.href = '/signup';
  }

</script>


<nav>
  <img src="./src/Images/technest.png" alt="logo" id="logo" width="100" height="100">
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
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Perspiciatis,
          iure excepturi tempora commodi totam voluptas 
          beatae exercitationem modi aut iusto cum nesciunt nisi 
          dolore praesentium cumque vitae! Rerum, consequuntur animi!   
        </h3>

        <button>
          Get Started
        </button>
    </div>

    <div>
      <img src="" alt="hero">
    </div>
</div>

<h3 id="todays">Today's Offers</h3>
   
<div>
 
  <div>
     <img src="" alt="product name">
     <h3>Product Name</h3>
     <p>Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
     <h4>$300</h4>
  </div>
</div>

<div>
    <div>
      <img src="" alt="more detailed product">
        <p>
          Lorem ipsum dolor sit amet consectetur adipisicing elit. 
          Repudiandae
          nemo nisi ullam natus vitae cumque quos
          illum facilis quis cupiditate similique ea quisquam nostrum iusto, sint ab et sed voluptas!
        </p>
      <h2>$499 <em>Only</em></h2>
    </div>
</div>

<h3 id="todays">Our Products</h3>

<div>
    <div>
      <img src="" alt="product name">
      <h3>Product Name</h3>
      <p>Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
      <h4>$300</h4>
    </div>
    <button>
      View More
    </button>
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
 }
 #hero h1{
  font-size: 40px;
  font-weight: 800;
 }
 #hero-text{
  width: 60%;
  padding: 30px;
 }
 #hero-text button{
    margin: 10px;
    padding: 10px;
    background-color: blue;
    color: white;
    border-radius: 30px;
 }

 #todays{
  font-size: 20px;
  font-weight: 800;
  text-align: center;
 }


</style>