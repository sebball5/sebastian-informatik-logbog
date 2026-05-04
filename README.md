
# Sebastian-informatik-logbog

Der er først Datoer og ordenlig Logbog til emnerne arduino og tello drone. Desuden er der endelig kun ordenlig fyld til Grundforløb, Arduino og Tello. (da det er til de emner hvor jeg har skreven ordenlige noter), desuden har jeg også mistet nogen projekter (Jeg var ikke klar jeg skulle genbruge det) så der kan forkomme huller.

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
  Kryptering er en proces, der konverterer information til en kode for at forhindre uautoriseret adgang
  <details>
    <summary><h3>Teori om kryptering bla sikkerhed</h3></summary>
    `
    Kryptografi bygger på matematiske principper og anvendes for at sikre tre centrale elementer:
    <ul>
      <li><strong>Fortrolighed</strong> – kun autoriserede personer kan læse informationen</li>
      <li><strong>Integritet</strong> – data må ikke kunne ændres uden at det opdages</li>
      <li><strong>Autenticitet</strong> – man kan verificere, hvem der har sendt data</li>
    </ul>
    Et sikkert kryptosystem antager, at algoritmen er kendt, men at nøglen er hemmelig
    (Kerckhoffs’ princip).

  </details>
    <details>
    <summary><h3>Krypteringstyper</h3></summary>
      
#### Symmetrisk Kryptering
Forklaring: Symmetrisk kryptering er kryptering, hvor afsender og modtager skal bruge den samme nøgle: Afsender krypterer med nøglen, modtager dekrypterer med nøglen.
##### Cæsar kryptering:
`
     Cæsar-kryptering er en af de ældste krypteringsmetoder. Den fungerer ved at forskyde hvert bogstav 
      i alfabetet et fast antal pladser. Metoden er dog meget usikker og bruges kun til undervisning.
##### DES og AES
`
      DES (Data Encryption Standard) var tidligere en standard, men regnes i dag for usikker.
      AES (Advanced Encryption Standard) er en moderne og meget sikker symmetrisk algoritme,
      som bruges i bl.a. WiFi, harddiskkryptering og VPN-forbindelser.
#### Asymmetrisk kryptering 
Forklaring: Kryptering, hvor afsender og modtager hver har sit eget sæt nøgler, en privat nøgle og en offentlig nøgle. Den private nøgle er hemmelig og kun kendt af ejermanden, mens alle har adgang til at se den offentlige nøgle. Data krypteret med den offentlige nøgle kan kun dekrypteres med den private nøgle. 
##### RSA 
RSA fungerer ved at generere et nøglepar, der bruges til at beskytte information. Først vælges to store primtal, som ganges sammen for at danne en modulus, der er en del af både den offentlige og private nøgle. Når en afsender vil sende en sikker besked, bruger vedkommende modtagerens offentlige nøgle til at kryptere den. Kun modtagerens private nøgle kan derefter dekryptere beskeden og gøre den læsbar.

Ud over at beskytte kommunikation bruges RSA også til digitale signaturer, hvor afsenderen signerer en besked med sin private nøgle. Modtageren kan derefter verificere signaturen med afsenderens offentlige nøgle, hvilket sikrer, at beskeden er autentisk og ikke er blevet ændret undervejs. Denne metode bruges ofte i officielle dokumenter, softwareopdateringer og finansielle transaktioner.
##### HTTPS (Hypertext Transfer Protocol Secure)
HTTPS er en sikker version af HTTP og bruges til sikker kommunikation på internettet.
      HTTPS anvender kryptering (TLS/SSL) til at beskytte data, der sendes mellem browser og webserver,
      f.eks. adgangskoder og betalingsoplysninger
  </details>
  <details>
    <summary><h3>Krypterings produkt</h3></summary>
    Jeg kan ikke frembringe det igen, ved ikke hvor det er
  </details>
</details>
</details>
  <details>
  <summary><h2>3D design og print</h2></summary>
  <details>
    <summary><h3>Programmer</h3></summary>
  </details>
</details>
<details> 
  <summary><h2>arduino 02-03-2026 -> 10-04-2026 </h2></summary>
  Resume: Arduino som måler Luftkval og automatisk laver grafer
  # Arduino-projekt-1
Første arduino projekt 
af August, Emilie og Sebastian

# Problemformulering 
I vores klasseværelse er der ofte tung luft, meget støj og en kvælende temperatur. Dette forringer vores læringsevne ret markant, da det er svært at koncentrere sig og holde fokus når omgivelserne er dårlige. Vi vil derfor gerne undersøge luftkvaliteten, lydniveauet, temperaturen og mængden af fugt ved hjælp af en Arduino. Vi vil gerne undersøge sammenhængen mellem de forskellige faktorer, om der er forskel i pauserne vs. timerne (og dermed om faktorerne påvirkes markant af ændringer i lokalet som fx. mængden af mennesket og om vinduet er åbent) og om vi eventuelt kommer over nogle grænseværdier, som vi derefter kan forbedre enten selv eller ved at få lavet markante ændringer i klasselokalet.

# Powerpoint præsentation 

https://tstaarhustech-my.sharepoint.com/:p:/g/personal/at25sesj_edu_aarhustech_dk/IQDQW1roxacjSZUCvhoZm9N9AdtN3fWhZ4f2LsHmY900V4c?e=reZSht
skreven kort om vores præsentation mangler vi

# Flowchart 
Link til flowchart lavet i Miro ↓

https://miro.com/welcomeonboard/MHlqSzBMOTVPWXNoTlNaUFZjUjZzQ0VDeG5VWFA1b2R2UDF1SW1yS3JMaGE4M25BcWZmSGE5Q0xIcFp1WitxdGIvb1VlblY4WlVMWlZtclFnN1l4NTZSTVhMdVhWaGxTMnhZSjNDWkFFa09QRmE1ZmdBVElQZWhsT3hwMlgzbnNNakdSWkpBejJWRjJhRnhhb1UwcS9BPT0hdjE=?share_link_id=627217930046 
<details> <summary><h2>Koden</h2></summary>

## Arduino 
```cpp
//luft kval måler
#define SDA_PORT PORTD
#define SDA_PIN 2
#define SCL_PORT PORTD
#define SCL_PIN 3
#define I2C_SLOWMODE 1
#define DHTPIN 4
#define DHTTYPE DHT22

