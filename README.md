
<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Artistas</title>

<style>
body{
  margin:0;
  background:#000;
  font-family:Arial, Helvetica, sans-serif;
  color:white;
}

h1{
  text-align:center;
  padding:40px 0;
  font-size:40px;
  letter-spacing:4px;
}

.artist-grid{
  display:grid;
  grid-template-columns:repeat(auto-fit, minmax(250px,1fr));
  gap:30px;
  padding:40px 80px;
}

.artist{
  position:relative;
  overflow:hidden;
  cursor:pointer;
  transition:0.4s;
}

.artist img{
  width:100%;
  height:350px;
  object-fit:cover;
  transition:0.4s;
}

.artist::after{
  content:"";
  position:absolute;
  bottom:0;
  left:0;
  width:100%;
  height:100%;
  background:linear-gradient(to top, rgba(0,0,0,0.9), rgba(0,0,0,0));
  opacity:0;
  transition:0.4s;
}

.artist p{
  position:absolute;
  bottom:20px;
  left:20px;
  font-size:20px;
  font-weight:bold;
  letter-spacing:2px;
  opacity:0;
  transition:0.4s;
}

.artist:hover img{
  transform:scale(1.08);
}

.artist:hover::after{
  opacity:1;
}

.artist:hover p{
  opacity:1;
}

@media(max-width:768px){
  .artist-grid{
    padding:20px;
  }
}
</style>
</head>

<body>

<h1>ARTISTS</h1>

<div class="artist-grid">

<div class="artist" onclick="playSound()">
<img src="https://i.scdn.co/image/ab67616100005174049b4a6c038ea063a413c5df">
<p>Melanie Martinez</p>
</div>

<div class="artist" onclick="playSound()">
<img src="https://image-cdn-ak.spotifycdn.com/image/ab67706c0000da84f8cf2192b95680abaa9072b9">
<p>MISAMO</p>
</div>

<div class="artist" onclick="playSound()">
<img src="https://i.scdn.co/image/ab6761610000e5eb3d8820046fd455b38d644864">
<p>TWICE</p>
</div>

<div class="artist" onclick="playSound()">
<img src="https://i.scdn.co/image/ab6761610000e5eb9095683b555d7c16fd3b633f">
<p>LE SSERAFIM</p>
</div>

<div class="artist" onclick="playSound()">
<img src="https://i.scdn.co/image/ab6761610000e5eb169a757a7d0ba53a33984416">
<p>ILLIT</p>
</div>

<div class="artist" onclick="playSound()">
<img src="https://i.scdn.co/image/ab67616d00001e028b2f4e49660a958f4fa8bca1">
<p>Jazmin Bean</p>
</div>

<div class="artist" onclick="playSound()">
<img src="https://i.scdn.co/image/ab6761610000e5eb5da361915b1fa48895d4f23f">
<p>NewJeans</p>
</div>

<div class="artist" onclick="playSound()">
<img src="https://images.genius.com/77b0229f961afe70dff2594c6d5eef71.720x720x1.jpg">
<p>NJZ</p>
</div>

<div class="artist" onclick="playSound()">
<img src="https://i.scdn.co/image/ab67616d00001e026ea966c5bf516dabe1b44fb1">
<p>GIRLSET</p>
</div>

<div class="artist" onclick="playSound()">
<img src="https://i.scdn.co/image/ab6761610000e5eb9c50c977dce7112c4c26730f">
<p>VCHA</p>
</div>

<div class="artist" onclick="playSound()">
<img src="https://i.scdn.co/image/ab6761610000e5eb41e029f43b06da5c806c911d">
<p>KG Crown</p>
</div>

<div class="artist" onclick="playSound()">
<img src="https://i.scdn.co/image/ab6761610000f1787d8a2aa2f32e2235d4d81501">
<p>Kaylee Lee</p>
</div>

<div class="artist" onclick="playSound()">
<img src="https://i.scdn.co/image/ab6761610000e5eb70f34c0aeb5787411803adc4">
<p>NAYEON</p>
</div>

<div class="artist" onclick="playSound()">
<img src="https://i.scdn.co/image/ab6761610000e5eb23bc8f178f9fd3e56f6f6a27">
<p>JIHYO</p>
</div>

<div class="artist" onclick="playSound()">
<img src="https://i.scdn.co/image/ab6761610000e5ebe039b9b9ba211f98b42eb0d5">
<p>TZUYU</p>
</div>

<div class="artist" onclick="playSound()">
<img src="https://i.scdn.co/image/ab6761610000e5ebe1fd23eadc9b6e668bffa77f">
<p>CHAEYOUNG</p>
</div>

<div class="artist" onclick="playSound()">
<img src="https://image-cdn-ak.spotifycdn.com/image/ab67706c0000da84073a179268f7d25cb9b6c651">
<p>MINA</p>
</div>

<div class="artist" onclick="playSound()">
<img src="https://i.scdn.co/image/ab6761610000e5eb88952d640547d97808b359c9">
<p>SANA</p>
</div>

<div class="artist" onclick="playSound()">
<img src="https://image-cdn-fa.spotifycdn.com/image/ab67706c0000da8438f1c2dbc8ba8b4ad3c1ee1a">
<p>MOMO</p>
</div>

<div class="artist" onclick="playSound()">
<img src="https://i.scdn.co/image/ab6761610000e5eb484e326315e09b3f382a7960">
<p>KATSEYE</p>
</div>

</div>

<audio id="clickSound" src="https://www.soundjay.com/buttons/sounds/button-09.mp3"></audio>

<script>
function playSound(){
  document.getElementById("clickSound").play();
}
</script>

</body>
</html>
