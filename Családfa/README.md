# Bevezető:

Ne feledd, hogy az sql-kódot nem "írni", hanem "bővítgetni" kell!

1. Először vedd azon táblákat, amiket használsz
2. Kapcsold össze őket, ha több van
3. Jelenítsd meg, SELECT *-gal!
4. mentsd el a működő sql-kódot VSCODE-kódban, és mostantól itt dolgozz, mert az Access-es sql-szerkesztő egy rémálom. A fájlt, amiben dolgozol, mentsd el sql kiterjesztéssel, és szépen színez majd mindent.
5. A működő kódot ne írd felül: CTRL+C, CTRL+V, és az újat bővítgesd. Látszódjon az adott feladat kódjának az evolúciója! Ez különösen fontos akkor, amikor rájössz, hogy valamit rosszul csináltál és vissza akarsz ugrani egy még működő változathoz.


# Családfa

## Adatok áttekintése
1. Hozd létre azon Szülő-Gyerek reláción alapuló táblát, ahol a szülők és gyerekek nem az id-jükkel, hanem rendesen a vezeték és keresztnevükkel szerepelnek (konkatenációval dolgozz!)
2. Hozz létre egy graphviz-ben értelmezhető outputot, ahol olyan sorok vannak, hogy 

[...]
"Virág Barnabás" -> "Virág Marcián";
"Kovács Jaina" -> "Virág Marcián";
"Pásztor Tege" -> "Pásztor Masa";
[...]

3. Ezt aztán nézd meg: https://dreampuf.github.io/GraphvizOnline/


## Elemi összesítések
1. Mely vezetéknevek szerepelnek az adatbázisban? Mindegyik csak egyszer szerepeljen!
2. Hány különböző vezetéknév szerepel az adatbázisban?
3. Mi a legelső és legutolsó vezetéknév a névsorban?
4. Hány férfi és hány nő van az adatbázisban?

## Elemi csoportosítások
1. Melyik vezetéknévnek van a legtöbb viselője?
0. Melyik szülőnek hány gyermeke van?
0. Hány gyermeke van a legtöbb gyermekkel bíró szülőnek?
0. Add meg, hogy hány 2-gyerekkel bíró szülő van!
0. Add meg, hogy hány 1-gyerekes, 2-gyerekes, stb. szülő van! (0 gyerekes szülő nincs!)
0. Hány olyan vezetéknév van, amelyet csak egyetlen ember hord?

## Projekciók:

1. Kik a szülők, azaz azok, akiknek van gyermekük? 
0. Hány szülő van?
0. Az U tábla segítségével szerepeltesd a szülők neveit és a választ rendezd vezetéknév szerint ábécésorrendbe!
0. Add meg azt a szülőt, aki a legelső a szülők névsorában!
0. Kik azok, akik gyermekei valakiknek? 
0. Hány gyermek van?
0. Az U tábla segítségével szerepeltesd a gyerekek neveit és a választ rendezd vezetéknév szerint ábécésorrendbe!
0. Add meg azt a gyermeket, aki a legutolsó a gyerekek névsorában!

## Definíciók:

### Lánya:
1. Add meg az "x lánya y" relációt!
2. Az U segítségével szerepeltesd az emberek neveit is az előbbi tábla alapján!

### Apja:
3. Add meg az "x apja y-nak" relációt!
4. Az U segítségével szerepeltesd az emberek neveit is az előbbi tábla alapján!

### Unoka:
5. Hozd létre az Nagyszülő-unoka relációt! (Kinek ki az unokája?)
6. Az U segítségével szerepeltesd a nagyszülők és unokák neveit is az előbbi tábla alapján!

### Házaspár:
7. Házaspárnak tekintjük azokat, akiknek van közös gyermekük. Add meg a Házaspár relációt!
8. Az U segítségével szerepeltesd a párok neveit az előbbi tábla alapján!

### Testvér:
9. Hozd létre az Testvér relációt! Ügyelj arra, hogy senki sem testvére önmagának!
10. Az U segítségével szerepeltesd a Testvérpárok neveit is az előbbi tábla alapján!

### Lánytestvér:
11. Hozd létre a Lánytestvér relációt!
12. Az U segítségével szerepeltesd a párok neveit is az előbbi tábla alapján!

### Fiús anyuka:
13. Hozd létre a "fiús anyuka" relációt! Azt mondjuk, hogy egy anya fiús anyuka, ha minden gyermeke fiú.
14. Az U segítségével szerepeltesd a párok neveit is az előbbi tábla alapján!

## Unokatestvér
15. Hozd létre az unokatestvér relációt! Ügyelj arra, hogy senki sem unokatestvére önmagának, sőt, a testvérek sem unokatestvérek!
16. Az U segítségével szerepeltesd a neveket is az előbbi tábla alapján!

## Negáció:
1. Kik nem gyermekei senkinek sem? (Kik a családfák gyökerei?)
2. Kiknek nincs szerepeltetve gyermeke?
3. Kiknek van úgy gyerekük, hogy nincs párjuk?

## Komplex:
1. Kik az egykék?
2. Mely nagyszülőnek van a legtöbb unokája? És hány unoka ez tulajdonképpen?