#include <SoftI2CMaster.h>
#include <Wire.h>
#include "Adafruit_SGP30.h"
#include "DHT.h"

Adafruit_SGP30 sgp;
unsigned long startTid;
DHT dht(DHTPIN, DHTTYPE);

void setup() {
  Serial.begin(9600);
  dht.begin();
  while (!Serial) { delay(10); }

  i2c_init();

  if (!sgp.begin()) {
    Serial.println("FEJL: SGP30 ikke fundet! Tjek D2/D3 tilslutning.");
    while (1);
  }

  startTid = millis();
  Serial.println("Tid_sek,eCO2_ppm,TVOC_ppb,Status_nr,Status_tekst,dB,C°,RL");
}

void loop() {
  if (!sgp.IAQmeasure()) {
    delay(1000);
    return;
  }

  float tid = (millis() - startTid) / 1000.0;
  float h = dht.readHumidity();
  float t = dht.readTemperature();

  // Tjek om DHT-aflæsning lykkedes
  if (isnan(h) || isnan(t)) {
    Serial.println("FEJL: Kunne ikke læse fra DHT-sensor!");
    delay(1000);
    return;
  }

  int eco2 = sgp.eCO2;
  int tvoc = sgp.TVOC;

  int statusNr;
  String statusTekst;

  if (eco2 < 800) {
    statusNr = 1; statusTekst = "God";
  } else if (eco2 < 1500) {
    statusNr = 2; statusTekst = "Moderat";
  } else {
    statusNr = 3; statusTekst = "Darlig";
  }

  int dB = 1; // stadig placeholder

  Serial.print(tid, 1);       Serial.print(",");
  Serial.print(eco2);         Serial.print(",");
  Serial.print(tvoc);         Serial.print(",");
  Serial.print(statusNr);     Serial.print(",");
  Serial.print(statusTekst);  Serial.print(",");
  Serial.print(dB);           Serial.print(",");
  Serial.print(t, 1);         Serial.print(",");  // <-- rigtig temperatur
  Serial.println(h, 1);                           // <-- rigtig luftfugtighed

  delay(1000);
}
```
## Python 
```py
import serial
import time
import os, sys
from datetime import datetime
from openpyxl import load_workbook

COM_PORT  = "COM4"
BAUD_RATE = 9600
pathname = os.path.abspath(os.path.dirname(sys.argv[0]))
EXCEL_FIL = "SGP30_Data.xlsx"
EXCEL_FULL_PATH = os.path.join(pathname,EXCEL_FIL)
GEM_HVERT = 10

