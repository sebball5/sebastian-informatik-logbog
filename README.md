
# Sebastian-informatik-logbog

<details>
  <summary><h1>Grundforløb</h1></summary>

  <details>
    <summary><h2>App og interaktionsdesign</h2></summary>
    vi valgte at lave en App for at sælge/reklamer for bilmærket Audi, vores mål var at apalere vores målgrubbe som vi identificerede som familie faren som både er moderne og pragmatisk, de skal også være vældhavende. (der kan også appaleres til unge mænd så som låner deres fars bil) <br>
    vores målgruppe placeret på minerva modellen ↓ <br>
<img width="564" height="411" alt="billede" src="https://github.com/user-attachments/assets/baf7950e-ce53-4d58-ae79-cfbc3839fec1" /><br>
den nuværende hjemmeside som vi gerne vil forbedre:<br> https://www.audi.dk/da/?utm_source=google&utm_medium=cpc&utm_campaign=audi&utm_content=brand&gad_source=1&gad_campaignid=737116201&gclid=EAIaIQobChMI5_uh6uDujwMVOIN8B <br>
    de dele fra websitet som vi mente skulles findes i jeres app. <br>
- Modeller info <br>
- Service og tilbehør info <br>
- Audi logo <br>
- Menu <br>
- Bruger <br>
<h3>Gestalt love</h3>
      Gestalt lovene fortæller om hvorvidt elementer på en hjemmesider passer som udvikleren tilsigtede.<br>
      Når lovene er overholdt er det nemmere for brugeren at benytte hjemmesiden, hvis ikke, er det modsat. <br>

<H4>Lovene er:</H4><br>

Loven om figur og baggrund <br>
Loven om nærhed  <br>
Loven om lighed  <br>
Loven om lukkethed  <br>
Loven om forbundethed  <br>
<h3>Prototyper</h3>
    vi bruge blandt andet crazy 8 metoden for at dele vores syn for hvordan vi synes appen skulle se ud.
<img width="564" height="411" alt="billede" src="https://github.com/user-attachments/assets/c14b8a5f-53ed-42cb-84f8-a75f4def6964" />
<img width="564" height="411" alt="billede" src="https://github.com/user-attachments/assets/28c65db2-bb9b-4703-be48-9bb00e0141d2" />
<img width="564" height="411" alt="billede" src="https://github.com/user-attachments/assets/da64d0b9-e103-49eb-89b4-3a3debbc8e19" />
<img width="564" height="411" alt="billede" src="https://github.com/user-attachments/assets/432dcdd5-e244-401a-b892-f85add4fdb19" /> <br>
derudover lavede vi også et flowcharts og et strukturdiagram så vi kunne se, og blive enige om, hvordan vores app skulle virke.

strukturdiagram ↓ <br>
<img width="564" height="411" alt="billede" src="https://github.com/user-attachments/assets/dd140abc-06dd-4f40-96ca-f7ef8a763a40" /> 

flowchart ↓ <br>
<img width="564" height="411" alt="billede" src="https://github.com/user-attachments/assets/3293a79d-1e7e-47e8-ab78-98053c6c638c" /> <br>
til sidst lavede vi en papir versionen af appen, for man kan rykke på papiret for at vise hvordan appen skulle interegere, jeg har mistede billede men burde kunne ses på videoen i brugertest.
<h3>Brugertest (think-aloud)</h3>
Tænke højt test gik fint, mangel på tilbageknap, Men nok fint bare at kunne swipe <br>
    link til videon af brugertesten ↓ <br>
