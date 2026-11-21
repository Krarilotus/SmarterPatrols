# Smarter Patrols

**Szerző**: Monsterfish
**Verzió**: 1.0.1

Gondoskodik róla, hogy az MI járőr- és ostromvédelmi csapatai támadás közben valóban az összes csoportjukat használják. Mindkét rész külön kikapcsolható a beállításokban.

## Járőrcsapatok

Az alapjátékban csak az első járőrcsoport kap parancsot. A második az egész támadás alatt csak a gyülekezési ponton áll.

Ezzel a modullal minden járőrcsoport saját útvonalat kap a megtámadott vár körül:

- **1. csoport**: egyik irányban kerüli meg a várat.
- **2. csoport**: a másik irányban kerüli meg.
- **3. csoport**: a vár elülső oldala (a támadó felé néző oldal) mentén jár oda-vissza.
- **4., 5., 6. csoport**: ugyanazt teszik, mint az 1., 2. és 3., egy negyed körrel mögöttük. A 7., 8., 9. csoport azokat követi, és így tovább.

Meghatározott gyaloglási távolságra haladnak a váron kívül (alapértelmezés szerint 12 mezőre, mint az alapjáték járőre), így kikerülik a falakat és várárkokat ahelyett, hogy beléjük sétálnának. Ha egy csoport ellenségbe ütközik, előbb harcol, majd továbbhalad.

## Ostromvédelmi csapatok

Ezek a csapatok már eddig is ostromgépről ostromgépre jártak, de mindkét csoport egyszerre ugyanazon az útvonalon haladt, így egyetlen csoportként viselkedtek.

Ezzel a modullal:

- Minden csoport másik ostromgépnél indul, és minden második csoport ellenkező irányban halad, így lefedik az összes ostromgépet.
- A főként közelharci egységekből álló csoportok néhány mezővel az ostromgépek előtt (a vár felé) haladnak, hogy a védők őket lőjék a gépek helyett. Az íjászok a gépeknél maradnak.
- Amikor megindul a falak elleni roham, minden csoport támad, akárcsak az alapjátékban.

## Több csoport

Az alapjáték legfeljebb 2 járőrcsoportot és 2 ostromvédelmi csoportot tud kezelni. Ha egy MI-fájl többet kér, a többletegységek rossz csapatokba kerülnek (árokásókhoz vagy a főseregbe). Ez a modul mindkettőből akár 12-t is támogat. A szám az MI saját fájljából származik, ha a beállításokban nem adsz meg más értéket (ostromvédelemnél alapértelmezett: 4). A csapat csak addig oszlik tovább, amíg minden csoportba legalább 4 egység jut (ez módosítható).

A többletcsoportok csak a támadás idején léteznek. Amint rést ütnek a falon, meghal a lord vagy az MI visszavonul, újra csatlakoznak a többiekhez és követik az MI megszokott parancsait.

## Jó tudni

- Csak az MI támadásait érinti; a saját csapataid változatlanok maradnak.
- Működik a Lord Hunt modullal együtt.
- A mentésekbe nem ír semmilyen többletadatot.
