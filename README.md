# Pontvadász ZH 

## Cherry Picking 

Az adatbázis a Chat-GPT segítségével lett generálva.

## Árlap 

A pontszámok szorzat formájában kerültek megadásra, pl: `4x1p`. A **második** szám -- a példában `1p` -- azt jelenti, hogy hogy hány pontot ér az adott részfeladat, az **első** pedig az adja meg, hogy hány ismétlés kerül beszámításra. Így nem lehet egyetlen részfeladat ismételgetésével teljesíteni a ZH-t. 

### Windows Forms Application

##### User Interface 

- `1x2p` Az alkalmazásból a **kilépés csak megerősítő kérdés után** lehetséges. 
- `3x2p` Olyan alkalmazás **elrendezés, melyben gombok lenyomására UserControl-ok kerülnek elhelyezésre egy Panel vezérlőben**, teljesen kitöltve azt. Minden gombra jár a pont, amennyiben az funckuonlalitással rendelkező UserControl-t tölt be. 

- `2x1p` **Többablakos alkalmazás** legalább két felugró ablakkal. Minden Form-nak saját osztályon kell alapulnia, és funcionalitással kell rendelkeznie. Az ablakok nyílhatnak gombokkal vagy felső menüből is.

##### Tábla adatainak megjelenítése `ListBox`-ban. 

- `1x2p` Adatok  megjelenítése 
- `2x2p` Ha az adatok tetszőleges módszerrel, pl. `TextBox`-on keresztül szűrhetőek.

##### Tábla adatainak megjelenítése `DataGridView`-ban 

- `1x2p` Adatok  megjelenítése
- `1x2p` Ha a tábla adatforrása saját osztály. 

##### Adatkötés `BindingSource` -on keresztül

- `1x2p` Működő  `BindingSource` 

##### Új rekord rögzítése 

A pontok összeadódnak. 

- `1x2p` master-detail reláció detail táblájába ÉS/VAGY több-a-több kapcsolatban álló táblák kapcsolótáblájába
- `1x2p` Ha csak az idegen kulcsok vannak felvéve
- `1x1p` Ha legalább egy nem kulcs mező, pl. _Mennyiség_ is fel van véve
- `1x2p` Ellenőrzéshez kötött adatfelvitel (egyszerű validáció pl: `String.IsNullOrEmpty()`)
- `1x2p` Felugró ablakon keresztül történik _Ok_ és _Mégse_ gombbal

#####  Rekord törlése 

- `1x2p` Sikeres törlés
- `1x2p` Megerősítéshez kötött törlés

##### Diagram rajzolása, Excel munkafüzet generálása

- `1x7p` Excel munkafüzet generálása kódból, adatbázstába tartalmának megjelenítésével, legalább egy formázással

### ASP .NET 

- `1x2p`  `program.cs` beállítása `wwwroot` mappában tárolt statikus tartalmak megosztására

##### API végpontok

- `1x3p` Teljes SQL tábla adatainak szolgáltatása API végponton keresztül 
- `2x2p` SQL tábla egy választható rekordjának szolgáltatása API végponton keresztül
- `1x3p` SQL tábla egy választható rekordjának törlése
- `1x5p` Új rekord felvétele `HttpPost` metóduson keresztül SQL táblába
- `1x3p` Rekord módosítása `HttpPost` metóduson keresztül SQL táblában 

##### Javascript

- `1x5p` (pl: szöveg és kép) DOM feltöltése javascripttel (vizsgán írandó, NEM HOZOTT, aki ezt választja az a hozott anyagba nem rakhatja bele a js kódot amivel feltölti a tartalommal a DOM-ot, tehát ez az előre feltöltött `hozott.js`-ben nem lehet benne, vizsgán kell megírni egy `vizsga.js` fájlba.) 

### Hozott anyagok

Hozott CSS.

##### Saját Adatbázis

Azure SQL szerveren hosztolva.

- `3x1p` Az alkalmazásban használt táblánként pont
- `1x1p` Az adatbázis tartalmaz Constraint-eket (min 2)
- `1x1p` Az adatbázis adatainak forrásmegjelölése értsd: miből készült és hogyan
- `1x2p` Az adatbázis saját Azure SQL szerveren van

##### Weboldal

Itt csak azok az elemek számíthatóak be, amelyeknek meg van a ZH alatt felépített API végpontja. 

- `1x1p` A weboldalnak van egy értelmezhető struktúrája
- `1x1p` A weboldal dinamikus tartalommal tölthető fel adatbázison keresztül
- `1x1p` A weboldal használ legalább 20 sor értelmes css-t

### Egyéb, extra

- `2x1p`  `Scaffold-DbContext` használata (ajándék)

##### Bonyolultabb algoritmus használata értelmes feladatra

  

##### Identity Framework alkalmazása hitelesítéshez ínyenceknek