https://tstaarhustech-my.sharepoint.com/personal/at25fbra_edu_aarhustech_dk/_layouts/15/stream.aspx?id=%2Fpersonal%2Fat25fbra%5Fedu%5Faarhustech%5Fdk%2FDocuments%2FOneNote%20Uploads%2FIMG%5F0302%2EMOV&ga=1&referrer=StreamWebApp%2EWeb&referrerScenario=AddressBarCopied%2Eview%2E50552b72%2D9ef2%2D40a2%2D82cd%2D0671c2eea405&isDarkMode=true 
<h3>Applab 06-11-25  </h3>
  <p> vores endelige produkt i Applab for at reklamer for Audi, vi endt med at lave forsiden, profilen og at kunne komme til siden hvor man logger ind, ikke det at logge ind, der hvor man kan søge uden søgefunctionen, og så laverede vi at man kunne navigere fra forsiden gennem burgermenuen, ind på bilmodeller, vælge elbiler og vælge Q4Etron og lidt information om den. selvom vi lavet at information om en bil, var det for at vise hvordan hjemmesiden skulle fungere.  <br>
  <img width="321" height="591" alt="billede" src="https://github.com/user-attachments/assets/982a1342-d09f-457f-8655-bab3c8c1536b" /><br>
  neden stående er linket til previewet af vores bilapp <br>
  https://studio.code.org/projects/applab/WskV32RwFC9BhJyZ__gj84eFpxl7lQAAoUFOrX0zxGc<br></p>
  
  <details>
  <summary><h3>Koden</h3></summary>
    
      onEvent("Profilbillede", "click", function() {
      setScreen("Profil");
    });
    onEvent("Logpå", "click", function() {
      setScreen("Profil.Loggetind");
    });
    onEvent("Menu", "click", function() {
      setScreen("Menubar");
    });
    onEvent("Menu.Bilmodller.Knap", "click", function() {
      setScreen("Menu-Bilmodeller");
    });
    onEvent("Elbil.Knap", "click", function() {
      setScreen("Bilmodeller-Elbil");
    });
    onEvent("Menu.Kundeservice.knap", "click", function() {
      setScreen("Menu-Kundeservice");
    });
    onEvent("Elbil.Q4", "click", function() {
      setScreen("Q4Etron");
    });
    onEvent("Søg", "click", function() {
      setScreen("Søgefunktion");
    });
    onEvent("Audilogo", "click", function() {
      setScreen("Forside");
    });
    onEvent("image7", "click", function() {
      setScreen("Forside");
    });
    onEvent("image13", "click", function() {
      setScreen("Forside");
    });
    onEvent("image21", "click", function() {
      setScreen("Forside");
    });
    onEvent("image2", "click", function() {
      setScreen("Forside");
    });
    onEvent("image11", "click", function() {
      setScreen("Forside");
    });
    onEvent("image16", "click", function() {
      setScreen("Forside");
    });
    onEvent("image32", "click", function() {
      setScreen("Forside");
    });
    onEvent("image1", "click", function() {
      setScreen("Forside");
    });

  </details>
  </details>
</details>
<details>
  <summary><h1>Informatik 1.g </h1></summary>
<details>
  <summary><h2>Programmering i heltal</h2></summary>
  <details>
    <summary><h3>Teori</h3></summary>
  <h4>Variabler</h4>
     <h4>Løkker</h4>
     <h4>Kontrolstruktur</h4>
    <h4>Lister</h4>
    <h4>Flowcharts</h4>
   </details>
  <details>
    <summary><h3>Mini Projekter</h3></summary>
  <h4>Sierpinski trekantskode</h4>
    https://editor.p5js.org/sebastian29/sketches/ceDRPV87D 
    <details>
      ```
      <summary>Koden</summary>
      var punkter = [];
const nedkølingstid = 1000;
let sidstenedkølingtidmitterpunkt = 0;
let sidstenedkølingtidslettepunkter = 0;
let sidstenedkølingskabepunkter = 0;
function setup() {
  createCanvas(400, 400);
}
function draw() {
  background(220);
  strokeWeight(10);
  for (let p of punkter) {
    point(p.x, p.y);
  }
  const nu = millis();
  if (
    punkter.length < 3 &&
    (nu - sidstenedkølingskabepunkter) > nedkølingstid
  ) {
    const nytpunkt = {
      x: random(width),
      y: random(height)
    };
    sidstenedkølingskabepunkter = nu;
    sidstenedkølingtidslettepunkter = nu;
    sidstenedkølingtidmitterpunkt = nu;
    punkter.push(nytpunkt);
  }
  else if (
    punkter.length === 3 &&
    (nu - sidstenedkølingtidmitterpunkt) > nedkølingstid
  ) {
    const i = floor(random(punkter.length));
    let j = floor(random(punkter.length));
    while (j === i) {
      j = floor(random(punkter.length));
    }
    const mitterpunkt = {
      x: (punkter[i].x + punkter[j].x) / 2,
      y: (punkter[i].y + punkter[j].y) / 2
    };
    punkter.push(mitterpunkt);
    sidstenedkølingtidmitterpunkt = nu;
    sidstenedkølingtidslettepunkter = nu;
    sidstenedkølingskabepunkter = nu;
    console.log("punkt 1:", i+1, "punkt 2:", j+1);
  }
  else if (
    punkter.length === 4 &&
    (nu - sidstenedkølingtidslettepunkter) > nedkølingstid
  ) {
    sidstenedkølingtidslettepunkter = nu;
    sidstenedkølingskabepunkter = nu;
    sidstenedkølingtidmitterpunkt = nu;
    punkter.splice(0, 3);
  }
}
      ```
    </details>
     <h4>Fysik simuleringskode</h4>
      https://editor.p5js.org/sebastian29/sketches/4fjYWHHm6 
      <details>
      <summary>Koden til første fysik simulering</summary>
