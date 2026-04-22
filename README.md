
<!DOCTYPE html>
<html>
<head>
<title>管理ページ</title>

<style>
body{
  font-family:"Trebuchet MS";
  background:linear-gradient(#ffe6f2,#e6f7ff);
  text-align:center;
}
h1{color:#ff4da6;text-shadow:2px 2px white;}

.box{
  background:white;
  width:360px;
  margin:auto;
  padding:25px;
  border-radius:25px;
  box-shadow:0 0 15px rgba(0,0,0,0.2);
}

input{
  padding:10px;
  font-size:20px;
  width:90px;
  text-align:center;
  border-radius:10px;
  border:1px solid #ccc;
}

button{
  background:#ff66b2;
  color:white;
  border:none;
  padding:10px 20px;
  border-radius:20px;
  margin-top:15px;
  cursor:pointer;
}
</style>
</head>

<body>

<h1>⭐管理ページ⭐</h1>

<div class="box">
  <h3>待ち時間を入力</h3>
  <input type="number" id="waitInput"> 分
  <br>
  <button onclick="saveWait()">更新</button>
  <p id="nowSet"></p>
</div>

<script>
function saveWait(){
  const wait = document.getElementById("waitInput").value;
  localStorage.setItem("waitTime", wait);
  document.getElementById("nowSet").innerHTML="更新しました✨";
}
</script>

</body>
</html>
