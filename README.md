# currency-convertor
This web application will convert the US dollor to appropriate types
<html>
<title>currency convertor</title>
<style type="text/css">
body{
	background-color: #ff6666;
}
.s1{
	height:130%;
width: 50%;
padding: 10px;

background-color: #27E573;
border-radius: 20px;
}
.s2{
	text-align: left;
	height: 50%;
	width: 40%;
	font-style: italic;
}
.s3{
	background-color: #cccccc;
	height: 10%;
	width: 30%;
	border-radius: 10px;
	cursor: pointer;
	font-size: 20px;
	color: #ffffff


}
.s4{
	width: 100%;
	height: 10%;
}
img {
  border-radius: 130%;
}
.s5{
background-color: #ff9999;
height: 5%;
width: 40%;
padding: 10px;

}
</style>
<body>
	<br>
	<br>
	

	<center>
	<section class="s1">
		<img src="rupee.jpg" alt="Avatar" style="height:100px" >

		<div>
	<form name="f1" onsubmit="return compute()" method="post">
		<br>
		<br>
		
		
		<center><h1>CURRENCY CONVERTOR</h1></center>
		<br>
        <div class="s2">
		<input type="text" placeholder="enter US dollor" name="n1" class="s4">

		<br>
		
		<br>
		<input type="radio" name="r1" value="india">INDIA<br><br>
		<input type="radio" name="r1" value="australia">AUSTRALIA<br><br>
		<input type="radio" name="r1" value="china">CHINA<br><br>
		<input type="radio" name="r1" value="japan">JAPAN<br><br>
		<input type="radio" name="r1" value="england">ENGLAND<br><br>
		<input type="radio" name="r1" value="brazil">BRAZIL<br><br>
		<input type="radio" name="r1" value="spain">SPAIN<br><br>
	</div>
	
		<input type="submit" value="compute" class="s3" onmouseover="fun1(this)" onmouseout="fun2(this)"><br><br>
		<div class="s5">
		<h2 id="demo"></h2>
    </div>
	
		</form>
	</div>
</section>
</center>
		

<script type="text/javascript">
function fun1(x){
	x.style.background="#1a0000"
}
function fun2(x){
	x.style.background="#cccccc";
}
function compute(){
	var n1=document.forms["f1"]["n1"].value;
	var r1=document.forms["f1"]["r1"].value;
	if(r1==""){
		alert("press any one");
		return false;
	}
    if(r1=="india"){
    	document.getElementById("demo").innerHTML=n1*71.92;
         return false;
  
    
    }
    if(r1=="australia"){
    	document.getElementById("demo").innerHTML=n1*1.39;
         return false;
  
    
    }
    if(r1=="china"){
    	document.getElementById("demo").innerHTML=n1*6.91;
           return false;
  
    
    }
    if(r1=="japan"){
    	document.getElementById("demo").innerHTML=n1*113.44;

          return false;
  
    }
    if(r1=="england"){ return false;
  
    	document.getElementById("demo").innerHTML=n1*0.79;
         return false;
  
    
    }
    if(r1=="spain"){
    	document.getElementById("demo").innerHTML=n1*0.88;
         return false;
  
    
    }
    if(r1=="india"){
    	document.getElementById("demo").innerHTML=n1*71.92;
         return false;
  
    
    }
   
}
</script>
</body>
</html>
