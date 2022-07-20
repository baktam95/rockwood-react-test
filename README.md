# Project setup

Az alkalmazásotok backend prototípusát a [json server](https://www.npmjs.com/package/json-server) fogja kiszolgálni.
Fontos: globalba kell telepíteni, hogy használni tudjátok. Ehhez segítséget és a sémákat az npm-es dokumentációban találjátok a fenti linken.


## Scriptek

### `npm install`
- Feltelpíti a modul dependencyket (ezzel kezdjétek klónozás/download után)
### `npm start`
- Futtatja a devszervert és az appot
### `npm test`
- futtatja a teszteket
### `npm run build`
- elkészíti a minified prod buildet

## MVP

A feladatotok egy user tracking webalkalmazás elkészítése, ehhez meghatározok egy minimum feature/requirement setet amit tartalmaznia kell:
1. Az alkalmazás development módban futtatható (`npm start`), compile és runtime error nélkül
2. A userdata a `db.json`-ből van kiolvasva, megfelelő api layer készítésével
3. A userek tile VAGY card megjelenítésben vannak listázva, oldalanként 5 darab, paginggel
4. A userek kezelésére, módosítására rendelkezésre állnak **CRUD** műveletek
5. Az app általános best practiseknek és konvencióknak megfelelő komponensek implementációja (KISS, DRY, Single responsibility)
6. A projekt mappaszerkezete jól átlátható, megfelel az általános guideline-oknak (mappánként max 5 file, típus/logikai felosztás)
7. Minimum UX: a műveletek sikerességéről popup/toast jelez vissza, async calloknál van spinner, törlés előtt van confirmation dialog
8. SPA approach, az oldal sososem tölt újra csak browser refreshnél.
9. Nincs leftover console.log
10. Az alkalmazás életképes mobil nézetben

## Extrák

1. Typescript használata típusokra, interfészekre
2. React-redux használata
3. SCSS preprocesszor használata
4. Styled komponensek
5. Unit tesztek írása, fő featuresetek lefedése, 80% körüli line coverage
6. Animációk (css-ből is elég lehet)
7. Linter, pre-commit hookba bekötve (husky)
8. Nincsenek trailing spacek
9. Mobile first approach
10. ES6 ahol csak lehetséges és nem szükségtelen.

## Kommentek

- A db.json file-t betettem gitignore-ba, így minden refreshnél vissza fog állni a tartalma, attól függetlenül hogy mit módosítottatok az apin keresztül rajta. (És nem piszkálni ám közvetlen a file-t, direkt van úgy ahogy 😉)
- Az arculat legyen légyszi 2022-es szintű, nyugodtan lehet lopni hasonló célú webappoktól ötleteket
- Törekedjetek légyszi a minőségre, a cél nem az MVP pontok kipipálása meg a featureset összehányása "csak működjön" alapon, hanem egy olyan app létrehozása ami a szakmai képességeiteket reprezentálja és később akár referenciának is használható a karrieretekben.
- A munkátokat **saját** gitlab/github/bitbucket repóba töltsétek fel, a commit historyt igyekezzetek tisztán tartani, **lehet**, hogy bele fogok nézni egy-egy commit változásaiba.
- A deadline végén ti fogjátok demózni az appot ha elkészültem a review-val.