def main():
    print("SGP30 -> Excel Logger")

    print(f"Åbner: {EXCEL_FULL_PATH}")
    if not os.path.exists(EXCEL_FULL_PATH):
        print(f"Kunne ikke finde '{EXCEL_FULL_PATH}'")
        input("Tryk Enter...")
        return

    print(f"Forbinder til {COM_PORT}...")
    try:
        ser = serial.Serial(COM_PORT, BAUD_RATE, timeout=2)
        time.sleep(2)
        print("Forbundet! Koerer... tryk Ctrl+C for at stoppe\n")
    except serial.SerialException:
        print(f"Kunne ikke forbinde til {COM_PORT}")
        input("Tryk Enter...")
        return

    wb = load_workbook(EXCEL_FULL_PATH)
    ws = wb["Data"]

    naeste_gem = time.time() + GEM_HVERT
    naeste_row = 2

    try:
        while True:
            line = ser.readline().decode("utf-8", errors="ignore").strip()	
            print(f"DEBUG: '{line}'")
            if not line or "Tidspunkt" in line or "FEJL" in line:
                continue
            parts = line.split(",")
            if len(parts) < 8:
                continue

            try:
                eco2      = int(parts[1])
                tvoc      = int(parts[2])
                status_nr = int(parts[3])
                status    = parts[4].strip()
                dB        = int(parts[5])
                temp      = float(parts[6])
                humidity  = float(parts[7])
            except ValueError:
                continue

            tidspunkt = datetime.now().strftime("%H:%M:%S")

            ws.cell(row=naeste_row, column=1, value=tidspunkt)
            ws.cell(row=naeste_row, column=2, value=eco2)
            ws.cell(row=naeste_row, column=3, value=tvoc)
            ws.cell(row=naeste_row, column=4, value=status_nr)
            ws.cell(row=naeste_row, column=5, value=status)
            ws.cell(row=naeste_row, column=6, value=dB)
            ws.cell(row=naeste_row, column=7, value=temp)
            ws.cell(row=naeste_row, column=8, value=humidity)
            naeste_row += 1

            print(f"  {tidspunkt} | eCO2: {eco2:>5} ppm | TVOC: {tvoc:>4} ppb | dB: {dB:>4} | Temp: {temp:>3}C | Fugt: {humidity:>5.1f}% | {status}")

            if time.time() >= naeste_gem:
                wb.save(EXCEL_FULL_PATH)
                print(f"  [GEMT] {datetime.now().strftime('%H:%M:%S')}")
                naeste_gem = time.time() + GEM_HVERT

    except KeyboardInterrupt:
        print("\nStopper...")
    finally:
        wb.save(EXCEL_FULL_PATH)
        ser.close()
        print("Faerdig! Aaben SGP30_Data.xlsx og tjek Data fanen.")
        input("Tryk Enter...")

if __name__ == "__main__":
    main()
```
</details>
<details>
<summary><h2>Logbog for Arduino Emnet </h2></summary>


  ## 02-03-2026 <br>
  Arduino IDE 
  x = digital read, så er x = 0 eller 1, altså low eller high
  pinmode (5, input_pullup) 
  x =digital read(5), hvis x 
Arduino
Er open source: alle må bygge en, kode en, etc.
Man kan sætte ledninger i og kode og få processoren til at gøre ting.
i arduino IDE tjekker verify for fejl mens upload uploader
Noget med analog...
ADC
0V --> 0
2,5V --> 511
5V --> 1023
Pins har TO funktioner: inputs/outputs    kaldes GPIO: General Purpose, input/output
Flowcharts er en god idé
Blokdiagrammer kan gøre ting mere overskuelige. Man deler de forskellige dele op og gør det mere overskueligt.
ArduinoIDE: appen man koder i
For kode-viden, se "programmering". Der er også noter fra introduktionen til Arduino fra grundforløbet.
Setup kører én gang.
Loop kører forever (kaldes draw i p5js).
BUILTIN bruges til at snakke om en indbygget pin/led/andet
funktion: PinMode (#, x)   x = input eller output. # = hvilken pin
Måder den kan tale med omverdenen på...:
x = DigitalRead(#)     x = 0/1 el. low/high    så aflæser den en specifik pin
AnalogRead ()     konverterer tal rundt
Protokol: når man skal sende data, og ikke bare tænd/sluk ex.
  i library i arduino IDE, kan man intallere eksempler fra et bibliotek, eksemplet mark gav var at søge på accelaratometer og så finder den en til en.
  det er en dum ide at give en AI chatbot, hele projektet på en gang, men at bryde den op i bider. for at hjælpe med at forstå ens kode kan man bruge flowcharts og blokdiagrammer.
  
  få at teste ovenstående teori vil et lave et program i arduino IDE, hvor man trykker på knappen tændes en led.
  til at starte indeholde arduinoen allerede kode fra det sidste projekt den er bleven brugt, dette vil vi gerne have væk, derfor resetter den.
  så går vi ind i eksempler i arduino IDE hvor vi finde BLINK og sætter os ind i koden.
  vi vil ændre så at LEDen lyser når man trykker på en knap, vi finder et eksemple i Arduino IDE og så ændre vi inputne og outputne, så virker med vores huller
  // constants won't change. They're used here to set pin numbers:
const int buttonPin = A4;  // the number of the pushbutton pin
const int ledPin = 13;    // the number of the LED pin
```
// variables will change:
int buttonState = 0;  // variable for reading the pushbutton status

