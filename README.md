# index.htmlcellulare
<html>
<head>
<meta name="viewport" content="width=device-width, initial-scale=1">
<style>
body {
  font-family: 'Lato', sans-serif;
}

.overlay {
  height: 100%;
  width: 0;
  position: fixed;
  z-index: 1;
  top: 0;
  left: 0;
  background-color: rgb(0,0,0);
  background-color: rgba(0,0,0, 0.9);
  overflow-x: hidden;
  transition: 0.5s;
}

.overlay-content {
  position: relative;
  top: 25%;
  width: 100%;
  text-align: center;
  margin-top: 30px;
}

.overlay a {
  padding: 8px;
  text-decoration: none;
  font-size: 36px;
  color: #818181;
  display: block;
  transition: 0.3s;
}

.overlay a:hover, .overlay a:focus {
  color: #f1f1f1;
}

.overlay .closebtn {
  position: absolute;
  top: 20px;
  right: 45px;
  font-size: 60px;
}

@media screen and (max-height: 450px) {
  .overlay a {font-size: 20px}
  .overlay .closebtn {
  font-size: 40px;
  top: 15px;
  right: 35px;
  }
}
</style>
</head>
<body>

<!DOCTYPE html>
<html>
<body>
<h1>Calcolo moltiplicazione </h1>
<form id="frm1" >
 A <input type="text" name="Hbase" value="0"><br>
 B<input type="text" name="HArrivo" value="1000"><br><br>
 <!-- <input type="submit" value="Input dati Trekking">-->
</form>

<p>Calcola il dislivello:</p>
<button onclick="myFunction()">Calcola il dislivello:</button>

<p>Il punto di partenza è:</p>
<p id="base"></p>
<p>Il punto di arrivo è:</p>
<p id="arrivo"></p>

Ia moltiplicazione è di:
<p id="demo"></p>
<script>
function myFunction() {

var x = document.getElementById("frm1");

var base=x.elements[0].value;  
document.getElementById("base").innerHTML =base;

var arrivo=x.elements[1].value;
document.getElementById("arrivo").innerHTML =arrivo;
  
  document.getElementById("demo").innerHTML =Dislivello(base,arrivo);
}

function Dislivello(h1,h2){
return h2*h1;
}

</script>

</body>
</html>
