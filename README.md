<!DOCTYPE html>
<html>
<head>
<title>Finance</title>
<style>
body{font-family:Arial;background:#111;color:#fff;padding:20px}
input,button{padding:10px;margin:5px;border:none}
button{background:green;color:#fff}
div{margin-top:10px}
</style>
</head>
<body>

<h1>💰 Finance</h1>

<input id="text" placeholder="Nima">
<input id="sum" type="number" placeholder="Summa">

<button onclick="add()">Qo'sh</button>

<h2 id="balans">0 so'm</h2>

<div id="list"></div>

<script>
let total=0;

function add(){
let text=document.getElementById("text").value;
let sum=+document.getElementById("sum").value;

total+=sum;

document.getElementById("balans").innerHTML=total+" so'm";

document.getElementById("list").innerHTML+=`
<p>${text} - ${sum} so'm</p>
`;
}
</script>

</body>
</html>