void setup() {
  // initialize the LED pin as an output:
  pinMode(ledPin, OUTPUT);
  // initialize the pushbutton pin as an input:
  pinMode(buttonPin, INPUT);
}

void loop() {
  // read the state of the pushbutton value:
  buttonState = digitalRead(buttonPin);

  // check if the pushbutton is pressed. If it is, the buttonState is HIGH:
  if (buttonState == HIGH) {
    // turn LED on:
    digitalWrite(ledPin, LOW);
  } else {
    // turn LED off:
    digitalWrite(ledPin, HIGH);
  }
  ```
## Brainstorm 06-03-2026

Typer af sensorere vi kan bruge: afstand, infrarød, motion sensor, fugt, temperatur, luft kvalitet, gas, menneske radar, touch, vibration/kollision/bevægelse, støv, afstand, ultralyd, vægt, magnet, fugt, encoders, lyd, kraft, puls  

Vi vil gerne lave noget til klasseværelset. 

### Første ide: 

Klasseværelses måler, en måler der måler alt der påvirker et klasseværelse, så som luftkvalitet, temperatur, fugt, lyd, gas, måske mængde mennesker (er der for mange mennesker etc.).

### Anden ide: 

Hvordan påvirker dårlig luft dem i klasseværelset? Vi vil måle luftkvalitet og gas og så et par andre parametre, såsom lyd/støj, temperatur, mængde mennesker (går folk væk hvis luften er shit).

### Tjerde ide:

Plante-vander, vander John Newton (vores plante) hver gang jorden bliver for tør.

### Fjerde ide: 

En bil der kan suse rundt i klassen, (nok lidt uden for vores niveau).

### Femte ide: 

Roomba til klassen, tror ikke vi har noget til at suge, men vi kan måle støv og distance til væggen.

### Sjette ide: 

Menneske logger, ved hjælp af menneske radar kunne vi tjekke hvornår folk mødte ind.

### Syvende ide: 

Sidder man ordenligt-sensor

### Ottende ide: 

Flappy bird ud fra lyd/lys eller luft kvalitet.

## Lyskrydsmetoden til ovenstående ideer. 06-03-2026

Første ide, black box over alt i klasse ![](https://img.shields.io/badge/GOD-grøn-green)

Anden ide, stort set første ide ![](https://img.shields.io/badge/GOD-grøn-green)

Tjerde ide, vande newton (andre går med den ide) ![](https://img.shields.io/badge/GOD-grøn-green)

Fjerde ide, en bil der kører rundt i klassen![](https://img.shields.io/badge/MODERAT-gul-yellow)

Femte ide, ligesom bilen men virker som støvsuger, altså en roomba ![](https://img.shields.io/badge/MODERAT-gul-yellow)

Syvende ide, hvorvidt man sidder ordenligt på en stol og om man sidder for lang tid på den ![](https://img.shields.io/badge/DÅRLIG-rød-red)

Ottende ide, flappy bird ud fra en sensor ![](https://img.shields.io/badge/DÅRLIG-rød-red)

## Ideen valgt 06-03-2026

Vi har valgt at køre med den første/anden ide, nu skal vi så finde ud af hvad vi skal bruge.

Sensorne vi gerne vil bruge, vi vil gerne måle luftkval og gasser (eventuelt menneske sensor i døren som tæller hver gang man går ind eller ud) , hvordan de påvirker så meget andet. det andet er støj, temperatur lufttryk, fugt 

så luftkval, gasser og menneske radar

og støj, temperatur, lufttryk og fugt

# Det vi har lånt

- En Arduino med overdel

- Ledning så den kan gå i computeren

- VOC and eCO2 Sensor (SGP30) v1.1

- Grove-LCD RGB Backlight V4.0

- Sound Sensor v1.6

- Temperature&Humidity Sensor Pro v1.3

- MicroPressureSensor

- En lilla dimmelut Mark gav os


## Logger pro. 06-03-2026

Nu vi gerne skrive et kort program i arduino, og vise dataen i logger pro 

starter med at prøve at måle gas med VOC and eCO2 Gas Sensor (SGP30) v1.1 og vise dataen i loggerpro

Vi brugte Claude, her er Claudes forklaring (forfines senere men lige nu skal python virke og det er vigtigere):

Vi har sat en SGP30 gassensor op på vores Arduino Uno, som måler luftkvalitet i form af eCO2 (kuldioxid) og TVOC (flygtige organiske forbindelser) i klasseværelset. Sensoren er tilsluttet via I2C på pin D4 og D5. For at få dataen ind i vores computer har vi skrevet et Python-script, der automatisk læser målingerne fra Arduino og gemmer dem direkte i en Excel-fil med grafer, så vi kan følge med i luftkvaliteten over tid. Scriptet starter automatisk med et enkelt dobbeltklik og kræver ingen manuel indgriben undervejs.

## Problemformulering (12-03-2026)

I vores klasseværelse er der ofte tung luft, meget støj og en kvælende temperatur. Dette forringer vores læringsevne ret markant, da det er svært at koncentrere sig og holde fokus når omgivelserne er dårlige. Vi vil derfor gerne undersøge luftkvaliteten, lydniveauet, temperaturen og mængden af fugt ved hjælp af en Arduino. Vi vil gerne undersøge sammenhængen mellem de forskellige faktorer, om der er forskel i pauserne vs. timerne (og dermed om faktorerne påvirkes markant af ændringer i lokalet som fx. mængden af mennesket og om vinduet er åbent) og om vi eventuelt kommer over nogle grænseværdier, som vi derefter kan forbedre enten selv eller ved at få lavet markante ændringer i klasselokalet.

## flowchart (12-03-2026)
https://miro.com/welcomeonboard/MHlqSzBMOTVPWXNoTlNaUFZjUjZzQ0VDeG5VWFA1b2R2UDF1SW1yS3JMaGE4M25BcWZmSGE5Q0xIcFp1WitxdGIvb1VlblY4WlVMWlZtclFnN1l4NTZSTVhMdVhWaGxTMnhZSjNDWkFFa09QRmE1ZmdBVElQZWhsT3hwMlgzbnNNakdSWkpBejJWRjJhRnhhb1UwcS9BPT0hdjE=?share_link_id=627217930046
Miro
Miro | The Visual Workspace for Innovation
Miro is a visual workspace for innovation where teams manage projects, design products, and build the future together. Join 60M+ users from around the world.
Billede 


## kode for i dag (23/3):
```cpp
#define SDA_PORT PORTD
#define SDA_PIN 2
#define SCL_PORT PORTD
#define SCL_PIN 3
#define I2C_SLOWMODE 1
#define DHTPIN 4
#define DHTTYPE DHT22
#define lydpin A0

#include <SoftI2CMaster.h>
#include <Wire.h>
#include "Adafruit_SGP30.h"
#include "DHT.h"

Adafruit_SGP30 sgp;
unsigned long startTid;
DHT dht(DHTPIN, DHTTYPE);

void setup() {
  Serial.begin(9600);
  dht.begin();
  while (!Serial) { delay(10); }

  i2c_init();

  if (!sgp.begin()) {
    Serial.println("FEJL: SGP30 ikke fundet! Tjek D2/D3 tilslutning.");
    while (1);
  }

  startTid = millis();
  Serial.println("Tid_sek,eCO2_ppm,TVOC_ppb,Status_nr,Status_tekst,dB,C°,RL");
}

void loop() {
  if (!sgp.IAQmeasure()) {
    delay(1000);
    return;
  }

  float tid = (millis() - startTid) / 1000.0;
  float h = dht.readHumidity();
  float t = dht.readTemperature();

  // Tjek om DHT-aflæsning lykkedes
  if (isnan(h) || isnan(t)) {
    Serial.println("FEJL: Kunne ikke læse fra DHT-sensor!");
    delay(1000);
    return;
  }

  int eco2 = sgp.eCO2;
  int tvoc = sgp.TVOC;
  int statusNr;
  int dB = analogRead(lydpin);

//long sum = 0;
//for(int i=0; i<32; i++)
//{
//    sum += analogRead(lydpin);
//}
//sum = sum / 32;

  String statusTekst;

  if (eco2 < 800) {
    statusNr = 1; statusTekst = "God";
  } else if (eco2 < 1500) {
    statusNr = 2; statusTekst = "Moderat";
  } else {
    statusNr = 3; statusTekst = "Darlig";
  }


  Serial.print(tid, 1);       Serial.print(",");
  Serial.print(eco2);         Serial.print(",");
  Serial.print(tvoc);         Serial.print(",");
  Serial.print(statusNr);     Serial.print(",");
  Serial.print(statusTekst);  Serial.print(",");
  Serial.print(dB);           Serial.print(",");
  Serial.print(t, 1);         Serial.print(",");  
  Serial.println(h, 1);                           

  delay(1000);
}
```
Udover ovenstående er vi nået langt. Gangen før var Sebastian fraværende, så vi brugte lang tid på at få downloadet de nødvendige programmer og udvidelser på Emilies computer. I dag har August og Emilie brugt tid på at tilslutte en lyd-sensor, rette i koden og forsøge at kalibre den, sådan at vi får værdierne i dB (pt giver den bare rå ACD data, som er en måling af elektriske impulser). Derudover har vi i fællesskab fået Excel til at fungere sådan, at vi kan se den opdatere live i stedet for at crashe programmet hver gang den starter op.

## 08-04-2026

Idag vil vi gerne have designet vores kasse. så det ser lidt bedrer ud end bare en arduino plade med en masse ledningerne der stikker op, mark har også sagt at vi skal have forberet en præsentation af vores projekt så det skal vi have gjort til på fredag.

vi bruger autodesk fusion til at lave og designe vores kasse
den nuværende design ide lavet i microsoft paint: 
<img width="1157" height="664" alt="image" src="https://github.com/user-attachments/assets/b582a9d7-60bf-4e40-9d35-f84777808a2f" />

#### resume af dagen:

vi har fået lavet kassen, med huller til ledningerne og lommer til målerne på siden. det tog lang tid da målene af måleren skulle være ret præcise da vi gerne vil ha at den ligger indeni uden at rumstere alt for meget.

derudover at vi også startet på præsentation, hvor vi har udtænkt at den skal indeholde: forside, disposition, hvad projektet handler om, hvordan vores virker, demostration at den virker, opsamling på vores data og projekt.
vi er ikke nået særligt langt med det præcise indhold at de forskellige punkter. men vi vil gerne præsentere på klassen (der skulle ikke være tid til at alle kan præsentere), nu vi jo har lavet projektet og eneligt er kommer fint i mål:

##### kassen:

<img width="1113" height="512" alt="image" src="https://github.com/user-attachments/assets/0ba7226a-51e5-4d8f-9309-230a447d85ab" />

##### kassen med forklaringer:

<img width="1372" height="625" alt="image" src="https://github.com/user-attachments/assets/e512a018-f2e9-4bc1-9628-82b1e1e4229c" />


## 09-04-2026

#### dagen program: 

vi skal have printet vores kasse, taget målinger af klassen så vi har noget data at præsentere, lavet præsentationen så vi er klar i morgentidlig.

#### Resume af dagen

Vi har sat kassen til at printe, så den er klar til i morgen tidlig. Derudover har vi foretaget en række målinger så vi har nogle grafer vi kan præsentere. Præsentationen er lavet i powerpoint, alle slides er lavet med stikord.

## 10-04-2026

#### Dagens program 

i dag skal vi have præsenteret vores projekt med vores powerpoint, derudover skal vi også være færdig med alt andet. SIDSTE DAG

#### Resume af dagen


</details>
   </details>
  <details> 
  <summary><h2>Tello projekt 28-04-2026 -> </h2></summary>
    Tello projekt, med Sander, Sebastian og Sylvester. <Br>
    Resume: Dronen som flyver efter tyske kommandoer
    
LINK til miro 

https://miro.com/app/board/uXjVHb_tvd0=/ 

 ### Problemformulering

Vi vil meget gerne lave en nemmere måde at styre dronen på, da den lige nu skal programeres, det vil vi gerne ændre til en mere brugervenlig overflade.
     <details> 
    <summary><h2>Kode </h2></summary>
      
       import speech_recognition as sr
r = sr.Recognizer()

from djitellopy import Tello
import time

Tello.connect()
print("Battery:", Tello.get_battery())

while True:
    try:
        with sr.Microphone() as source:
            print("lytter.......")
            
            #gør så den lytter efter, selvom der er støj i rummet
            r.adjust_for_ambient_noise(source, duration=0.2)
            #lytter til havd man siger
            audio = r.listen(source)
            #sammenligner lyden til google tyske lydbibilotek
            text = r.recognize_google(audio, language="de-DE")
            #lovercaser teksten
            text = text.lower()  

            print("Du sage:", text)

            if(text == "abheben"):
                Tello.takeoff()

            elif(text == "hoch"):
                Tello.move_up(50)
            
            elif(text == "runter"):
                Tello.move_down(50)

            elif(text == "vorwarts"):
                Tello.move_forward(50)
            
            elif(text == "ruckwarts"):
                Tello.move_back(50)

            elif(text == "rechts"):
                Tello.move_right(50)
            
            elif(text == "links"):
                Tello.move_left(50)

            elif(text == "israel"):
                Tello.land


            
            if "exit" in text:
                print("slukker programmet:")
                break

    except sr.RequestError as e:
        print("gad kke virke {0}".format(e))

    except sr.UnknownValueError:
        print("kunne ikke forstå dig")

    except KeyboardInterrupt:
        print("program slukket")
        break 
        

   
</details>
  <details> <h3>Logbog</h3>

28-04-2026 
    
Intro til otello drone projekt. 

Dronen er meget sikker, samt hvordan man koder til den. 
Så fik vi også vist marks plan for emnet, noget med gestalt love, noget med trelags modellen. 
Vi skal starte et projekt omkring dronerne, målet er at lave et program som kan styre en drone (rimeligt løst emne) 
I Grupperne skal der være fælles dokumenter (Ala Miro, trello og GitHub.), vi skal også skrive en problemformulering og forstå droner og mulighederne. 
 
 30-04-2026
 
Dagens humør:
Vi er håbefulde

Dagens program:

Vi vil gerne undersøge python commands så vi kan lave lyd om til commands som dronen kan følge. 
Vi skal også finde simple prombts til at videregive så meget information som muligt, uden at skulle råbe en længere sætning af dronen.
 
Hvad nået vi i dag: 

Vi fik skrevet et python program der opfanger lyd og sammenligner det med googles tyske lyd bibliotek
Samt lavet elif statement to at converter det til commands for dronen


04-05-2026

Vi er fortsat håbefulde 

Dagensprogram:

Vi vil gerne nå at få dronen til at kunne flyve i dag, det kræver en USB internet adapter så vi kan både være connected til dronen og internettet (for APIen), 
Hvad vi nået idag:
Vi fik ikke drone i vejret grundet lidt bøvl med internet og dronen, men vi fik lidt diagrammer såsom trelagsmodellen, client-server modellen, flowchart og blokdiagram. 

### Flowchart

<img width="625" height="706" alt="image" src="https://github.com/user-attachments/assets/a3c96fa9-6700-4ac7-a006-f852dd1487ef" />

flowchartet delt i 2, den øverste del til venstre, den nederste til højer

### Blokdiagram

<img width="975" height="494" alt="image" src="https://github.com/user-attachments/assets/a7bf5324-f86e-4d55-9656-38aa75482729" />

som der ses på blokdiagrammet snakker manden tysk, computerens mikrofon opfanger det og sender det til google API tyske lydbibliotek. Lydbibilioteket registrere så hvilken lyd det er og skriver det tilbage til computeren. computeren tjekker så hvilken command der korropondere til lyden, dronen aflyder så ordren.

### Trelags model 

<img width="653" height="700" alt="image" src="https://github.com/user-attachments/assets/e41fe399-95d0-47fc-8aeb-e22d6fa81a2d" />

### Client- Server akitektuktur

<img width="975" height="364" alt="image" src="https://github.com/user-attachments/assets/16c4743b-b10c-439d-b80f-f01b7ff85b52" />

  </details>
  </details>
</details>
