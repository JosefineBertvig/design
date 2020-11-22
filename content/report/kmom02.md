---
Title: Kmom02
Description: Part 2
Template: kmom
---

![redovisning](%assets_url%/img/redovisning.png){.redovisning}

Kmom2
==================

<h3>Vad tycker du om SASS än så länge?</h3>

Det känns roligt och användbart att arbeta med SASS. Det är bra med möjligheten att använda variabler och det förenklar att kunna använda nästlade regler. 
Jag tycker om möjligheten att använda variabler för att underlätta att skapa ett färgtema. Jag gick in på canvas.com där jag skapat loggan och en av bilderna, där kunde jag hämta ut färgkoden och se färgteman utifrån de färgerna skapade jag sedan variablerna för färger som hemsidan bygger på. Det var ett roligt sätt att jobba på för att få balans och en känsla av att sidan hör ihop. 
<br><br>
Jag tycker att SASS erbjuder många bra möjligheter. Jag vill fortsätta utforska mer och är intresserad av att lära mig om mixins, det kommer att underlätta för att inte behöva återupprepa sig i koden när jag vill använda samma struktur flera gånger.
<br><br>
<h3>Är du bekant med Node, npm eller npm scripts (t.ex. npm run lint) sedan tidigare? Vad anser du om det?</h3>

Är inte bekant sedan tidigare. Bra att ha möjlighet att använda npn run lint för att rätta. Jag har använt kommandot npm run watch som gör automatiska ändringar vilket var väldigt hjälpsamt. 
<br><br>
<h3>Hur kändes det att kompilera SASS till CSS, var det något du reflekterade över?</h3>

Det blev väldigt mycket text i CSS filen från fonterna som vi importerade. Det gick bra att skriva scss filerna, några är kvar i det gamla formatet som importeras i style.scss. Till nästa redovisning ska jag göra om till en minifierad version. 
<br><br>
<h3>Kommentera ditt tema, hur kan man beskriva dess design och hade du några planer på “design” när du byggde ditt tema?</h3>

Jag har valt att använda ett färglatt tema då jag tänkt att innehållet skall i stil med rubriken " Happyness is a habit", därför har jag valt att använda detta tema.
Jag har utgått från block med en aside för att få två bilder, har sett att vi kommer jobba med grid i nästa moment och ser fram emot att utveckla sidan mer med hjälp av det. Har läst om version of the golden ratio som är regeln om tredjedelar och tänker att jag vill utveckla sidan mer åt det hållet med hjälp av grid så att den får rätt proportioner. 
Navigationen är under headern och är enkel att se, det är enkelt för besökaren att veta vilken aktuell sida man besöker då den är markerad i menyraden. 
Jag har gjort en logga som är i headern på sidan. Flashbilden finns med på alla sidor. Så header med loggan och flashbilden ska rama in hemsidan och skapa en enhetlig känsla medan tanken är att innehållet på undersidorna kan se lite olika ut. På redovisningssidan har jag skapat en bild med temat för redovisning. I asiden finns en bild som symboliserar hemsidans tema, tänker att jag kan använda den på endans första sidan och sedan utveckla de andra sidorna mer med eget innehåll.
I footern lade jag de 3 bilderna för hemsidan som fick vara symboler för de 3 länkarna jag valde att ha med. Footern är enkel med lite innehåll änn så länge. 
Jag har en tanke om att använda whitespace på sida då det är lika viktigt som att fylla sidan med innehåll då det skapar balans och lyfter det man vill visa på sidan.   
<br><br>
Typografin som jag har valt är en font för rubriken och en för undertexten. Jag ville göra typsnittet för rubriken lite mer speciell och valde därför en kursiv stil Fondamento och en fall back stil som är cursive. För texten ville jag ha ett enkelt och snyggt typsnitt, så därför valde jag Open Sans med en fall back som är sans-serif. Hemsidan får därmed en kontrast mellan rubriker och vanlig text vilket skapar en intressant känsla på sidan. Jag har gjort variabler för text storlek, radavstånd och för magic-number som räknar ut avståndet för margin-bottom genom att gånga text storleken med radavståndet. 
<br><br>
<h3>Valde du att dela upp din kod? Vilka uppdelningar valde du att göra?</h3>

Jag har delat upp koden för att skapa SASS-filerna. Jag har en style.scss som importerar de andra och är min basfile för SASS. Den importerar variablerna som har en egen fil, typografin som har en egen fil och de gamla css filerna som jag inte har hunnit transformera till scss ännu. 
<br><br>
<h3>Vilken är din TIL för detta kmom?</h3>

Jag har jobbat parallellt med en process gällande problemlösning och resiliens, förmågan att hantera motgångar, den här veckan. Har gått från frustration i kmom01 till att tycka att det är problemlösningen som är det roliga och utmanande och glädjen är stor när saker fungerar som jag har fått fundera på ett tag och sedan kunnat lösa. Jag har haft dialog med en systemutvecklare som berättar att det är själva problemlösningen som är glädjen för honom i sitt yrke och inte bara att nå fram till resultatet. Jag har varit väldigt resultatinriktad och velat haft lösningen snabbt, förstår nu att det viktiga är att prova på olika sätt och att lära mig hur saker fungerar. När/om jag kommer ut på en arbetsplats kommer det inte finnas lika bra guider och mallar, jag kommer få installera SASS och olika paket själv, så det viktiga är att förstå hur man gör och hur jag ska kunna söka information de gånger jag fastnar och inte vet hur man gör och hur de olika delarna hör ihop. Så mitt TIL för detta Kmom är lärandeprocessen och problemlösningen och att byta ut frustrationen mot nyfikenhet och lusten att utforska och lära mig mer! 

