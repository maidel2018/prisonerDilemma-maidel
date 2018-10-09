# prisonerDilemma-maidel

<!DOCTYPE html>
<html>
<head>
<style>

.button {
    background-color: #008CBA; /* BLUE */
    border: none;
    color: white;
    padding: 50px 120px;
    text-align: center;
    text-decoration: none;
    display: inline-block;
    font-size: 20px;
    margin: 5px 6px;
    cursor: pointer;
	border-radius: 12px;
	

}
.button1:hover {
    box-shadow: 0 12px 16px 0 rgba(0,0,0,0.24),0 17px 50px 0 rgba(0,0,0,0.19);}
.button2:hover { padding: 50px 108px;
 box-shadow: 0 12px 16px 0 rgba(0,0,0,0.24),0 17px 50px 0 rgba(0,0,0,0.19);
 
}
</style>
</head>

<body>

<!--Header-->
<h1 align="center"> Prisoner Number One</h1>
<div style= "width: 100%; min-height: 4vh; background: #000000; float: left;"> </div>

<!--CONFESS AND KEEP QUIET BUTTONS-->
<br>
<button class="button button1" id="demo"  onclick="myFunction2();confessDecision()" >Confess</button>
<br>
<br>
<button style="padding: 50px 108px;"class="button button2" id="demo3"  onclick= "myFunction2();quietDecision()">Keep Quiet</button>

<!--DIV FOR COUNTER AND CURRENT PLAYER-->
<div style="width: 20%; min-height: 50vh; background: #D3D3D3; position: fixed; left: 500px; top:110px;" >
<p>Current Player: </p> 
<div style="width: 100%; height: 50%; background: #D3D3D3;"   >

<p id="demo2">Total Counter: </p>
<p id= "quiet1">Keep Quiet Counter: </p>
<p id="confess1">Confess Counter: </p>
</div>
</div>


<div style="width: 20%; min-height: 50vh; background: #D3D3D3; position: fixed; right: 100px; top:110px;" ><p align="center"><b> Rules:</b> </p>
<ul style="list-style-type: disc">

<li><p> If each plaer confesses, each of them will serve 2 years in prison<p></li>
<li><p> If one player confesses and the other remains silent, the player who confessed will be set free and the player who remained silent serves 3 years</p></li>
<li><p>If both player remain silent, both will serve 1 years</p>

</li></ul></div>


<script>
var count =0;
var quiet =0;
var confess=0;
function quietDecision(){
	quiet=quiet+1;
	document.getElementById("quiet1").innerText = "Keep Quiet Counter: " +quiet;
	
}

function confessDecision(){
	confess=confess+1;
	document.getElementById("confess1").innerText = "Confess Counter: " + confess;
	
}



function myFunction2() {
	count = count+1;
	
    document.getElementById("demo2").innerText = "Total Count: " +count;
	document.getElementById("demo2").innerText = " Total Count: " +count;
	
	
}
</script>



</body>
</html>
