<template>
<section class="loggin">
<div class="full-page">
    <div class="navvbar">
        <div>
            <a href="website.html">Seek Coding</a>
        </div>
        <nav>
            <ul id="MenuItems">
                <li><a href="#">Home</a></li>
                <li><a href="#">About</a></li>
                <li><a href="#">Services</a></li>
                <li><a href="#">Contact</a></li>
                <li><button class='logginbtn' onclick="document.getElementById('login-form').style.display='block'" style="width:auto;">Login</button></li>
                
            </ul>
        </nav>
    </div>
    <div id="loggin-form" class="loggin-page">
        <div class="forrm-box">
            <div class="buutton-box">
                <div id="btn"></div>
                <button type="button" onclick="login()" class="toggle-bttn">Log In</button>
                <button type="button" onclick="register()" class="toggle-bttn">Register</button>
            </div>
            <form id="login" class="input-group-login">
                <input type="text" class="input-fielld" placeholder="Email Id" required>
                <input type="password" class="input-fielld" placeholder="Enter Password" required>
                <input type="checkbox" class="check-boxx" ><span>Remember Password</span>
                <button type="submit" class="submit-bttn">Log in</button>
            </form>
            <form id="register" class="input-group-register">
                <input type="text" class="input-fielld" placeholder="First Name" required>
                <input type="password" class="input-fielld" placeholder="Last Name" required>
                <input type="email" class="input-fielld" placeholder="Email Id" required>
                <input type="password" class="input-fielld" placeholder="Enter Password" required>
                <input type="password" class="input-fielld" placeholder="Confirm Password" required>
                <input type="checkbox" class="check-boxx"><span>I agree to the terms and conditions</span>
                <button type="submit" class="submit-bttn">Register</button>
            </form>

        </div>

    </div>
</div>
</section>
</template>
<script>
/*

var x=document.getElementById('login');
var y=document.getElementById('register');
var z=document.getElementById('btn');
function register(){
    x.style.left='-400px';
    y.style.left='50px';
    z.style.left='110px';

}
function login(){
    x.style.left='50px';
    y.style.left='450px';
    z.style.left='0px';

}
var modal = document.getElementById('login-form');
window.onclick = function(event){
    if(event.target == modal)
    {
        modal.style.display = "none";
    }
}
*/
</script>


<style>
.loggin{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

.full-page{
    height: 100%;
    width: 100%;
    background-image: linear-gradient(rgba(0,0,0,0.4),rgba(0,0,0,0.4)),url("../assets/camping.jpg");
    background-position: center;
    background-size: cover;
    position: absolute;
}

.navvbar{
    display: flex;
    align-items: center;
    padding: 20px;
    padding-left: 50px;
    padding-right: 30px;
    padding-top: 50px;
}
nav{
    flex: 1;
    text-align: right;
}

nav ul{
    display:inline-block;
    list-style: none;
}
nav ul li{
    display:inline-block;
    margin-right: 70px;
}

nav ul li a {
    text-decoration: none;
    font-size: 20px;
    color: white;
    font-family: sans-serif;
}

nav ul li button{
    font-size: 20px;
    color:white;
    outline: none;
    border: none;
    background: transparent;
    cursor: pointer;
    font-family: sans-serif;
}

nav ul li button:hover{
    color: aqua;
}

nav ul li a:hover{
    color: aqua;

}

a{
    text-decoration: none;
    color: palevioletred;
    font-size: 28px;
}

#loggin-form{
    display: none;
}

.forrm-box{
    width: 380px;
    height:480px;
    position: relative;
    margin: 2% auto;
    background: rgba(0,0,0,0.3) ;
    padding: 10px;
    overflow: hidden;
}

.buutton-box{
    width: 220px;
    margin: 35px auto;
    position: relative;
    box-shadow: 0 0 20px 9px #ff61241f;
    border-radius: 30px;
}

.toggle-bttn{
    padding:10px 30px;
    cursor: pointer;
    background: transparent;
    border: 0;
    outline: none;
    position: relative;
}
#btn{
    top: 0;
    left: 0;
    position: absolute;
    width: 110px;
    height: 100%;
    background: #F3C693;
    border-radius: 30px;
    transition: .5s;
}

.input-group-login{
    top: 150px;
    position: absolute;
    width: 280px;
    transition: .5s;
}

.input-group-register{
    top: 120px;
    position: absolute;
    width: 280px;
    transition: .5s;
}

.input-fielld{
    width:100%;
    padding: 10px 0;
    margin: 5px 0;
    border-left: 0;
    border-top: 0;
    border-right: 0;
    border-bottom: 1px solid #999;
    outline: none;
    background: transparent;
}

.submit-bttn{
    width:85%;
    padding: 10px 30px;
    cursor: pointer;
    display: block;
    margin: auto;
    background: #F3C693;
    border: 0;
    outline: none;
    border-radius: 30px ;
}

.check-boxx{
    margin:30px 10px 34px 0;
}

span{
    color: #777;
    font-size: 12px;
    bottom: 68px;
    position: absolute;
}

#login{
    left:50px;
}

#login-input{
    color: white;
    font-size: 15;
}

#register{
    left:450px;
}

#register input{
    color: white;
    font-size: 15;
}


</style>