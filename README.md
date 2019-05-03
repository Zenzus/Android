# Android

2019-04-08:
exsempel på stiden til en lydbog:
https://librivox.org/robinson-crusoe-by-daniel-defoe/
librivox api:
https://librivox.org/api/info

Beskrivelse: 
Vi vil lave en lydafspildningsapp der egner sig godt til lydbøger.
1. prioritet
Den skal kunne læse lydfiler i apparatets hukommelse.
Vi kan se dem på skærmen og tillade afspildning.
Brugeren skal kunne se progress bar, start/pause knap osv. 
Vores app skal skille sig ud ved at have god håndtering af spoling for store lydfiler
(hvor det er svært at spole via. progressbaren)

2. prioritet:
Appen skal kunne lave og gemme bogmærker, som gemmes i appens hukommelse, dvs. hver lydfil har sin egen liste af bogmærker

3. prioritet:
"Sleep mode": appen vil stoppe af sig selv efter et aftalt stykke tid,
så brugeren kan lægge sig til at sove uden at hele bogen afspilles.

4. prioritet:
avanceret sleepmode hvor brugeren kan se hvornår appen sidst bevægede sig (der hvor man tabte telefonen fordi man faldt i søvn)

5. prioritet:
man kan downloaded lydfiler til sin app fra nette. f.eks. fra librivox.com (public domain bøger)




2019-04-08:
Christian: forsøger at lave 003 og 004.
Jonas: kigger på hvordan man laver en afspiller.

Userstories:

001: finde filer på telefonen: 
Antagelse: vi har downloaded en fil og overført den til en mappe på telefonen.
Beskrivelse: når tester på telefonen, kan vi finde filnavnet (givet placeringen som vi kender)
og kan afspille filen.
Acceptance: ovenstående.


002: afspiller metode:
beskrivelse: vi laver en metode/klasse der afspiller en lydfil givet filnavn og filplacering.
den må gerne bruge en preinstalleret android afspiller.

003: fil oversigt layout:
Når man går ind i appen, får man en kanp. Når man trygger på den, 
får man en liste over alle lydfiler. 
Ved at trygge på et list-item, skal man kunne "vælge" den.

004: "gemme state":
når man går ind i appem igen, skal appen huske hvilken fil man arbejde med og
hvor langt man var nået.

005: afspildning af valgt fil.
forudsætning: 004 og 002 er løst.
Beskrivelse: når man har valgt en lydfil, kan vores afspildningsmetode afspille den.
Vores app skal være stylet sådan at appen ikke går i vejen for telefonens præ-installerede
afspiller.

006: udvidelse af telefonens almindelige afspiller:
Liste af features (betragt hver af dem som en usrstory):
A: 5 sec frem, 5 tilbage
B: 1 min frem, 1 min tilbage
C: 5 min frem, 5 tilbage.
D: "bookmark" (skal kunne gemmes efter man har forladt lydfilen)
E: "buffer knap": stopper automatisk appen efter en time, og laver automatisk et bookmark. (se også 004)


007: knap med liste og beskrivelser over bookmarks

