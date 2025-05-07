Descrierea jocului:

Jocul este un shooter 2D inspirat din clasicele jocuri de acțiune, în care jucătorul preia rolul unui soldat animat ce trebuie să lupte împotriva inamicilor într-o serie de nivele provocatoare. Fiecare nivel aduce noi obstacole și inamici, care devin tot mai dificili pe măsură ce avansezi. Jocul include un sistem de tragere dinamic, cu posibilitatea de a utiliza atât gloanțe, cât și grenade. Meniurile sunt animate, iar tranzițiile sunt fluide pentru a crea o experiență mai plăcută. Pe lângă acțiunea intensă, jocul beneficiază de o coloană sonoră captivantă și efecte audio care sporesc imersiunea, iar sistemul de inteligență artificială al inamicilor oferă provocări suplimentare. Fiecare moarte sau victorie este reflectată într-un meniu de restart sau win, menținând jucătorul implicat în fiecare moment al jocului.

🧱 Structura generală
Librării folosite: pygame, os, random, csv, button

Rezoluție: 800x640 pixeli

FPS: 60

🎮 Gameplay
Jucătorul controlează un soldat care se mișcă stânga-dreapta (A/D), sare (W), trage (SPACE) și aruncă grenade (Q).

Se pot colecta muniție, grenade și cutii de viață.

Există dușmani controlați de AI care trag în jucător.

Jucătorul moare dacă viața ajunge la 0 sau cade în apă.

🔧 Funcționalități importante
Clasa Soldier – definește jucătorul și inamicii:

Se poate mișca, sări, trage, arunca grenade.

Conține animații pentru acțiuni (Idle, Run, Jump, Death).

AI-ul pentru inamici detectează jucătorul și trage când e aproape.

Clasa World – gestionează harta și obstacolele, pe baza unui fișier CSV.

Tile-urile (plăcile) sunt încărcate și poziționate.

Creează entități precum apa, decorațiuni, obiecte, player, inamici.

Clasa Bullet și Grenade – proiectilele lansate:

Bullet: merge în direcția trasă și provoacă daune.

Grenade: sare, explodează după un timp, provoacă explozie.

Clasa ItemBox – obiecte ce pot fi colectate (ammo, grenades, health).

Clasa HealthBar – afișează bara de viață a jucătorului.

Clasa ScreenFade – efecte de tranziție între scene (intro și moarte).

🖱️ Meniu principal
Butoane pentru Start, Exit, și Restart (folosind o clasă Button externă).

Jocul începe doar după ce este apăsat Start.

🔁 Loop-ul principal de joc
Actualizează logica jocului (mișcare, coliziuni, trageri).

Desenează pe ecran toate entitățile.

Verifică dacă nivelul este complet sau jucătorul a murit.

Reîncarcă nivelul următor sau îl resetează.