let NyePunkter = [];

function setup() {
  createCanvas(600, 600);
}
function draw() {
  background(220);
  strokeWeight(10);

  for (let p of NyePunkter) {
    point(p.x, p.y);
    p.yv += p.ya;
    //p.xv += p.xa; 
    // ser fucker mærk lig ud med accelration
    p.y += p.yv;
    p.x += p.xv;
    if (p.y <= 10 || p.y >= height-10) {
      p.yv *= -0.98;
      //p.ya *= -0.98;
    }
    if (p.x <= 10 || p.x >= width-10) {
      p.xv *= -0.98;
      //p.xa *= -0.98;
    }
  }
  
for (let i = 0; i < NyePunkter.length; i++) {
    for (let j = i + 1; j < NyePunkter.length; j++) {
      let p = NyePunkter[i];
      let q = NyePunkter[j];
      let d = dist(p.x, p.y, q.x, q.y);
      if (d < 10) { 
        let tempXv = p.xv;
        let tempYv = p.yv;
        p.xv = q.xv;
        p.yv = q.yv;
        q.xv = tempXv;
        q.yv = tempYv;
      }
    }
} 
}
function mousePressed() {
  let NytPunkt = {
    x: mouseX,
    y: mouseY,
    yv: random(-2,2),
    xv: random(-2,2),
    xa: 0.1,
    ya: 0.1
  };
  NyePunkter.push(NytPunkt);
}
</details>
https://editor.p5js.org/sebastian29/sketches/ceDRPV87D 
      <details>
      <summary>Koden til anden fysik simulering med pool</summary>
        let NyePunkter = [];
const R = 7.5;   
const e = 0.9;    


let kugler = [
  { x: 111*3/2, y: 100, vx: 0, vy: 0, color: [255, 0, 0] },
  { x: 111*3/2+16, y: 100, vx: 0, vy: 0, color: [255, 255, 0] },
  { x: 111*3/2+32, y: 100, vx: 0, vy: 0, color: [255, 0, 0] },
  { x: 111*3/2-16, y: 100, vx: 0, vy: 0, color: [255, 255, 0] },
  { x: 111*3/2-32, y: 100, vx: 0, vy: 0, color: [255, 0, 0] },

  { x: 111*3/2-8, y: 113, vx: 0, vy: 0, color: [255, 255, 0] },
  { x: 111*3/2-16-8, y: 113, vx: 0, vy: 0, color: [255, 0, 0] },
  { x: 111*3/2+8, y: 113, vx: 0, vy: 0, color: [255, 255, 0] },
  { x: 111*3/2+16+8, y: 113, vx: 0, vy: 0, color: [255, 0, 0] },

  { x: 111*3/2, y: 126, vx: 0, vy: 0, color: [255, 255, 0] },
  { x: 111*3/2+16, y: 126, vx: 0, vy: 0, color: [255, 0, 0] },
  { x: 111*3/2-16, y: 126, vx: 0, vy: 0, color: [255, 255, 0] },

  { x: 111*3/2-8, y: 139, vx: 0, vy: 0, color: [255, 0, 0] },
  { x: 111*3/2+8, y: 139, vx: 0, vy: 0, color: [255, 255, 0] },

  { x: 111*3/2, y: 152, vx: 0, vy: 0, color: [255, 0, 0] },

  { x: 111*3/2, y: 400, vx: 0.1, vy: -33, color: [255, 255, 255] } // white ball 
];

let huller = [
  { x: 25, y: 25, r: 10 }, // top-left
  { x: 111*3 - 25, y: 25, r: 12.5 }, // top-right
  { x: 25, y: 183*3 - 25, r: 12.5 }, // bottom-left
  { x: 111*3 - 25, y: 183*3 - 25, r: 12.5 }, // bottom-right
  { x: 25, y: 183*3 / 2, r: 12.5 }, // left-center
  { x: 111*3 - 25, y: 183*3 / 2, r: 12.5 } // right-center
];

