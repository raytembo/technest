<script>

function goToHome() {
     window.location.href = '/home';
  }

    
</script>

<div id="auth">

    <img src="../src/Images/sign_in_back.jpg" alt="sign static" width="50%">

    <div>
        <h3>Welcome Back</h3>
        <input type="email" placeholder="Email" >
        <input type="password" placeholder="Create Password">
        <input type="password" placeholder="Re-enter Password">
        <button on:click={goToHome}>Sign In</button>
        <div id="sign-up">
            <p>Already have an account</p>
            <a href="../signin"><p id="sign-up-button">Sign In</p></a>  
        </div>
    </div>

</div>

<style>
    p{
        color: white;
    }

    #sign-up{
        display: flex;
    }
    #sign-up-button{
        padding-left: 10px;
        color: blue;
       

    }

    form h3{
        color: white;
        font-size: 30px;
        font-weight: 700;
    }

    form{
        width: 50%;
        padding-top: 250px;
        display: flex;
        flex-direction: column;
        align-items: center;
        background-color: black;
    }

    form input{
        padding: 5px;
        margin: 10px;
        border: 1px solid black;
    }

    form button{
        margin:30px;
        padding: 10px;
        background-color: blue;
        color: white;
        border-radius: 10px;
    }

   #auth{
        display: flex;
        justify-content: space-between;
        height: 100vh;
   }

  

   
    
</style>