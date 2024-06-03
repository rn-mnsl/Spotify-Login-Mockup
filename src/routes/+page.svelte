<script>
    let username = '';
    let password = '';
 </script>
 
 <style>

    @import url('https://fonts.googleapis.com/css2?family=Poppins:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&display=swap');

    :global(body) {
       margin: 0;
       font-family: 'Poppins', sans-serif;
       background: linear-gradient(to bottom, #2C2B2B, #000000);
       color: white;
    }

    .container {
       margin-top: 5rem;
       margin-bottom: 5rem;
       padding: 3rem;
       display: flex;
       justify-content: center;
       align-items: center;
       height: 100vh;
    }
 
    .login-box {
       background: #121212;
       padding: 3rem;
       border-radius: 10px;
       box-shadow: 0 4px 12px rgba(0, 0, 0, 0.5);
       text-align: center;
       width: 500px;
    }
 
    .login-box h2 {
       margin-bottom: 2rem;
    }
 
    .input-group {
    margin-bottom: 1.5rem;
    margin-top: 1.5rem;
    display: flex;
    flex-direction: column;
    align-items: center;
  }
 
    .input-group label {
       font-size: 0.9rem;
       align-self: flex-start;
       margin-left: 4.5rem;
    }
 
    .input-group input {
       width: 65%;
       padding: 0.8rem;
       border: 2px solid white;
       border-radius: 4px;
       margin-top: 0.5rem;
       background-color: transparent;
       display: block;
       color: white;
    }
 
    .login-button {
       font-family: 'Poppins', sans-serif;
       font-weight: bold;
       font-size: 16px;
       background: #1db954;
       border: none;
       border-radius: 50px;
       color: black;
       padding: 0.8rem 2rem;
       cursor: pointer;
       margin-top: 1rem;
       width: 71%;
    }
 
    .checkbox-group {
       display: flex;
       justify-content: space-between;
       align-items: center;
       margin-top: 1rem;
       font-size: 0.9rem;
       margin-left: 4rem;
    }
 
    .social-login {
       margin-top: 1rem;
    }
 
    .social-login button {
      font-family: 'Poppins', sans-serif;
      background: transparent; 
      border: 2px solid white; 
      border-radius: 70px;
      color: white; 
      padding: 0.6rem 2rem;
      cursor: pointer;
      margin: 0.5rem 0;
      width: 350px; 
   }
 
    .forgot-password {
       display: block;
       margin-top: 2rem;
       margin-bottom: 2rem;
       font-size: 0.9rem;
       text-decoration: none;
       color: #1db954;
    }

    .dont-have-account { 
       display: block;
       margin-top: 2rem;
       margin-bottom: 2rem;
       font-size: 0.9rem;
       text-decoration: none;
       color: whitesmoke;
    }

    .logo { 
        width: 50px; 
        height: auto;
    }
    
    .social-logo-google { 
        height: 20px;
        vertical-align: middle;
        margin-right: 35px;
        margin-left: -35px; 
    }

    .social-logo-facebook { 
        height: 20px;
        vertical-align: middle;
        margin-right: 30px;
        margin-left: -20px;
    }

    .social-logo-apple { 
        height: 20px;
        vertical-align: middle;
        margin-right: 40px;
        margin-left: -40px; 
    }

    .line {
    width: 100%; 
    border: none;
    border-top: 1px solid white; 
    margin: 20px auto; 
  }

  
 </style>
 
 <div class="container">
    <div class="login-box">
       <img class="logo" src="/spotify-logo.png"  alt="Spotify logo">
       <h2>Login to Spotify</h2>
       <div class="social-login">

        <button>
            <img class= "social-logo-facebook" src="/facebook-logo.png" alt="Facebook logo">
            Continue with Facebook</button>

        <button>
            <img class= "social-logo-google" src="/google-logo.png" alt="Google logo">Continue with Google</button>

        <button>
            <img class = "social-logo-apple" src="/apple-logo.png" alt="Apple Logo">Continue with Apple</button>
        </div>

        <hr class="line">

       <div class="input-group">
          <label for="email">Email address or username</label>
          <input id="username" type="text" bind:value={username}>
       </div>

       <div class="input-group">
          <label for="password">Password</label>
          <input id="password" type="password" bind:value={password}>
       </div>

       <div class="checkbox-group">
          <div>
             <input type="checkbox" id="remember" name="remember">
             <label for="remember">Remember me</label>
          </div>
       </div>

       <button class="login-button">Log In</button>
       <a href="https://fonts.google.com/selection/embed" class="forgot-password" text-decoration= "Underline"><u>Forgot password?</u></a>

       <hr class="line">

       <a href="https://www.spotify.com/ph-en/signup?flow_ctx=69dc4a54-5356-4bbb-9027-ddd2f41e8c6c%3A1717433310" class="dont-have-account" text-decoration= "Underline">Don't have an account? <strong><u>Sign up for Spotify</u></strong></a>
    </div>
 </div>
 