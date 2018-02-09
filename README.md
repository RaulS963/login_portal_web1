A simple login page for e-commerce websites, etc.. using HTML,CSS,Bootstrap and javaScript.

==================================================================================================

<!DOCTYPE html>
<html>
<head>
<title>project</title>
<link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap.min.css"/>
<script src="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/js/bootstrap.min.js" ></script>
<style>
.box1{
  height:410px;
  border:5px solid red;
  margin-top:30px;
  border-radius:15px;
  background-color:white;
}
.box2{
  margin-top:30px;
  margin-left:50px;
  height:260px;
  border:5px solid lightgreen;
  border-radius:15px;  
  background-color:white;
}
.heading1{
  margin-top:15px;
  background-color:	#D00000 ;
  color:white;
  height:40px;
  border-radius:10px 10px 0 0;
  padding:6.5px;
  
}
</style>
<script>
function func1(){
  var pass1=document.getElementById("iput1").value;
  var pass2=document.getElementById("iput2").value;
  if(pass1.length==0 || pass2.length==0)
  {
     alert("enter password!");
  }
  else if(pass1==pass2)
    {
      alert("Sign up Successfull");
    }
  else
    {
      alert("password not matching!");
    }
}
function login(){
  window.open("C:\Users\HP\Documents\test1.1.html");
}
</script>
</head>
<body style="background-color:#ccccff;">
<div class="container">
  <div class="row">
  <h1 align="center" style="font-family:cursive; font-size:50px;">Online-Kart</h1>

  </div>
  <div class="row">
    <div class="col-xs-5 box1" >
      <h3 align="center" class="heading1">Sign-Up</h3>
      <br/>
      <div>
        <form>
        <input type="text" class="form-control" placeholder="enter name"/><br/>
        <input type="text" class="form-control" placeholder="email id/phone no"/><br/>
        <input text="text" class="form-control" placeholder="enter username"/>
        <br/>
          <input type="password" class="form-control" placeholder="enter password" autofocus value="" id="iput1"/><br/>
          <input type="password" class="form-control" placeholder="confirm password" autofocus value="" id="iput2"/><br/>
          <button class="btn btn-danger btn-block" onclick="func1()">Sign Up</button> 
        </form>    
      </div>
    </div>
    <!--login box starts-->
    <div class="col-xs-5 box2">
      <h3 align="center">Log-In</h3><br/>
      <div>
        <form>
      <input type="text" class="form-control" placeholder="enter username"/><br/>
      <input type="password" class="form-control" placeholder="password"/><br/>
          <button class="btn btn-success btn-block">Log In</button>
        </form>
      </div>  
    </div>
    
  </div>
</div>

</body>
</html>
