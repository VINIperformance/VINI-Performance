# VINI-Performance
<!DOCTYPE html>
<html lang="sv">
<head>
<meta charset="UTF-8">
<title>Viktor Nilsson – Långloppsåkare & tränare</title>

<style>
body{
    font-family: Arial, sans-serif;
    max-width: 900px;
    margin: auto;
    padding: 20px;
    background:#f4f4f4;
    line-height:1.6;
}

header{
    background:white;
    padding:25px;
    border-radius:12px;
}

.tabs{
    margin-top:15px;
}

.tabbutton{
    padding:10px 16px;
    border:none;
    cursor:pointer;
    background:#ddd;
    border-radius:8px 8px 0 0;
    margin-right:6px;
    font-size:15px;
}

.tabbutton.active{
    background:white;
    font-weight:bold;
}

.tabcontent{
    display:none;
    background:white;
    padding:25px;
    border-radius:0 12px 12px 12px;
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
    <button class="tabbutton" onclick="openTab(event,'lektioner')">Lektioner</button>
    <button class="tabbutton" onclick="openTab(event,'meriter')">Meriter</button>
    <button class="tabbutton" onclick="openTab(event,'kontakt')">Kontakt</button>
</div>

<div id="om" class="tabcontent">
<h2>Om mig</h2>
<p>
Jag heter Viktor Nilsson och är långloppsåkare med målsättning att etablera mig på elitnivå
och på sikt ta steget in i ett Ski Classics-team.
Jag tävlar för Lysekils Skid- & Löparförening och kombinerar min elitsatsning med studier
inom träning och idrott.
</p>

<p>
Mitt mål är att utvecklas långsiktigt, både fysiskt och tekniskt, och att hela tiden höja min
prestation i de stora svenska långloppen.
</p>
</div>

<div id="lektioner" class="tabcontent">
<h2>Lektioner & träningspass</h2>

<p>
Utöver min egen elitsatsning håller jag i tekniklektioner och träningspass inom
längdskidåkning och fysträning.
Jag riktar mig främst till barn, ungdomar och motionärer, men även till föreningar och skolor.
</p>

<ul>
<li>Teknikträning längdskidor (klassisk och skate)</li>
<li>Individuella lektioner</li>
<li>Gruppträning för föreningar</li>
<li>Fysträning och bålstabilitet</li>
<li>Inspirationspass och prova-på-pass</li>
</ul>

<p>
Fokus i mina pass ligger på teknik, rörelseförståelse, träningsglädje och långsiktig utveckling.
</p>
</div>

<div id="meriter" class="tabcontent">
<h2>Meriter</h2>

<ul>
<li>3:a i H17–20 – Craft Ski Marathon</li>
<li>3:a i H17–20 – Moraloppet</li>
<li>2:a i totalställningen i H17–20, säsongen 2025/2026</li>
</ul>
</div>

<div id="kontakt" class="tabcontent">
<h2>Kontakt</h2>

<p>
Vill du boka lektion, träningspass eller diskutera samarbete är du välkommen att kontakta mig.
</p>

<p>
Instagram: @viktor_nilsson.06<br>
E-post: viktor.nilsson2006@hotmail.com
</p>
</div>

<script>
function openTab(evt, tabId){

    let contents = document.getElementsByClassName("tabcontent");
    for(let i=0;i<contents.length;i++){
        contents[i].style.display = "none";
    }

    let buttons = document.getElementsByClassName("tabbutton");
    for(let i=0;i<buttons.length;i++){
        buttons[i].classList.remove("active");
    }

    document.getElementById(tabId).style.display = "block";
    evt.currentTarget.classList.add("active");
}

document.getElementById("om").style.display = "block";
</script>

</body>
</html>
