<!DOCTYPE html>
<html lang="sv">
<head>
<meta charset="UTF-8">
<title>Viktor Nilsson – Långloppsåkare</title>

<style>
body{
    font-family: Arial, sans-serif;
    max-width: 900px;
    margin: auto;
    padding: 20px;
    background:#f4f4f4;
}

header{
    background:white;
    padding:20px;
    border-radius:10px;
}

.tabs{
    margin-top:15px;
}

.tabbutton{
    padding:10px 16px;
    border:none;
    background:#ddd;
    cursor:pointer;
    border-radius:8px 8px 0 0;
    margin-right:6px;
}

.tabbutton.active{
    background:white;
    font-weight:bold;
}

.tabcontent{
    display:none;
    background:white;
    padding:20px;
    border-radius:0 10px 10px 10px;
}

.dropdown{
    display:inline-block;
    position:relative;
}

.dropdown-content{
    display:none;
    position:absolute;
    background:white;
    min-width:220px;
    box-shadow:0 4px 8px rgba(0,0,0,0.15);
    border-radius:8px;
    z-index:10;
}

.dropdown-content a{
    display:block;
    padding:10px 12px;
    text-decoration:none;
    color:black;
}

.dropdown-content a:hover{
    background:#eee;
}

.dropdown:hover .dropdown-content{
    display:block;
}
</style>
</head>

<body>

<header>
<h1>Viktor Nilsson</h1>
<p><strong>Långloppsåkare – satsar mot elitnivå och Ski Classics</strong></p>
<p>Tävlar för Lysekils Skid- & Löparförening</p>
</header>

<div class="tabs">

<button class="tabbutton active" onclick="openTab(event,'om')">Om mig</button>

<div class="dropdown">
<button class="tabbutton">Lektioner ▾</button>
<div class="dropdown-content">
<a href="#" onclick="openTab(event,'lektioner_individ')">Individuella lektioner</a>
<a href="#" onclick="openTab(event,'lektioner_grupp')">Grupp & förening</a>
<a href="#" onclick="openTab(event,'lektioner_skola')">Skola</a>
</div>
</div>

<button class="tabbutton" onclick="openTab(event,'meriter')">Meriter</button>
<button class="tabbutton" onclick="openTab(event,'kontakt')">Kontakt</button>

</div>

<div id="om" class="tabcontent">
<h2>Om mig</h2>
<p>
Jag heter Viktor Nilsson och är långloppsåkare med målet att etablera mig på elitnivå och på sikt ta plats i ett Ski Classics-team.
Jag tävlar för Lysekils Skid- & Löparförening.
</p>
</div>

<div id="lektioner_individ" class="tabcontent">
<h2>Individuella lektioner</h2>
<p>
Jag erbjuder individuella tekniklektioner i längdskidåkning, anpassade efter nivå och mål.
</p>
</div>

<div id="lektioner_grupp" class="tabcontent">
<h2>Grupp & förening</h2>
<p>
Jag håller teknik- och träningspass för föreningar och träningsgrupper.
</p>
</div>

<div id="lektioner_skola" class="tabcontent">
<h2>Skola</h2>
<p>
Jag håller även inspirationspass och lektioner för skolor.
</p>
</div>

<div id="meriter" class="tabcontent">
<h2>Meriter</h2>
<ul>
<li>3:a H17–20 Craft Ski Marathon</li>
<li>3:a H17–20 Moraloppet</li>
<li>2:a i totalen H17–20 säsongen 2025/2026</li>
</ul>
</div>

<div id="kontakt" class="tabcontent">
<h2>Kontakt</h2>
<p>
Instagram: @dittkonto<br>
E-post: dinmail@example.com
</p>
</div>

<script>
function openTab(evt, tabId){

    if(evt){
        evt.preventDefault();
    }

    var contents = document.getElementsByClassName("tabcontent");
    for(var i=0;i<contents.length;i++){
        contents[i].style.display = "none";
    }

    var buttons = document.getElementsByClassName("tabbutton");
    for(var i=0;i<buttons.length;i++){
        buttons[i].classList.remove("active");
    }

    var tab = document.getElementById(tabId);
    if(tab){
        tab.style.display = "block";
    }

    if(evt && evt.currentTarget && evt.currentTarget.classList.contains("tabbutton")){
        evt.currentTarget.classList.add("active");
    }
}

window.onload = function(){
    openTab(null,"om");
};
</script>

</body>
</html>
