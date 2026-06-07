<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>The Happiness Hub</title>

<style>
body{
    margin:0;
    font-family:Arial,sans-serif;
    background:#f4fff7;
    color:#333;
    text-align:center;
}

header{
    background:linear-gradient(to right,#87CEEB,#98FB98);
    padding:50px 20px;
}

h1{
    margin:0;
    font-size:3rem;
}

section{
    padding:40px 20px;
}

.quote{
    font-size:1.3rem;
    font-style:italic;
    max-width:700px;
    margin:auto;
}

.gallery{
    display:flex;
    flex-wrap:wrap;
    justify-content:center;
    gap:15px;
}

.gallery img{
    width:300px;
    height:200px;
    object-fit:cover;
    border-radius:12px;
}

.breathing{
    background:#e8f8ff;
    border-radius:15px;
    padding:30px;
    max-width:500px;
    margin:auto;
}

#breathText{
    font-size:2rem;
    margin:20px 0;
}

button{
    padding:12px 25px;
    border:none;
    background:#4CAF50;
    color:white;
    border-radius:8px;
    cursor:pointer;
}

.music a{
    display:block;
    margin:10px;
    text-decoration:none;
    color:#0066cc;
}

.gratitude{
    max-width:600px;
    margin:auto;
}

textarea{
    width:100%;
    height:120px;
    padding:10px;
    border-radius:10px;
}

footer{
    background:#dff6df;
    padding:20px;
}
</style>
</head>

<body>

<header>
<h1>The Happiness Hub 😊</h1>
<p>Small moments of gratitude create lasting happiness.</p>
</header>

<section>
<h2>Inspirational Quote</h2>
<p class="quote">
"Happiness is not something ready made. It comes from your own actions."
– Dalai Lama
</p>
</section>

<section>
<h2>Nature Gallery 🌿</h2>

<div class="gallery">
<img src="https://images.unsplash.com/photo-1506744038136-46273834b3fb?w=800" alt="">
<img src="https://images.unsplash.com/photo-1500530855697-b586d89ba3ee?w=800" alt="">
<img src="https://images.unsplash.com/photo-1441974231531-c6227db76b6e?w=800" alt="">
</div>

</section>

<section>
<h2>3-Minute Guided Breathing Exercise 🫁</h2>

<div class="breathing">
<p>Follow the instructions below.</p>
<div id="breathText">Ready?</div>
<button onclick="startBreathing()">Start</button>
</div>

</section>

<section class="music">
<h2>Happy & Relaxing Music 🎵</h2>

<a href="https://www.youtube.com/results?search_query=relaxing+nature+music" target="_blank">
Relaxing Nature Music
</a>

<a href="https://www.youtube.com/results?search_query=happy+uplifting+music" target="_blank">
Happy Uplifting Music
</a>

<a href="https://www.youtube.com/results?search_query=calming+instrumental+music" target="_blank">
Calming Instrumental Music
</a>

</section>

<section class="gratitude">
<h2>Things I'm Grateful For 🙏</h2>

<p>Write 3 things that make you thankful today.</p>

<textarea placeholder="I am grateful for..."></textarea>

</section>

<footer>
<p>Dynamics of Happiness Project</p>
<p>Created by Student Project Submission</p>
</footer>

<script>
function startBreathing(){

const text=document.getElementById("breathText");

let cycle=0;

const interval=setInterval(()=>{

if(cycle%3===0){
text.innerHTML="Breathe In 🌿";
}
else if(cycle%3===1){
text.innerHTML="Hold ✨";
}
else{
text.innerHTML="Breathe Out 🍃";
}

cycle++;

if(cycle===18){
clearInterval(interval);
text.innerHTML="Great Job! 😊";
}

},5000);
}
</script>

</body>
</html>