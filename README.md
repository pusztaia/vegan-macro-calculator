# 🌱 Vegán Makró & Étrend Tervező (Vegan Macro Calculator)

Növényi étrendre optimalizált kalória-, makrotápanyag- és étkezéstervező mindenkinek, bekapcsolható **Sport móddal** a rendszeresen edzőknek. Modern webes felület, interaktív grafikon és részletes növényi táplálkozási útmutató.

---

## ✨ Főbb Funkciók

1. **🎯 3-Irányú Célválasztó**
   - **Fogyás**: tempó a testsúly %-ában (0,25–1%/hét), becsült időtartam-tartománnyal.
   - **Súlytartás**: energiaegyensúly (TDEE).
   - **Izomépítés**: lassú súlygyarapodás (0,1–0,5%/hét).
   - A célkalória soha nem megy az alapanyagcsere (BMR) alá.

2. **🔬 BMR Számítás**
   - **Mifflin-St Jeor** (ajánlott, általános), **Katch-McArdle** (testzsír alapján), **Cunningham** (sport módban, izmos sportolóknak).
   - Nemenként eltérő testzsír-irányadók.

3. **📊 Makró Stratégiák**
   - **Ajánlott (automatikus)**: fehérje a cél, az életkor (65+) és a sport mód szerint.
   - Kiegyensúlyozott, Fehérjedúsabb, Teljes értékű növényi (WFPB), sport módban Sportolói presetek, illetve egyéni csúszkák.
   - 30 feletti BMI-nél a fehérje referencia-testsúlyra számolódik.
   - Zsír legalább 0,6 g/kg, szénhidrát-ellenőrzés (45–60%).
   - Rost: 14 g / 1000 kcal (25–50 g), folyadék: 30–35 ml/kg.

4. **🏋️ Sport Mód**
   - Hétköznapi aktivitás + külön megadott edzésenergia (nincs dupla számolás).
   - **Energiaelérhetőség (EA)** és RED-S figyelmeztetés.
   - Edzésnapi / pihenőnapi kalória és szénhidrát, ajánlott g/kg tartomány az edzés jellege szerint.
   - Edzés előtti / utáni étkezések makróihoz igazított elosztás, leucin-tipp.

5. **⚠️ Figyelmeztetések**
   - 18 év alatti életkor, alacsony (cél) BMI, 65 év feletti gyors fogyás, túl alacsony zsír vagy szénhidrát, BMR alá eső kalória.

6. **🔄 Vegán Fehérje Átváltó**
   - 11 növényi fehérjeforrás fehérjeminőségi megjegyzésekkel (pl. lizin- vagy metioninszegény), tetszőleges adagmérettel.

7. **🛡️ Vegán Mikrotápanyag Útmutató**
   - B12, D3, omega-3, vas + C-vitamin, kalcium, jód, cink, szelén, kreatin és éves laborvizsgálat.

8. **📱 Mobil UX & Adatmentés**
   - Lebegő összefoglaló sáv mobilon, automatikus LocalStorage mentés, nyomtatóbarát nézet.
   - **Telepíthető alkalmazás (PWA)**: saját ikon és név (Vegán Makró), teljes képernyős indítás iOS-en és Androidon.
   - **Telepítés gomb** a fejlécben (Chrome / Edge / Android), iOS Safariban pedig egy bezárható tipp-sáv mutatja a „Főképernyőhöz adás” lépéseit.
   - **Offline működés**: a Service Worker (`sw.js`) gyorsítótárazza az oldalt, az ikonokat és a CDN-könyvtárakat, így az első betöltés után internet nélkül is használható.

> Tájékoztató becslés, nem helyettesíti az orvosi vagy dietetikusi tanácsot.

---

## 🚀 Használat és Futtatás

Nincs szükség szerverre vagy telepítésre, a projekt egyetlen önálló weboldal:

1. Nyisd meg az `index.html` fájlt bármelyik modern böngészőben.
2. Vagy kapcsold be a **GitHub Pages** szolgáltatást a repóban.
3. Mobilon (GitHub Pages-ről megnyitva): Safariban **Megosztás → Főképernyőhöz adás**, Androidon Chrome-ban **Hozzáadás a kezdőképernyőhöz**.

> **Megjegyzés:** a Service Worker és a telepítés csak `https`-en (pl. GitHub Pages) vagy `localhost`-on működik, közvetlenül megnyitott fájlból nem. Az oldal a gyorsítótárból indul és a háttérben frissül, ezért egy új verzió általában a **második** megnyitáskor jelenik meg. Nagyobb változásnál érdemes az `sw.js`-ben a `CACHE_NAME` verzióját növelni.

---

## 🛠️ Felhasznált Technológiák

- **HTML5 & Vanilla JavaScript** (build eszközök nélkül, teljesen kliensoldali)
- **Tailwind CSS** (sötét mód támogatással)
- **Chart.js** (makrotápanyag fánkdiagram)
- **Lucide Icons** (vektoros ikonok)
- **PWA**: Web App Manifest (`manifest.webmanifest`) + Service Worker (`sw.js`)

---

## 📄 Licenc

MIT License &copy; 2026
