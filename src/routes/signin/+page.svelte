<script>
    
</script>

<div id="auth">

    <img src="" alt="sign static" width="50%">

    <form action="">
        <h3>Welcome Back</h3>
        <input type="email" placeholder="Email" required>
        <input type="password" placeholder="Password" required>
        <button type="submit">Sign In</button>
        <div id="sign-up">
            <p>Don't Have have an account</p>
            <a href="../signup"><p id="sign-up-button">Sign Up</p></a>  
        </div>
        
    </form>

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
    }

   #auth{
        display: flex;
        justify-content: space-between;
        height: 100vh;
   }

   #auth img{

   }

   
    
</style>