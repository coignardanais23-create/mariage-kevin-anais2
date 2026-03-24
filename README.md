}
<!DOCTYPE html>
<html lang="fr">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>Mariage Kévin & Anaïs</title>

<style>
body {
margin:0;
font-family:Georgia, serif;
overflow:hidden;
background:white;
}

/* SCENE /
#scene {
width:100vw;
height:100vh;
position:relative;
cursor:pointer;
overflow:hidden;
}

/ RIDEAUX /
.curtain {
position:absolute;
width:50%;
height:100%;
background:white;
z-index:3;
transition:transform 2s ease;
}

#left {left:0;}
#right {right:0;}

.open #left {transform:translateX(-100%);}
.open #right {transform:translateX(100%);}

/ SCEAU /
#seal {
position:absolute;
top:50%;
left:50%;
transform:translate(-50%,-50%);
width:140px;
height:140px;
border-radius:50%;
background:white;
display:flex;
align-items:center;
justify-content:center;
font-size:42px;
color:gold;
font-weight:bold;
box-shadow:0 20px 50px rgba(0,0,0,0.3);
z-index:4;
transition:all 0.7s ease;
}

.break {
transform:translate(-50%,-50%) scale(1.8) rotate(25deg);
opacity:0;
}

/ CONTENU */
#content {
opacity:0;
text-align:center;
padding:20px;
position:absolute;
width:100%;
top:50%;
transform:translateY(-50%);
}

.open #content {
opacity:1;
animation:fade 2s ease;
}

@keyframes fade {
from {opacity:0; transform:translateY(40px);}
to {opacity:1; transform:translateY(-50%);}
}

button {
padding:12px;
margin:5px;
background:black;
color:white;
border:none;
border-radius:6px;
}

textarea {
width:80%;
height:60px;
margin-top:10px;
}
</style>
</head>

<body>

<audio id="music" loop>
<source src="https://cdn.pixabay.com/download/audio/2022/10/25/audio_946b6d2c43.mp3">
</audio>

<div id="scene" onclick="openInvite()">

<div id="left" class="curtain"></div>
<div id="right" class="curtain"></div>

<div id="seal">A & K</div>

<div id="content">
<h1>Bienvenue au mariage de Kévin et Anaïs</h1>
<p>17 juillet 2027</p>

<p>Serez-vous présent ?</p>
<button>Oui</button>
<button>Non</button>

<p>Dormirez-vous sur place ?</p>
<button>Oui</button>
<button>Non</button>

<p>Avez-vous des allergies ?</p>
<button>Oui</button>
<button>Non</button>
<textarea placeholder="Si oui, précisez..."></textarea>

<br><br>
<button>Envoyer</button>
</div>

</div>

<script>
function openInvite(){
document.getElementById("scene").classList.add("open");
document.getElementById("seal").classList.add("break");
document.getElementById("music").play();
}
</script>

</body>
</html
