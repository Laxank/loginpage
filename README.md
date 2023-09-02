<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <style>
        body{
            overflow: hidden;
            /* background:linear-gradient(rgb(0, 255, 234), blueviolet); */
     background-color: aliceblue;
           
        }

    .log{
      border: 2px solid rgb(255, 255, 255);
     
      box-shadow: 0 0 20px 0 rgba(0,0,0,0.1);
      border-radius: 30px;
      background-color: white;
      background-position: center;
      align-items: center;
        width: 30%;
        height: 60vh;
        margin-top: 25%;
        margin-left: 50%;
        transform: translate(-50%, -50%);
    }
    .title{
        text-align: center;
        margin: 50px 200px;
        
      line-height: 50px;
        border-radius: 60px;
     

    }
    
    .log form{
        padding: 0 40px;
        box-sizing: border-box;
    }
    form .text_fild{
        margin-top: 50px;
       position: relative;
     border-bottom: 2px solid silver;
       margin: 30px 0;
       

    }
    .text_fild input{
        width: 100%;
   padding: 0 -5px;
        height: 40px;
        font-size: 17px;
        background: none;
      border: none;
      outline: none;
      font-family: system-ui, -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
        
    }
    .text_fild label{
        position: absolute;
        left: 35px;
        top: 50%;
        transform: translate(-50%);
        pointer-events: none;
        color: silver;
        font-size: 17px;
        transition: 0.5s;
    }
    .text_fild span::before{
        content: '';
        position: absolute;
        top: 42px;
        height: 2px;
        left: 0;
        width: 0;
    
     
    }
    
    .text_fild input:focus~label ,.text_fild input:valid~label{
        top: -15px;
        color: rgb(0, 0, 0);
        font-family: system-ui, -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;

    }
    .text_fild input:focus~span::before ,.text_fild input:valid~span::before{
       width: 100%;
   background-color: blueviolet;
  

    }
    .pass{ 
        font-family: system-ui, -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
        margin: 10px 20px;
        margin-bottom: 30px;
    }
    input[type="submit"]{
        width: 100%;
        
        height: 5vh;
        background-color: blueviolet;
        border-radius: 10px;
        font-size: large;
        border: none;
        color: white;
        cursor: pointer;
    }
    input[type="submit"]:hover{
      background-color: rgb(81, 22, 136);
    }
    .signup{
        font-family: system-ui, -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
        text-align: center;
        margin-top: 30px;
    }
    input[type="checkbox"]{
        position: relative;
    }
    </style>
</head>
<body>
    <div class="log">
        <div class="title"><h1>Login</h1></div>
      
       
        <form method="form">
           
            <div class="text_fild">
                <input type="text" required>
                <span></span>
                <label>Usarname</label>
            </div>
            <div class="text_fild">
                <input type="text" required>
                <span></span>
                <label>Password</label>
            </div>
            <div>
                <input type="checkbox" value="remindar"> Remember me
            </div>
            
            <div class="pass">
                <a href="#">forgot password?</a>
            </div>
            <input type="submit" value="Login">
            <div class="signup">
                Don't have an account <a href="signup.html">signup</a>
            </div>
        </form>
    </div>
    
    
</body>
</html>