function setup() {
  createCanvas(111*3, 183*3);
  startBalls();
}
function draw() {
  background(24, 69, 25);
  drawEdges();
  strokeWeight(15);
  startBalls();
  updateBalls();
}

function startBalls() {
  for (let i = 0; i < kugler.length; i++) {
    stroke(kugler[i].color[0], kugler[i].color[1], kugler[i].color[2]);
    point(kugler[i].x, kugler[i].y);
  }
}

function updateBalls() {
  const edge = 25;

  for (let i = 0; i < kugler.length; i++) {
    kugler[i].x += kugler[i].vx;
    kugler[i].y += kugler[i].vy;
    if (kugler[i].x < edge + R) { kugler[i].x = edge + R; kugler[i].vx *= -e; }
    if (kugler[i].x > width - edge - R) { kugler[i].x = width - edge - R; kugler[i].vx *= -e; }
    if (kugler[i].y < edge + R) { kugler[i].y = edge + R; kugler[i].vy *= -e; }
    if (kugler[i].y > height - edge - R) { kugler[i].y = height - edge - R; kugler[i].vy *= -e; }
    kugler[i].vx *= 0.9935;
    kugler[i].vy *= 0.9935;
    if (abs(kugler[i].vx) < 0.09) kugler[i].vx = 0;
    if (abs(kugler[i].vy) < 0.09) kugler[i].vy = 0;
    for (let j = i + 1; j < kugler.length; j++) {
      const dx = kugler[j].x - kugler[i].x;
      const dy = kugler[j].y - kugler[i].y;
      const dist = Math.sqrt(dx * dx + dy * dy);
      if (dist > 0 && dist < 2 * R) {
        const nx = dx / dist;
        const ny = dy / dist;
        const overlap = 2 * R - dist;
        kugler[i].x -= overlap / 2 * nx;
        kugler[i].y -= overlap / 2 * ny;
        kugler[j].x += overlap / 2 * nx;
        kugler[j].y += overlap / 2 * ny;
        const vi = kugler[i].vx * nx + kugler[i].vy * ny;
        const vj = kugler[j].vx * nx + kugler[j].vy * ny;
        const diff = vi - vj;
        kugler[i].vx -= diff * nx;
        kugler[i].vy -= diff * ny;
        kugler[j].vx += diff * nx;
        kugler[j].vy += diff * ny;
      }
    }
  }

  for (let i = kugler.length - 1; i >= 0; i--) {
    for (let h = 0; h < huller.length; h++) {
      const dx = kugler[i].x - huller[h].x;
      const dy = kugler[i].y - huller[h].y;
      const dist = Math.sqrt(dx * dx + dy * dy);
      if (dist < huller[h].r) {
        if (i ===  15)
            {
              console.log("hvid kugle ramt i");
              kugler.splice(i, 1);
            }
        else 
        kugler.splice(i, 1);
        console.log("kugle "+i+" ramt i");
        break;
      }
    }
  }
}


function xyd (x1,y1,x2,y2)
{
  let xd = x1-x2;
  let yd = y1-y2;
  
  let d = sqrt(xd**2+yd**2) //yd**2 = yd^2
  return d;
}

function drawEdges()
{
  let edgeColour = {r:40, g:40, b:26}
  strokeWeight(15);
  stroke(edgeColour.r,edgeColour.g,edgeColour.b);
  fill(edgeColour.r,edgeColour.g,edgeColour.b);
  rect(0,0,111*3,20);
  rect(0,0,20,183*3);
  rect(0,183*3-20,111*3,183*3);
  rect(111*3-20,0,20,183*3);
  for (let i = 0; i < huller.length; i++) 
    {
      strokeWeight(25);
      stroke(edgeColour.r*2,edgeColour.g*2,edgeColour.b*2);
      point(huller[i].x,huller[i].y);
    }
}
function mousePressed() {
  console.log(mouseX+","+mouseY)
}
   </details>
</details>
<details>
  <summary><h2>kryptografi</h2></summary>
  <details>
    <summary><h3>Teori om kryptering bla sikkerhed</h3></summary>
  </details>
    <details>
    <summary><h3>Krypteringstyper</h3></summary>
  </details>
  <details>
    <summary><h3>Krypterings produkt</h3></summary>
  </details>
</details>
  <details>
  <summary><h2>3D design og print</h2></summary>
  <details>
    <summary><h3>Programmer</h3></summary>
  </details>
</details>
    <details>
  <summary><h2>Logbog i Github 16/2</h2></summary>
      </details>

