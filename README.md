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

<style>
.longread{margin-top:28px;border-top:4px double var(--ink);padding-top:20px}
.longread h2{font-size:38px;text-transform:uppercase;margin:4px 0 8px}
.longread h3{font-size:25px;margin-bottom:6px}
.longread p{font-size:16px;line-height:1.65}
.two-col{columns:2;column-gap:34px}
.factbox{break-inside:avoid;border:2px solid #555;padding:14px;margin:16px 0;background:#e4dece}
.factbox h4{margin:0 0 8px;text-transform:uppercase;font:700 12px Arial;letter-spacing:2px;color:var(--red)}
.evidence{display:grid;grid-template-columns:repeat(4,1fr);gap:10px}
.evidence div{border:1px solid #888;padding:12px;background:#ddd6c5;min-height:90px}
.evidence strong{display:block;font:700 11px Arial;letter-spacing:1px;color:var(--red);margin-bottom:6px}
.pull{font-size:27px!important;line-height:1.15!important;font-style:italic;text-align:center;border-top:1px solid #777;border-bottom:1px solid #777;padding:15px!important;margin:20px 0}
.familytree{display:flex;flex-direction:column;align-items:center;gap:8px;margin:20px 0}
.node{border:2px solid var(--ink);padding:9px 18px;background:#e5dfd0;text-align:center;min-width:220px}
.node.red{border-color:var(--red)}
.branch{display:flex;gap:10px;justify-content:center;flex-wrap:wrap}
.profile-grid{display:grid;grid-template-columns:repeat(2,1fr);gap:14px}
.profile{border-top:3px solid var(--ink);padding:12px 4px}
.profile h3{margin:0;font-size:23px}
.profile .role{font:700 11px Arial;letter-spacing:2px;color:var(--red)}
.profile p{font-size:14px}
@media(max-width:800px){.two-col{columns:1}.evidence,.profile-grid{grid-template-columns:1fr}}
</style>


<style>
.archive-nav{display:flex;gap:8px;flex-wrap:wrap;margin:18px 0;padding:12px;border:1px solid #777;background:#ddd6c5;position:sticky;top:0;z-index:3}
.archive-nav button{background:#eee9dc}
.case-grid{display:grid;grid-template-columns:repeat(3,1fr);gap:14px}
.case-card{background:#ded7c7;border:2px solid #555;padding:15px;cursor:pointer;position:relative;transition:.15s}
.case-card:hover{transform:translateY(-2px);box-shadow:4px 4px 0 #777}
.case-card .stamp{position:absolute;right:8px;top:8px;border:2px solid var(--red);color:var(--red);font:bold 9px Arial;padding:3px;transform:rotate(-5deg)}
.case-card h3{font-size:23px;margin:8px 0}
.case-card p{font-size:14px;line-height:1.45}
.case-number{font:bold 11px Arial;letter-spacing:2px;color:var(--red)}
.badge{display:inline-block;font:700 10px Arial;letter-spacing:1px;border:1px solid #555;padding:3px 6px;margin-top:5px}
.searchbar{display:flex;gap:8px;margin:15px 0}
.searchbar input{flex:1;background:#f3eee3;border:1px solid #555;padding:10px;font-family:Georgia}
.detective-file{display:grid;grid-template-columns:180px 1fr;gap:20px;border:2px solid #444;background:#ddd6c5;padding:18px}
.detective-seal{height:180px;border:3px double #555;display:flex;align-items:center;justify-content:center;text-align:center;font:bold 15px Arial;letter-spacing:2px;transform:rotate(-2deg)}
.redacted{background:#171717;color:#171717;padding:0 5px;cursor:pointer}
.redacted:hover{color:#eee}
.modal.case-modal{background:#000c}
.case-modal .modalbox{max-width:950px}
.case-paper{background:#eee9dc;padding:22px;border:1px solid #555;box-shadow:inset 0 0 30px #0001}
.case-header{display:flex;justify-content:space-between;border-bottom:3px double #222;padding-bottom:10px;gap:15px}
.case-header h2{margin:0;font-size:32px}
.case-meta{font:11px Arial;line-height:1.6;text-transform:uppercase}
.file-section{border-top:1px solid #777;margin-top:15px;padding-top:12px}
.file-section h4{font:bold 12px Arial;letter-spacing:2px;color:var(--red);margin:0 0 8px}
.file-section p{font-size:16px;line-height:1.65}
.file-list{display:grid;grid-template-columns:repeat(2,1fr);gap:8px}
.file-item{padding:9px;background:#ddd6c5;border:1px solid #999;font-size:13px}
.timeline .event{position:relative}
.timeline .event:after{content:"OPEN FILE";display:block;margin-top:7px;font:9px Arial;letter-spacing:1px;color:var(--red)}
@media(max-width:800px){.case-grid{grid-template-columns:1fr}.detective-file{grid-template-columns:1fr}.file-list{grid-template-columns:1fr}.case-header{display:block}}
</style>

</head>
<body>
<main class="paper">
<header class="masthead">
  <div class="date">SPECIAL INVESTIGATIVE EDITION • LOS SANTOS • 2026</div>
  <h1>The Los Santos Chronicle</h1>
  <div class="sub">Truth, Power &amp; The Stories They Tried To Bury</div>
</header>


<nav class="archive-nav">
  <button onclick="scrollToId('cases')">CASE FILES</button>
  <button onclick="scrollToId('detective')">DETECTIVE FILE</button>
  <button onclick="scrollToId('evidence')">EVIDENCE ROOM</button>
  <button onclick="scrollToId('questions')">UNSOLVED</button>
</nav>

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



<section class="longread" id="cases">
  <div class="kicker">LOS SANTOS POLICE ARCHIVE • RECONSTRUCTED FILES</div>
  <h2>The Romano Case Files</h2>
  <p>These reconstructed case files present the Romano saga as a collection of investigative records. Some entries are established facts within the Romano history; others are investigative leads, unanswered questions, or details whose truth remains uncertain.</p>

  <div class="searchbar">
    <input id="caseSearch" oninput="filterCases()" placeholder="Search the archive: Roxwood, Ivan, Saints, Locke...">
    <button onclick="document.getElementById('caseSearch').value='';filterCases()">CLEAR</button>
  </div>

  <div class="case-grid" id="caseGrid">
    <article class="case-card" data-search="roxwood garrison lyra murder korro">
      <span class="stamp">COLD CASE</span>
      <div class="case-number">CASE 24-001</div>
      <h3>The Roxwood Murders</h3>
      <p>Garrison and Lyra Romano are killed inside their home. The investigation ultimately points inward, toward their son Korro.</p>
      <span class="badge">OPEN FILE</span>
      <button onclick="openCase('roxwood')">VIEW DOSSIER</button>
    </article>
    <article class="case-card" data-search="korro romano motive son">
      <span class="stamp">MOTIVE UNKNOWN</span>
      <div class="case-number">SUPPLEMENT 24-K</div>
      <h3>The Korro Question</h3>
      <p>A supplemental investigation into the family member identified as responsible for the Roxwood killings—and the motive nobody could explain.</p>
      <span class="badge">VIEW SUPPLEMENT</span>
      <button onclick="openCase('korro')">VIEW DOSSIER</button>
    </article>
    <article class="case-card" data-search="ivan kings nadia king saints">
      <span class="stamp">ARCHIVED</span>
      <div class="case-number">INTEL 25-I</div>
      <h3>Ivan &amp; The Kings</h3>
      <p>Ivan assumes control of the Romano Family and enters The Kings, where he meets Nadia King.</p>
      <span class="badge">INTELLIGENCE FILE</span>
      <button onclick="openCase('kings')">VIEW DOSSIER</button>
    </article>
    <article class="case-card" data-search="third street saints gang ivan nadia">
      <span class="stamp">HIGH INTEREST</span>
      <div class="case-number">ORG 25-TS</div>
      <h3>The Saints Dossier</h3>
      <p>The rise of The Third Street Saints from a post-Kings organization into Los Santos' dominant street gang.</p>
      <span class="badge">ORGANIZED CRIME</span>
      <button onclick="openCase('saints')">VIEW DOSSIER</button>
    </article>
    <article class="case-card" data-search="nadia affair murder cole locke detective">
      <span class="stamp">CLOSED / ESCAPE</span>
      <div class="case-number">HOMICIDE 25-N</div>
      <h3>The Nadia Romano Homicide</h3>
      <p>Ivan kills Nadia after discovering her affair. Detective Cole Locke catches Ivan red-handed.</p>
      <span class="badge">HOMICIDE FILE</span>
      <button onclick="openCase('nadia')">VIEW DOSSIER</button>
    </article>
    <article class="case-card" data-search="ivan escape prison accomplices disappearance">
      <span class="stamp">ACTIVE LEAD</span>
      <div class="case-number">ESC-25-IR</div>
      <h3>The Ivan Romano Escape</h3>
      <p>Unknown accomplices break Ivan out of prison. His whereabouts—and theirs—remain unknown.</p>
      <span class="badge">ACTIVE LEAD</span>
      <button onclick="openCase('escape')">VIEW DOSSIER</button>
    </article>
  </div>
</section>

<section class="longread" id="detective">
  <div class="kicker">LAW ENFORCEMENT ARCHIVE</div>
  <h2>The Detective Who Saw The End</h2>
  <div class="detective-file">
    <div class="detective-seal">LOS SANTOS<br>DETECTIVE<br>ARCHIVE<br>CASE OFFICER</div>
    <div>
      <h3 style="margin-top:0;font-size:30px">Detective Cole Locke</h3>
      <p>By the time Cole Locke encountered Ivan Romano, the Romano name already carried years of history. Garrison's death had become a family legend. The Saints had become a street legend. Nadia had become the second matriarch.</p>
      <p>Locke's importance to the story came from something much simpler: he was there when Ivan's final public chapter collapsed.</p>
      <p>Following Nadia's death, Locke caught Ivan red-handed. Unlike the Roxwood case, where the truth emerged through investigation, the evidence against Ivan was immediate. The detective had effectively watched the Romano dynasty's second patriarch become the perpetrator of another family tragedy.</p>
      <p>But Locke never got the ending investigators wanted. Ivan was imprisoned—and then escaped.</p>
      <div class="factbox">
        <h4>Detective's Note</h4>
        <p>“The case ended in custody. The story did not.”</p>
      </div>
      <p>From that point forward, Locke's role shifted from arresting officer to one of the last known investigators connected directly to Ivan Romano. The escape left him with the question every investigator hates: <i>where did the suspect go?</i></p>
    </div>
  </div>
</section>

<section class="longread" id="evidence">
  <div class="kicker">EVIDENCE ROOM</div>
  <h2>Evidence &amp; Investigative Leads</h2>
  <p>Click a redacted item to reveal the text. In-universe, these represent the fragments investigators might have assembled while trying to understand the Romano family.</p>
  <div class="evidence">
    <div><strong>EXHIBIT A</strong>Roxwood residence — scene connected to the deaths of Garrison and Lyra.</div>
    <div><strong>EXHIBIT B</strong>Family connection — investigators eventually identified Korro Romano as responsible.</div>
    <div><strong>EXHIBIT C</strong>Saints intelligence — Ivan and Nadia's organization rose to unprecedented street power.</div>
    <div><strong>EXHIBIT D</strong>Witness account — Ivan was caught red-handed by Detective Cole Locke.</div>
    <div><strong>EXHIBIT E</strong>Escape network — <span class="redacted" onclick="reveal(this)">IDENTITY WITHHELD</span></div>
    <div><strong>EXHIBIT F</strong>Last known destination — <span class="redacted" onclick="reveal(this)">LOCATION UNKNOWN</span></div>
    <div><strong>EXHIBIT G</strong>Financial trail — <span class="redacted" onclick="reveal(this)">INSUFFICIENT INFORMATION</span></div>
    <div><strong>EXHIBIT H</strong>Romano family status — <span class="redacted" onclick="reveal(this)">NO CONFIRMED PUBLIC LEADER</span></div>
  </div>
</section>

<section class="longread" id="questions">
  <div class="kicker">DETECTIVE'S BOARD</div>
  <h2>What Locke Never Solved</h2>
  <div class="file-list">
    <div class="file-item"><b>QUESTION 01</b><br>Who helped Ivan escape?</div>
    <div class="file-item"><b>QUESTION 02</b><br>Where is Ivan now?</div>
    <div class="file-item"><b>QUESTION 03</b><br>What motivated Korro?</div>
    <div class="file-item"><b>QUESTION 04</b><br>Who knew the escape was coming?</div>
    <div class="file-item"><b>QUESTION 05</b><br>Are Romano businesses still connected?</div>
    <div class="file-item"><b>QUESTION 06</b><br>Did the Saints truly disappear?</div>
  </div>
  <p class="pull">“Every answer led to another name. Every name led back to Romano.”</p>
</section>

<section class="longread">
  <div class="kicker">THE ROMANO ARCHIVE</div>
  <h2>The Making Of A Los Santos Dynasty</h2>
  <p class="pull">“Every family has a beginning. The Romanos had a beginning—and then they had a legend.”</p>

  <div class="two-col">
    <p>The Romano Family did not emerge from a single grand event. It was assembled piece by piece in the aftermath of another family's collapse. When the Rizzo Family fell, Los Santos entered a familiar period of uncertainty: territory changed hands, alliances fractured, businesses changed ownership, and people who had once operated under one banner suddenly needed a new one.</p>
    <p>Garrison Romano understood that uncertainty. He had already lived the criminal life and knew what it demanded. But his ambition was different this time. The Romano name would not merely be another street organization. It would become a family name—something his children could inherit without inheriting every mistake he had made.</p>
    <p>Lyra Romano stood beside him through that transformation. If Garrison represented the family's hard edge, Lyra represented its center. Their household became the first true foundation of the Romano legacy. The children were encouraged to become their own people, and several eventually moved toward business and legitimate enterprise.</p>
    <p>That distinction became important later. The Romanos were never simply criminals trying to become businessmen. They were a family repeatedly trying to decide what the word “Romano” was supposed to mean.</p>
    <p>The answer changed with every generation.</p>
  </div>

  <div class="factbox">
    <h4>Archive Note — The Rizzo Connection</h4>
    <p>The Romano era begins immediately after the fall of the Rizzo Family. In Los Santos history, that transition is often treated as the opening chapter of the Romano story rather than a separate event. The Romanos inherited a city already shaped by the Rizzos—and spent the years that followed creating a legacy distinct from them.</p>
  </div>
</section>

<section class="longread">
  <div class="kicker">THE ROXWOOD FILE</div>
  <h2>A House Full Of Silence</h2>
  <div class="two-col">
    <p>Early 2024 should have been a year of consolidation for the Romanos. Instead, it became the year that permanently changed the family.</p>
    <p>The Romano home in Roxwood became the center of an investigation after Garrison and Lyra were found dead following a shooting. Their deaths immediately raised questions about Garrison's past. Who had he angered? Who might have wanted revenge? Had the former criminal ever truly escaped the world he claimed to have left behind?</p>
    <p>Investigators initially had every reason to look outward. A man with Garrison's history naturally creates enemies. But as the case developed, the possibility of an outside assassin began to fade.</p>
    <p>The most devastating answer was already inside the family.</p>
    <p>Korro Romano was eventually identified as the killer. The discovery turned the investigation into something far more personal than a conventional Los Santos homicide. The Romanos had not simply lost their patriarch and matriarch. They had lost them to one of their own.</p>
    <p>Yet even after the identity of the killer became known, the central question remained: why?</p>
    <p>No motive has ever adequately explained the violence. That absence has become part of the Romano mythology. Korro's intentions remain unknown, and the Roxwood murders continue to cast a shadow over every generation that followed.</p>
  </div>
  <div class="evidence">
    <div><strong>LOCATION</strong>Roxwood residence</div>
    <div><strong>VICTIMS</strong>Garrison &amp; Lyra Romano</div>
    <div><strong>PRIMARY SUSPECT</strong>Korro Romano</div>
    <div><strong>MOTIVE</strong>Still unknown</div>
  </div>
</section>

<section class="longread">
  <div class="kicker">THE SECOND GENERATION</div>
  <h2>Ivan Romano: The Reluctant Heir?</h2>
  <div class="two-col">
    <p>When Garrison died, the Romano Family lost more than its founder. It lost the person who had defined its original purpose. The next chapter belonged to Ivan Romano, Garrison's younger brother.</p>
    <p>Ivan inherited a name carrying both prestige and trauma. He was not stepping into a clean organization. He was stepping into the remains of a family whose first generation had been destroyed by one of its own.</p>
    <p>In early 2025, Ivan officially took control. Instead of keeping the family isolated, he entered the wider Los Santos underworld through The Kings.</p>
    <p>The Kings became the setting for another defining encounter. Ivan met Nadia King, and what began as time spent within the same organization gradually became a relationship that would change both of their lives.</p>
    <p>Then The Kings fell.</p>
    <p>For most people, the collapse of an organization would have meant starting over alone. Ivan and Nadia chose to start over together.</p>
  </div>
  <p class="pull">“The Kings ended. The Saints began. And the Romano name found its second great architect.”</p>
</section>

<section class="longread">
  <div class="kicker">LOS SANTOS UNDERWORLD</div>
  <h2>The Third Street Saints</h2>
  <div class="two-col">
    <p>The Third Street Saints began with two people who had already learned what happens when an organization collapses. Ivan Romano and Nadia King had watched The Kings disappear. They understood the importance of loyalty, structure, and reputation.</p>
    <p>The Saints were their answer.</p>
    <p>What followed was one of the fastest rises associated with the Romano name. The organization built a reputation as a serious street force and continued climbing until it was regarded as the number one street gang in the city's history.</p>
    <p>But the Saints' greatest strength was not simply their ability to command the streets. It was the personal mythology surrounding their leaders. Ivan and Nadia were partners in public and partners in private, and their marriage transformed Nadia from King to Romano.</p>
    <p>The new matriarch brought another generation into the story. Ivan and Nadia fostered children, and the family's attention gradually shifted from criminal organizations toward businesses and legitimate ownership.</p>
    <p>For a brief period, the Romano experiment seemed to have succeeded. Garrison's dream had finally become reality.</p>
  </div>
</section>

<section class="longread">
  <div class="kicker">THE ROMANO TRANSITION</div>
  <h2>When The Guns Went Quiet</h2>
  <div class="two-col">
    <p>There is a tendency to remember the Romanos only as criminals. The later years tell a more complicated story.</p>
    <p>Under Ivan and Nadia, the family increasingly moved toward business. Their children began establishing ventures of their own. The family name could be found attached to legitimate work rather than criminal organizations.</p>
    <p>It was not merely a change in occupation. It was an attempt to redefine inheritance.</p>
    <p>Garrison had wanted his children to inherit a family rather than a criminal empire. Ivan and Nadia appeared to be giving the next generation precisely that.</p>
    <p>Then the marriage collapsed.</p>
  </div>
  <div class="factbox">
    <h4>The Romano Paradox</h4>
    <p>The family's greatest successes repeatedly contained the seeds of its greatest failures. Every attempt to create stability produced a new chapter—and every new chapter eventually returned the Romanos to violence.</p>
  </div>
</section>

<section class="longread">
  <div class="kicker">LATE 2025 — FINAL BREAK</div>
  <h2>The Night Nadia Died</h2>
  <div class="two-col">
    <p>Late 2025 brought the final fracture between Ivan and Nadia Romano. Ivan discovered that his wife was having an affair.</p>
    <p>Whatever had been built between them—the Saints, the marriage, the family, the businesses, the future—was suddenly viewed through the lens of betrayal.</p>
    <p>Ivan killed Nadia.</p>
    <p>Detective Cole Locke caught Ivan red-handed, ending any immediate possibility that the crime would become another unsolved Romano mystery. Ivan was arrested and imprisoned.</p>
    <p>For the second time in the family's history, a Romano had killed someone inside the family. But this time, the killer was not an unknown child acting from an unexplained motive. It was the patriarch himself, standing at the center of the family he had spent years building.</p>
    <p>It was the moment the Romano dream finally appeared to be dead.</p>
  </div>
</section>

<section class="longread">
  <div class="kicker">CONFIDENTIAL — PRISON RECORD</div>
  <h2>The Escape</h2>
  <div class="two-col">
    <p>Then something happened that nobody expected.</p>
    <p>Ivan Romano escaped.</p>
    <p>The circumstances remain deliberately obscured. Unknown accomplices were responsible for breaking him out, but their identities have never been established publicly. Whether the escape was planned long before Ivan entered prison or improvised afterward remains one of the unanswered questions surrounding the family.</p>
    <p>And then Ivan disappeared.</p>
    <p>No confirmed sighting has settled the question of where the former Romano patriarch went. The family itself became increasingly quiet. People who once occupied the center of Los Santos' social and criminal landscape seemed to retreat from view.</p>
    <p>That silence created a new kind of Romano legend.</p>
    <p>There was no funeral for the name. No formal declaration that the family was finished. Just absence.</p>
  </div>
  <p class="pull">“The last chapter was never written. It simply stopped being published.”</p>
</section>

<section class="longread">
  <div class="kicker">THE FAMILY TREE</div>
  <h2>Blood, Marriage &amp; Legacy</h2>
  <div class="familytree">
    <div class="node red"><b>GARRISON ROMANO</b><br>Founder • Patriarch</div>
    <div>│</div>
    <div class="branch">
      <div class="node"><b>LYRA ROMANO</b><br>Matriarch</div>
      <div class="node"><b>THE ROMANO CHILDREN</b><br>Next generation • Business owners</div>
    </div>
    <div style="margin-top:6px">│</div>
    <div class="node red"><b>IVAN ROMANO</b><br>Garrison's younger brother • Second patriarch</div>
    <div>│</div>
    <div class="node"><b>NADIA ROMANO</b><br>Formerly Nadia King • Matriarch</div>
    <div>│</div>
    <div class="node"><b>FOSTERED CHILDREN</b><br>The next generation</div>
  </div>
</section>

<section class="longread">
  <div class="kicker">PEOPLE OF THE STORY</div>
  <h2>The Names Behind The Legend</h2>
  <div class="profile-grid">
    <article class="profile"><div class="role">THE FOUNDER</div><h3>Garrison Romano</h3><p>A notorious criminal who attempted to leave his past behind and build a family legacy. His murder in Roxwood made him the first great tragedy of the Romano dynasty.</p></article>
    <article class="profile"><div class="role">THE FIRST MATRIARCH</div><h3>Lyra Romano</h3><p>Garrison's wife and the center of the original Romano household. Her death alongside Garrison transformed the family forever.</p></article>
    <article class="profile"><div class="role">THE HEIR</div><h3>Ivan Romano</h3><p>Garrison's younger brother and second patriarch. He rebuilt the family through The Kings, The Third Street Saints, marriage, and legitimate business before his life collapsed into murder and escape.</p></article>
    <article class="profile"><div class="role">THE SECOND MATRIARCH</div><h3>Nadia Romano</h3><p>Born Nadia King, she became Ivan's partner, co-founder of the Third Street Saints, wife, and mother figure within the next generation of Romanos.</p></article>
    <article class="profile"><div class="role">THE UNKNOWN MOTIVE</div><h3>Korro Romano</h3><p>Garrison and Lyra's son, eventually identified as responsible for their deaths. His intentions remain one of the family's deepest mysteries.</p></article>
    <article class="profile"><div class="role">THE DETECTIVE</div><h3>Cole Locke</h3><p>The detective who caught Ivan red-handed following Nadia's death, becoming one of the final known law-enforcement figures connected directly to the Romano patriarch.</p></article>
  </div>
</section>

<section class="longread">
  <div class="kicker">THE UNANSWERED QUESTIONS</div>
  <h2>Six Mysteries That Remain</h2>
  <div class="evidence">
    <div><strong>01</strong>What truly motivated Korro to kill Garrison and Lyra?</div>
    <div><strong>02</strong>Did Garrison have enemies who played a role in the Roxwood tragedy?</div>
    <div><strong>03</strong>Who helped Ivan escape prison?</div>
    <div><strong>04</strong>Where did Ivan go after his escape?</div>
    <div><strong>05</strong>How much of the Romano business network remains active?</div>
    <div><strong>06</strong>Will another generation reclaim the Romano name?</div>
    <div><strong>07</strong>What really happened behind the scenes of the family's disappearance?</div>
    <div><strong>08</strong>Was Ivan's escape the end—or simply an intermission?</div>
  </div>
</section>

<section class="longread">
  <div class="kicker">EDITORIAL</div>
  <h2>The Romano Legacy</h2>
  <div class="two-col">
    <p>Every dynasty eventually reaches the point where its history becomes larger than the people who created it. The Romanos reached that point quickly.</p>
    <p>Garrison wanted family. Ivan wanted to carry the name. Nadia wanted to build beside him. Their children represented the possibility of a future without the criminal life that had defined the earlier generations.</p>
    <p>Yet the Romano name became trapped in a cycle: family, ambition, violence, silence, and reinvention.</p>
    <p>Garrison's death gave Ivan a legacy. Ivan's relationship with Nadia created the Saints. The Saints created a new Romano era. The affair destroyed that era. Ivan's escape transformed a murder case into a mystery.</p>
    <p>And now, the city waits.</p>
    <p>Maybe the Romanos are gone. Maybe they simply chose peace. Maybe the remaining family members are living ordinary lives far from the spotlight.</p>
    <p>Or maybe somewhere in Los Santos, behind a business front and an unremarkable door, the Romano name is still being spoken.</p>
    <p>Because if history has taught Los Santos anything, it is this:</p>
  </div>
  <p class="pull">A family can disappear from the city without disappearing from history.</p>
</section>

<section class="classified">
  <b>THE ROMANO FILES</b> • Some names, motives and events remain disputed. This special edition presents the known history as reconstructed from accounts surrounding the Romano Family.
</section>
</main>


<div class="modal case-modal" id="caseModal">
 <div class="modalbox">
  <button class="close" onclick="closeCase()">CLOSE ✕</button>
  <div class="case-paper" id="casePaper"></div>
 </div>
</div>

<div class="modal" id="modal">
 <div class="modalbox">
  <button class="close" onclick="closeModal()">CLOSE ✕</button>
  <h2 id="modalTitle"></h2>
  <p id="modalText"></p>
 </div>
</div>

<script>

const caseFiles={
roxwood:{
title:"CASE 24-001 — THE ROXWOOD MURDERS",status:"COLD CASE / FAMILY HOMICIDE",date:"EARLY 2024",
summary:"Two members of the Romano family are dead. The most disturbing lead eventually points to their own son.",
body:`<div class="file-section"><h4>INCIDENT</h4><p>Garrison and Lyra Romano were found dead following a shooting at their Roxwood residence. The deaths immediately attracted attention because of Garrison's criminal history and the possibility of retaliation from an old enemy.</p></div>
<div class="file-section"><h4>INVESTIGATIVE TURN</h4><p>As investigators reconstructed the family and its relationships, the case moved away from the theory of an outside attacker. Evidence and investigation eventually identified Korro Romano as the killer.</p></div>
<div class="file-section"><h4>THE UNANSWERED PART</h4><p>The motive remains unknown. That single missing piece has kept the case alive in Romano lore long after the identities involved became known.</p></div>
<div class="file-section"><h4>CASE NOTE</h4><p>Garrison and Lyra's deaths created the vacancy that eventually brought Ivan Romano into control of the family.</p></div>`
},
korro:{
title:"SUPPLEMENT 24-K — THE KORRO QUESTION",status:"MOTIVE UNKNOWN",date:"2024",
summary:"The identity of the killer was eventually established. The reason never was.",
body:`<div class="file-section"><h4>SUBJECT</h4><p>Korro Romano, son of Garrison and Lyra Romano.</p></div>
<div class="file-section"><h4>FAMILY CONTEXT</h4><p>Korro was not an outsider attacking a powerful family. He was part of the household. That fact made the Roxwood killings fundamentally different from the city's usual organized-crime cases.</p></div>
<div class="file-section"><h4>MOTIVE</h4><p>No confirmed motive has been established in the Romano record. Investigators can identify the “who” without fully explaining the “why.”</p></div>
<div class="file-section"><h4>DETECTIVE THEORY</h4><p>The unanswered motive became more important than the arrest itself. Every later Romano tragedy would be viewed through the shadow of Roxwood.</p></div>`
},
kings:{
title:"INTEL 25-I — IVAN ROMANO & THE KINGS",status:"ARCHIVED INTELLIGENCE",date:"EARLY 2025",
summary:"A new patriarch enters a new organization and meets the woman who will define his next chapter.",
body:`<div class="file-section"><h4>SUBJECT</h4><p>Ivan Romano, younger brother of Garrison Romano and newly established head of the family.</p></div>
<div class="file-section"><h4>ORGANIZATION</h4><p>Ivan joined The Kings after assuming control of the Romano Family. During his time there, he met Nadia King.</p></div>
<div class="file-section"><h4>RELATIONSHIP</h4><p>Ivan and Nadia gradually became close. When The Kings eventually fell, their relationship survived the organization that introduced them.</p></div>
<div class="file-section"><h4>OUTCOME</h4><p>The two would go on to establish The Third Street Saints, beginning the most powerful period of Ivan's public life.</p></div>`
},
saints:{
title:"ORG 25-TS — THE THIRD STREET SAINTS",status:"HIGH INTEREST ORGANIZED CRIME FILE",date:"2025",
summary:"Born from the collapse of The Kings, the Saints become the city's dominant street organization.",
body:`<div class="file-section"><h4>FOUNDERS</h4><p>Ivan Romano and Nadia King.</p></div>
<div class="file-section"><h4>RISE</h4><p>The Third Street Saints climbed the Los Santos power structure rapidly, developing a reputation for influence and organization until they were regarded as the number one street gang in the city's history.</p></div>
<div class="file-section"><h4>ROMANO CONNECTION</h4><p>The Saints and the Romano Family became increasingly intertwined as Ivan and Nadia's personal relationship deepened.</p></div>
<div class="file-section"><h4>TRANSFORMATION</h4><p>After Ivan and Nadia married, Nadia became Nadia Romano. The family then began moving toward fostering children, business ownership, and a life beyond criminal organizations.</p></div>`
},
nadia:{
title:"HOMICIDE 25-N — THE NADIA ROMANO CASE",status:"HOMICIDE / ARREST MADE",date:"LATE 2025",
summary:"The second great Romano family murder is committed by the patriarch himself.",
body:`<div class="file-section"><h4>BACKGROUND</h4><p>By late 2025, Ivan and Nadia had attempted to move the Romano family toward legitimate business and away from its criminal past.</p></div>
<div class="file-section"><h4>BREAKDOWN</h4><p>Ivan discovered that Nadia had been having an affair. The discovery ended their marriage and triggered the final collapse of their household.</p></div>
<div class="file-section"><h4>ARREST</h4><p>Ivan killed Nadia and was caught red-handed by Detective Cole Locke. He was taken into custody and imprisoned.</p></div>
<div class="file-section"><h4>SIGNIFICANCE</h4><p>The case echoed Roxwood in the most disturbing way possible: once again, the greatest danger to the Romano family came from within it.</p></div>`
},
escape:{
title:"ESC-25-IR — THE IVAN ROMANO ESCAPE",status:"ACTIVE LEAD / SUSPECT AT LARGE",date:"AFTER LATE 2025",
summary:"The suspect was imprisoned. Then someone opened the door.",
body:`<div class="file-section"><h4>PRISON STATUS</h4><p>Following Nadia's homicide, Ivan Romano was incarcerated.</p></div>
<div class="file-section"><h4>ESCAPE</h4><p>Unknown accomplices broke Ivan out of prison. Their identities, motives, and precise method remain unknown within the available Romano record.</p></div>
<div class="file-section"><h4>DISAPPEARANCE</h4><p>After the escape, Ivan's whereabouts became unknown. No confirmed account has established where he went.</p></div>
<div class="file-section"><h4>FAMILY STATUS</h4><p>The Romano Family subsequently became quiet. Few members were seen publicly, and the family appeared to retreat from Los Santos life.</p></div>
<div class="file-section"><h4>CASE ASSESSMENT</h4><p>For investigators, the escape created an ending without closure. Ivan was no longer in custody, but the Romano story was far from resolved.</p></div>`
}
};

function openCase(id){
 const f=caseFiles[id];
 document.getElementById("casePaper").innerHTML=`<div class="case-header"><div><div class="case-number">${f.title.split(" — ")[0]}</div><h2>${f.title}</h2></div><div class="case-meta"><b>${f.status}</b><br>${f.date}</div></div><p style="font-size:19px;line-height:1.5"><b>${f.summary}</b></p>${f.body}<div class="file-section"><h4>ARCHIVE WARNING</h4><p>This is an in-universe reconstructed case file for the Romano Family newspaper. Unknown details are intentionally preserved as mysteries for future stories.</p></div>`;
 document.getElementById("caseModal").classList.add("open");
}
function closeCase(){document.getElementById("caseModal").classList.remove("open")}
function reveal(el){el.textContent=el.textContent==="IDENTITY WITHHELD"?"IDENTITY STILL UNKNOWN":el.textContent==="LOCATION UNKNOWN"?"NO VERIFIED LOCATION":el.textContent==="INSUFFICIENT INFORMATION"?"NO CONCLUSIVE TRAIL":"STATUS UNCHANGED"}
function filterCases(){
 const q=document.getElementById("caseSearch").value.toLowerCase();
 document.querySelectorAll("#caseGrid .case-card").forEach(c=>c.style.display=c.dataset.search.includes(q)?"block":"none");
}
function scrollToId(id){document.getElementById(id).scrollIntoView({behavior:"smooth"})}
document.getElementById("caseModal").addEventListener("click",e=>{if(e.target.id==="caseModal")closeCase()});

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
