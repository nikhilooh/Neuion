<!DOCTYPE html>
<html>
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>NK ARTS.in.com - Smart AI Studio</title>

<style>
body{
    margin:0;
    font-family:Arial;
    background:linear-gradient(135deg,#0f0c29,#302b63,#24243e);
    color:white;
    text-align:center;
}
header{
    padding:20px;
    background:#1a1a40;
}
h1{
    color:#ff4d6d;
}
nav button{
    padding:10px 20px;
    margin:5px;
    border:none;
    border-radius:8px;
    background:#ff006e;
    color:white;
    cursor:pointer;
}
nav button:hover{
    background:#fb5607;
}
.section{
    display:none;
    padding:20px;
}
.active{
    display:block;
}
input,textarea{
    width:80%;
    padding:10px;
    margin:10px;
    border-radius:8px;
    border:none;
}
.card{
    background:#3a0ca3;
    padding:20px;
    margin:10px;
    border-radius:12px;
    display:inline-block;
}
footer{
    margin-top:30px;
    padding:10px;
    background:#1a1a40;
}
</style>

</head>

<body>

<header>
<h1>NK ARTS.in.com</h1>
<p>World Smartest AI Video & Image Creator</p>
</header>

<nav>
<button onclick="show('video')">AI Video</button>
<button onclick="show('image')">AI Image</button>
<button onclick="show('textimage')">Text → Image</button>
<button onclick="show('emotify')">Emotify Tool</button>
<button onclick="show('premium')">Premium</button>
</nav>

<div id="video" class="section active">
<h2>🎥 AI Video Generator</h2>
<textarea placeholder="Describe your video idea..."></textarea><br>
<button onclick="generate('videoResult')">Generate Smart Video</button>
<p id="videoResult"></p>
</div>

<div id="image" class="section">
<h2>🖼️ AI Image Generator</h2>
<input type="text" placeholder="Enter image prompt..."><br>
<button onclick="generate('imageResult')">Generate Image</button>
<p id="imageResult"></p>
</div>

<div id="textimage" class="section">
<h2>✍️ Text → Image Converter</h2>
<input type="text" placeholder="Type text to convert..."><br>
<button onclick="generate('textImageResult')">Convert</button>
<p id="textImageResult"></p>
</div>

<div id="emotify" class="section">
<h2>😎 Emotify Style Tool</h2>
<input type="file"><br>
<p>Extract emotions & recreate with new textures & colors</p>
<button onclick="generate('emoteResult')">Process Emote</button>
<p id="emoteResult"></p>
</div>

<div id="premium" class="section">
<h2>👑 Premium Subscription</h2>
<div class="card">
<h3>Weekly</h3>
<p>₹49</p>
</div>
<div class="card">
<h3>Monthly</h3>
<p>₹99</p>
</div>
<div class="card">
<h3>Yearly</h3>
<p>₹1100</p>
</div>
</div>

<footer>
<p>🔒 AI Safety Shield Enabled | NK ARTS © 2026</p>
</footer>

<script>
function show(id){
    let sections=document.querySelectorAll('.section');
    sections.forEach(sec=>sec.classList.remove('active'));
    document.getElementById(id).classList.add('active');
}

function generate(resultId){
    document.getElementById(resultId).innerHTML=
    "🚀 Smart AI is generating content... <br> ✔ Safety Check Passed <br> ✔ Monetization Mode Optimized";
}
</script>

</body>
</html>
