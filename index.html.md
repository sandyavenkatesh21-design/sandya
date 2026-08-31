<!DOCTYPE html>  
<html lang="en">  
<head>  
<meta charset="UTF-8">  
<title>Happy Birthday ❤️</title>  
  
<style>  
body {  
    margin: 0;  
    font-family: 'Segoe UI', sans-serif;  
    background: linear-gradient(135deg, #ff9a9e, #fad0c4);  
    text-align: center;  
}  
  
/* Start screen */  
#startScreen {  
    position: fixed;  
    top: 0;  
    left: 0;  
    width: 100%;  
    height: 100%;  
    background: #ff6f91;  
    display: flex;  
    align-items: center;  
    justify-content: center;  
    font-size: 24px;  
    color: white;  
    z-index: 10;  
    cursor: pointer;  
}  
  
/* Main content */  
.container {  
    padding: 30px;  
    animation: fadeIn 2s ease-in;  
}  
  
@keyframes fadeIn {  
    from {opacity: 0; transform: translateY(30px);}  
    to {opacity: 1; transform: translateY(0);}  
}  
  
h1 {  
    color: white;  
    font-size: 32px;  
}  
  
/* Photos */  
img {  
    width: 200px;  
    border-radius: 15px;  
    margin: 8px;  
    box-shadow: 0 5px 15px rgba(0,0,0,0.2);  
}  
  
/* Typing text */  
#typing {  
    background: rgba(255,255,255,0.9);  
    padding: 15px;  
    border-radius: 15px;  
    max-width: 600px;  
    margin: 20px auto;  
    font-size: 18px;  
    white-space: pre-line;  
    border-right: 2px solid black;  
    animation: blink 1s infinite;  
}  
  
@keyframes blink {  
    0% { border-color: transparent; }  
    50% { border-color: black; }  
    100% { border-color: transparent; }  
}  
  
/* Button */  
button {  
    margin-top: 20px;  
    padding: 12px 18px;  
    border: none;  
    background: #ff4d6d;  
    color: white;  
    border-radius: 10px;  
    font-size: 16px;  
}  
</style>  
</head>  
  
<body>  
  
<!-- Start Screen -->  
<div id="startScreen" onclick="startSite()">  
Tap to open your surprise 💖  
</div>  
  
<div class="container">  
  
<h1>Happy Birthday My Love 🎂❤️</h1>  
  
<!-- 6 PHOTOS -->  
<img src="photo1.jpg">  
<img src="photo2.jpg">  
<img src="photo3.jpg">  
<img src="photo4.jpg">  
<img src="photo5.jpg">  
<img src="photo6.jpg">  
  
<!-- Typing message -->  
<p id="typing"></p>  
  
<!-- Song Button -->  
<button onclick="showVideo()">Play Our Song 🎶</button>  
  
<!-- YouTube Song -->  
<div id="video" style="display:none; margin-top:20px;">  
<iframe width="300" height="170"  
src="https://www.youtube.com/embed/R8FHtIhWqNo?autoplay=1"  
frameborder="0"  
allow="autoplay; encrypted-media"  
allowfullscreen></iframe>  
</div>  
  
</div>  
  
<script>  
const text = `Happy Birthday baby 😭😭😚  
  
You’re so special to me and no matter what I’ll always find a way to be with you coz I really love you so much Dumbb 😭😭😚😚😚❤️❤️  
  
I wish you the best birthday ever chloo I love you da kanna 😚😚`;  
  
let i = 0;  
  
function typeEffect() {  
    if (i < text.length) {  
        document.getElementById("typing").innerHTML += text.charAt(i);  
        i++;  
        setTimeout(typeEffect, 40);  
    }  
}  
  
function startSite() {  
    document.getElementById("startScreen").style.display = "none";  
    typeEffect();  
}  
  
function showVideo() {  
    document.getElementById("video").style.display = "block";  
}  
</script>  
  
</body>  
</html>  
