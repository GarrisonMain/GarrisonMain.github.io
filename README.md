<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>The Los Santos Chronicle — The Romano Files</title>
<style>
:root{--ink:#171717;--paper:#eee9dc;--paper2:#e2dccb;--red:#7d1717;--gold:#a47b31}
*{box-sizing:border-box}
body{margin:0;background:#26231e;color:var(--ink);font-family:Georgia,"Times New Roman",serif}
.paper{max-width:1180px;margin:28px auto;background:var(--paper);box-shadow:0 10px 35px #0008;padding:28px}
.masthead{text-align:center;border-bottom:4px double var(--ink);padding-bottom:14px}
.masthead .date{font:12px Arial,sans-serif;letter-spacing:3px;text-transform:uppercase}
h1{font-size:64px;line-height:.9;margin:8px 0;text-transform:uppercase;letter-spacing:-2px}
.sub{font-style:italic;font-size:15px}
.banner{margin:18px 0;background:var(--red);color:#f6efe1;text-align:center;padding:10px;font:bold 14px Arial;letter-spacing:2px}
.hero{display:grid;grid-template-columns:2fr 1fr;gap:22px;border-bottom:1px solid #555;padding-bottom:22px}
.hero h2{font-size:43px;line-height:.95;margin:5px 0 12px}
.kicker{font:bold 12px Arial;letter-spacing:2px;color:var(--red)}
.lede{font-size:19px;line-height:1.45}
.columns{display:grid;grid-template-columns:repeat(3,1fr);gap:20px;margin-top:22px}
.card{border-top:3px solid var(--ink);padding-top:10px}
.card h3{font-size:25px;margin:5px 0}
.card p{line-height:1.5;font-size:15px}
button{cursor:pointer;border:1px solid #333;background:var(--paper2);padding:8px 12px;font:bold 12px Arial}
button:hover{background:#d2c7ad}
.timeline{margin-top:25px;border-top:4px double var(--ink);padding-top:18px}
.timeline h2{text-align:center;text-transform:uppercase;letter-spacing:3px}
.events{display:grid;grid-template-columns:repeat(3,1fr);gap:10px}
.event{padding:14px;background:#ddd6c5;border:1px solid #999;cursor:pointer}
.event strong{display:block;color:var(--red);font: bold 13px Arial;letter-spacing:1px}
.event b{font-size:18px}
.details{margin-top:15px;min-height:95px;padding:15px;border:1px dashed #777;background:#f3eee3;font-size:16px;line-height:1.5}
.quote{font-size:25px;font-style:italic;border-left:5px solid var(--red);padding:10px 18px;margin:20px 0}
.classified{border-top:4px double var(--ink);margin-top:25px;padding-top:15px;text-align:center;font:12px Arial}
.modal{display:none;position:fixed;inset:0;background:#000b;align-items:center;justify-content:center;padding:20px;z-index:5}
.modal.open{display:flex}
.modalbox{max-width:820px;max-height:85vh;overflow:auto;background:var(--paper);padding:32px;border:3px solid var(--ink);box-shadow:0 15px 50px #000}.modalbox p{font-size:17px;line-height:1.7;margin-bottom:0}.modalbox h2{font-family:Georgia,"Times New Roman",serif;text-transform:uppercase;letter-spacing:1px;border-bottom:1px solid #777;padding-bottom:12px}
.modalbox h2{margin-top:0;font-size:32px}
.close{float:right;background:var(--red);color:white;border:0}
@media(max-width:800px){h1{font-size:42px}.hero,.columns,.events{grid-template-columns:1fr}.paper{margin:0;padding:16px}}
</style>
</head>
<body>
<main class="paper">
<header class="masthead">
  <div class="date">SPECIAL INVESTIGATIVE EDITION • LOS SANTOS • 2026</div>
  <h1>The Los Santos Chronicle</h1>
  <div class="sub">Truth, Power &amp; The Stories They Tried To Bury</div>
</header>

<div class="banner">THE ROMANO FILES — AN INVESTIGATION INTO A FAMILY'S RISE, FALL &amp; DISAPPEARANCE</div>

<section class="hero">
  <div>
    <div class="kicker">SPECIAL REPORT</div>
    <h2>The Family That Refused To Die</h2>
    <p class="lede"><b>Founded in 2023 after the fall of the Rizzo Family, the Romanos became one of Los Santos' most infamous dynasties.</b> From organized crime to legitimate business, from family tragedy to an unexplained prison escape, their story has left behind more questions than answers.</p>
    <button onclick="openModal('The Romano Question')">READ THE INVESTIGATION →</button>
  </div>
  <aside>
    <div class="kicker">THE LAST KNOWN CHAPTER</div>
    <h3>Where Is Ivan Romano?</h3>
    <p>After being caught in the killing of his wife Nadia, Ivan was imprisoned. Not long afterward, unknown accomplices broke him out.</p>
    <p><b>His current whereabouts remain unknown.</b></p>
  </aside>
</section>

<section class="columns">
  <article class="card"><div class="kicker">2023–2024</div><h3>A Dynasty Is Born</h3><p>After the Rizzo Family's fall, Garrison Romano builds a new household from the wreckage. He and Lyra attempt to turn a criminal legacy into a family legacy, raising children who will eventually build empires of their own.</p><button onclick="openModal('Garrison & Lyra')">FULL STORY</button></article>
  <article class="card"><div class="kicker">THE UNSOLVED MYSTERY</div><h3>Blood Within The House</h3><p>A quiet home in Roxwood becomes the scene of one of Los Santos' most disturbing family crimes. Garrison and Lyra are murdered, and the investigation eventually leads investigators back into the Romano bloodline.</p><button onclick="openModal('The Roxwood Murders')">CASE FILE</button></article>
  <article class="card"><div class="kicker">2025</div><h3>The Kings &amp; The Saints</h3><p>Ivan inherits the Romano name, enters The Kings, and meets Nadia King. When The Kings fall, the pair create something even more powerful: The Third Street Saints, a street organization that will dominate Los Santos.</p><button onclick="openModal('The Saints')">READ MORE</button></article>
</section>

<div class="quote">“Twice, the Romano name was nearly destroyed from within. Twice, it survived.”</div>

<section class="timeline">
<h2>Romano Family Timeline</h2>
<div class="events">
  <div class="event" onclick="showEvent(0)"><strong>2023</strong><b>The Beginning</b></div>
  <div class="event" onclick="showEvent(1)"><strong>EARLY 2024</strong><b>Roxwood</b></div>
  <div class="event" onclick="showEvent(2)"><strong>EARLY 2025</strong><b>Ivan Takes Control</b></div>
  <div class="event" onclick="showEvent(3)"><strong>2025</strong><b>The Third Street Saints</b></div>
  <div class="event" onclick="showEvent(4)"><strong>LATE 2025</strong><b>The Affair</b></div>
  <div class="event" onclick="showEvent(5)"><strong>AFTERWARD</strong><b>The Escape</b></div>
</div>
<div class="details" id="details">Select a headline above to open the corresponding case file.</div>
</section>


<section class="feature" style="margin-top:25px;border-top:4px double var(--ink);padding-top:20px">
  <div class="kicker">THE COMPLETE DOSSIER</div>
  <h2 style="font-size:38px;margin:5px 0 10px;text-transform:uppercase">A Family Built On Ashes</h2>
  <p style="font-size:18px;line-height:1.65">The Romano story cannot be reduced to a list of crimes. It is a story about what happens when a family repeatedly tries to reinvent itself—and repeatedly discovers that the past has a way of following it home.</p>
  <div class="columns">
    <article class="card"><div class="kicker">LEGACY</div><h3>From Crime To Commerce</h3><p>Garrison's dream of a family beyond crime did not die with him. His children carried that idea forward, and Ivan and Nadia eventually pushed the family further toward legitimate business.</p></article>
    <article class="card"><div class="kicker">TRAGEDY</div><h3>Blood Is Thicker</h3><p>Both of the family's defining murders came from within its own walls. Garrison and Lyra fell to their son. Nadia fell to her husband. In the Romano story, danger was never simply outside the family.</p></article>
    <article class="card"><div class="kicker">MYSTERY</div><h3>The Name Remains</h3><p>Korro's motives are still unknown. Ivan's whereabouts are unknown. The identities of Ivan's rescuers are unknown. What remains certain is that the Romano name has survived every attempt to erase it.</p></article>
  </div>
</section>

<section class="classified">
  <b>THE ROMANO FILES</b> • Some names, motives and events remain disputed. This special edition presents the known history as reconstructed from accounts surrounding the Romano Family.
</section>
</main>

<div class="modal" id="modal">
 <div class="modalbox">
  <button class="close" onclick="closeModal()">CLOSE ✕</button>
  <h2 id="modalTitle"></h2>
  <p id="modalText"></p>
 </div>
</div>

<script>
const data=[
["2023 — THE BEGINNING",
"Los Santos was no stranger to powerful families, but the Romano name arrived at a very particular moment. The Rizzo Family had fallen, leaving behind a vacuum of influence and a city full of people looking for the next name to rally behind. Garrison Romano stepped into that vacuum and founded the Romano Family.<br><br>Garrison's history made the decision all the more remarkable. He had spent years surrounded by crime and violence, yet his ambitions were no longer limited to the streets. Alongside his wife, Lyra Romano, he began constructing something that he hoped would outlive the criminal world: a family.<br><br>The Romanos became more than a surname. Their children grew into their own people, establishing businesses and carving out individual identities. The family's future appeared to be moving away from guns and toward ownership, independence, and legitimate enterprise.<br><br>But the Romano legacy was still young. And in Los Santos, a peaceful ending is rarely guaranteed."],

["EARLY 2024 — THE ROXWOOD MURDERS",
"The call that came out of Roxwood in early 2024 would change the Romano Family forever. Garrison and Lyra Romano had been shot inside their own home. There was no street battle, no rival organization claiming responsibility, and no obvious outsider waiting to be blamed. Their deaths struck at the heart of the family itself.<br><br>For a time, the case appeared to be another unsolved killing in a city already accustomed to them. Investigators searched for enemies from Garrison's past, people who may have wanted revenge against the former criminal. But the deeper the investigation went, the darker the answer became.<br><br>The trail eventually led to Garrison and Lyra's own son: Korro Romano.<br><br>The revelation transformed the case. What had looked like a conventional murder became a family tragedy of almost incomprehensible proportions. Korro's intentions remain unknown. No single explanation has ever completely settled the question of why a son would turn against his parents.<br><br>Whatever the answer, Garrison and Lyra were gone. The first generation of the Romano Family had been shattered, and the surviving Romanos were left to decide what the name would become next."],

["EARLY 2025 — IVAN TAKES CONTROL",
"With Garrison gone, the responsibility of carrying the Romano name eventually passed to his younger brother, Ivan Romano. In early 2025, Ivan took the reins of the family.<br><br>Ivan inherited more than a surname. He inherited the unfinished work of his brother, the scars left by the Roxwood murders, and a family whose future was suddenly uncertain. Rather than simply repeat Garrison's story, Ivan began writing a chapter of his own.<br><br>That chapter led him toward The Kings, a crew that became an important turning point in his life. Within the organization, Ivan encountered people who would influence his future and, most importantly, met Nadia King.<br><br>The two began spending more time together. Their relationship developed while The Kings themselves were rising and eventually approaching their own fall. When the organization collapsed, Ivan and Nadia did not disappear with it.<br><br>Instead, they walked away together—and began building something new."],

["2025 — THE SAINTS RISE",
"The end of The Kings became the beginning of the Third Street Saints.<br><br>Ivan Romano and Nadia King founded the organization as a street gang, but the Saints quickly became much more than a collection of people carrying a name. They built a reputation through organization, ambition, loyalty, and an aggressive climb through Los Santos' power structure.<br><br>The Saints kept moving upward. Territory became influence. Influence became power. Before long, their name carried weight throughout the city, and they were regarded as the number one street gang in Los Santos' history.<br><br>At the center of that rise were Ivan and Nadia. Their personal relationship and their organization became intertwined, each strengthening the other. What had started as two people finding one another after the fall of The Kings had become a partnership at the head of one of the city's most powerful street movements.<br><br>Then came marriage.<br><br>Nadia King became Nadia Romano, bringing a new matriarch into the family. For the first time since the deaths of Garrison and Lyra, the Romano name appeared to have found another generation willing to carry it forward.<br><br>And then, unexpectedly, the Romanos began to change."],

["LATE 2025 — THE AFFAIR",
"By late 2025, the Romanos had begun leaving their criminal history behind. Ivan and Nadia fostered children who would eventually find their own paths, including paths into business ownership. The family name that had once been associated with criminal organizations was increasingly associated with legitimate businesses and entrepreneurship.<br><br>For a family that had spent years surviving violence, this should have been the happy ending.<br><br>It wasn't.<br><br>Ivan discovered that Nadia had been having an affair. Whatever trust remained between them collapsed. The same man who had helped build an organization beside her would ultimately become the person responsible for her death.<br><br>Ivan killed Nadia.<br><br>Unlike the Roxwood murders, there was no distant mystery surrounding the immediate aftermath. Detective Cole Locke caught Ivan red-handed. The Romano patriarch was arrested and sent to prison, seemingly bringing the latest chapter of the family saga to a definitive close.<br><br>But the Romano story had never been known for definitive endings."],

["AFTERWARD — THE ESCAPE",
"Ivan Romano's imprisonment did not last forever.<br><br>At some point after his arrest, unknown accomplices succeeded in breaking him out of custody. The identities of those responsible, the circumstances of the escape, and Ivan's destination all remain unknown.<br><br>Then came the silence.<br><br>Ivan vanished from public view. The Romano Family, once one of the most visible names in Los Santos, became increasingly quiet. Businesses remained, memories remained, and the name remained—but the people who had once made the Romanos impossible to ignore were rarely seen anymore.<br><br>It was almost as if the family had collectively stepped away from the city and closed the door behind them.<br><br>Some believe Ivan is still alive somewhere beyond Los Santos. Others believe the surviving Romanos simply chose to protect what remained of the family by disappearing from the public eye.<br><br>And there is one possibility that refuses to die: that the Romano Family is not finished.<br><br>Because powerful names do not always disappear. Sometimes they go quiet. Sometimes they wait.<br><br>And if the Romano legacy has taught Los Santos anything, it is that the quietest chapters can be the ones that come immediately before the next storm."]
];
function showEvent(i){document.getElementById("details").innerHTML="<b>"+data[i][0]+"</b><br><br>"+data[i][1]}
const modal=document.getElementById("modal");
function openModal(title){
 document.getElementById("modalTitle").textContent=title;
 const map={
 "The Romano Question":"The Romano story is a cycle of reinvention. Garrison tried to turn a criminal past into a family legacy. Ivan inherited that legacy, rebuilt it through The Kings and The Third Street Saints, and then watched it collapse through betrayal and murder. Across every generation, the same question returns: can the Romano name ever escape the violence that created it?",
 "Garrison & Lyra":"Garrison Romano entered Los Santos as a notorious criminal, but his ambitions eventually changed. With Lyra beside him, he tried to build a household that could outlast his old life. Their children became business owners and independent figures, suggesting that the family might finally have a future beyond organized crime. Their deaths in Roxwood ended that dream violently.",
 "The Roxwood Murders":"The Roxwood murders remain one of the defining tragedies of the Romano story. Garrison and Lyra were killed inside their home, and investigators eventually discovered that their son Korro Romano was responsible. His motive remains one of the family's great unanswered questions, leaving the case surrounded by speculation and silence.",
 "The Saints":"Ivan Romano's time with The Kings introduced him to Nadia King. After The Kings fell, the two founded The Third Street Saints and rose rapidly through Los Santos. Their organization became one of the city's most powerful street gangs, while their personal relationship culminated in marriage and Nadia taking the Romano name. For a moment, the family appeared stronger than ever.",
 "The Affair":"The family's attempted transition into legitimate life ended in catastrophe when Ivan discovered Nadia's affair. Ivan killed his wife and was caught by Detective Cole Locke. The event shattered the family's new identity and placed Ivan at the center of another Romano tragedy.",
 "The Escape":"Ivan's story did not end in prison. Unknown accomplices broke him out, after which he disappeared. No confirmed account explains where he went or who helped him. Since then, the Romano Family has largely withdrawn from public life, creating the final mystery in a story already filled with them."
};
 document.getElementById("modalText").innerHTML=map[title]||"The full story is contained within the Romano investigative archive.";
 modal.classList.add("open");
}
function closeModal(){modal.classList.remove("open")}
modal.addEventListener("click",e=>{if(e.target===modal)closeModal()});
</script>
</body>
</html>
