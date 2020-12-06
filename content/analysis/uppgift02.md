---
Title: Laddningstider
Description: Part 2
Template: kmom_analysis
---

Laddningstider
=======================

I den här rapporten ska vi välja ut tre olika webbplatser och sedan testa dem genom att mäta hur laddningstider och analysera om sidorna innehåller något som skulle kunna förbättras med hänsyn till laddningstid och användbarhet. 

Urval
-----------------------

Jag kommer att fortsätta med mina webbsidor från föregående rapport viket är Friskis & Svettis, Elite och YogoBe. 

Yogobe: <a class="links"> https://yogobe.com/se </a> <br>
Elite: <a class="links"> https://elitsportsclub.se </a> <br>
Friskis & Svettis: <a class="links"> https://www.friskissvettis.se </a><br>

Metod
-----------------------
Första tas en snapshot på webbplatserna som valts ut i urvalet. 
I den här rapporten kommer jag använda mig av Google Pagespeed som gör en mätning på webbsidan och även använda Devtools fliken Networks för att kontrollera laddningstiderna för webbsidorna. Jag har använt Google Chromes devtool verktyget Lighthouse och gjort mätningar som jämför mobilläget för första sidan med desktop-läget för en undersida. 
Jag använder LibreOfficeCalc för att föra in resultaten. 

Resultat
-----------------------

<h3>Elit:</h3>
<br>
![elite](%assets_url%/img/elite.png){.schema}
<br>

PageSpeed:
Enligt Pagespeed hamnar Elit på 33/100 poäng och klarar enligt mätningen inte granskningen. Webbsidan använder blandade bildformat png och jpg och skulle enligt mätningen kunna 
spara 2.85s i laddningstid genom att skicka bilder i modernare bildformat. Det skulle gå att spara 1.98s genom att förhindra att resurser blockerar sidans första rendering. Det står
att det skulle vara möjligt att infoga nödvändig JS-/CSS-kod direkt på sidan och att det skulle vara möjligt att senarelägga inläsningen av JS-kod/formatmallar som är mindre viktiga för att öka hastigheten. Ytterligare 1s skulle kunna sparas genom att ta bort Javascript som inte används.

Lighthouse: 
Det högsta värdet i Lighthouse får webbsidan Elits mobilversion på SEO vilket indikerar hur hemsidan hamnar i ranking på sökmotorer. Det som gör att sidan inte hamnar på ett toppvärde är att bilderna på sidan saknar alt-attribut och att en länk inte har en beskrivande text. Accessibility, tillgänglighet, hamnar på 53% och det som står högst upp är att färgerna på hemsidan inte har tillräckligt med kontrast för att vara lätt tillgängliga för alla, det står också om bilder utan alt-attribut och länk utan beskrivning som också minskar tillgängligheten. Performance värdet hamnar på 46% och överst står att sidan skulle kunna spara hela 3.75s på att ta bort JavaScript som ej används i övrigt samma som framkom under Pagespeeds rapport. Best practices värdet är 79% och hamnar på detta värde p.g.a. att en länk är osäker och sidan använder JavaScript som har kända säkerhetsrisker.

Har jämfört med en Lighthousemätning på en undersida och i desktop-läge vilket ger ett högre Performance värde på 90%, ett Accessibility och Best practices värdena är kvar på samma värde som ovan och ett SEO värde som är mycket förbättrat i denna mätning på 91%, det enda som är anmärkt på är att bilder inte har alt-attribut. För ett högre Performence värde hade sidan behövt ha bättre storlek på bilderna. 

Devtools: 
Requests: 46st
Transferred: 1.4MB
Resources: 2.3MB
Finish: 2.2s

<h3>Yogobe:</h3>
<br>
![yogobe](%assets_url%/img/yogobe.png){.schema}
<br>

PageSpeed:
Webbsidan Yogobe klarar inte granskningen enligt PageSpeed mätningen, den hamnar på ett värde på 21/100 möjliga. Det som hamnar överst i förbättringsområden för sidan är att den skulle kunna förhindra resurser som blockerar sidans första rendering, det skulle kunna spara 2.83s. Vidare framkommer att sidan skulle kunna spara ytterligare 2.43s genom att ta bort JavaScript som ej används. Att använda ett mordernare bildformat skulle kunna spara ytterligare 2s. 

Lighthouse: 
Lighthouse mätrningen för mobilläget visar ett värde på 33 i Performance som hänvisar till samma effektiviseringsområden som PageSpeed gjorde i ovanstående mätning. Tillgänglighetsvärdet, Accessibility, hamnar på 52% och det framkommer att det är låg kontrast på texten som inte är tillgänlig för alla, det saknas titel på frame-element, bilder saknar alt-attribut och länkar har inte namngivits. Värdet dras även ner av att html-elementet inte har ett lang-attribut. Best Practices värdet hamnar på 79% och hamnar ej i topp p.g.a. att länkar till andra sidor ej är säkra samt att det finns 6 st kända säkerhetsrisker med JavaScript på sidan. Rankingvärdet för sökmotorer, SEO, hamnar på 79% och hamnar ej i topp p.g.a att bildelement inte har alt-attribut och att 3 st länkar ej har en beskrivande text.

Jag har jämfört med en undersida på Yogobe i desktop läge och sidan hamar då på lite högre värdenPerformance 38, Accessibility 79, Best Practices 79, SEO 82. Det som framkommer är att det handlar om lite lägre möjligheter att spara laddninstid, men inom samma områden som mobilsidan. Tillgängligheten är egentligen ingen skillnad förutom tillägg att knapparna inte har tillgängliga namn. På Best practices står det det finns browsers errors var loggade. SEO värdet hamnar lägre p.g.a. att dokument ej har meta descriptions.


Devtools: 
Requests: 114st
Transferred: 4.5MB
Resources: 6.6MB
Finish: 4.37s

<h3>Friskis&Svettis:</h3> 
<br>
![friskisochsvettis](%assets_url%/img/friskisochsvettis.png){.schema}
<br>
PageSpeed:
Enligt PageSpeed hamnar Friskis & Svettis hemsida på 26/100 poäng och klarar enligt mätningen inte granskningen. Enligt mätningen skulle webbsidan kunna spara tid på att skicka 
bilderna i modernare bildformat, det skulle kunna spara 18.89 s. Det framkommer också att det skulle vara möjligt att koda bilderna mer effektivt, optimerade bilder skulle kunna besprara halva utrymmet av bildstorleken enligt mätningen. Det skulle också vara möjligt att spara laddningstid genom att ta bort JavaScript som inte används (2.85 s) och oanvänds css (0.9 s). 

Lighthouse:
Tittar man på google Chromes lighthouse instrument och granskar mobilläget hamnar sidan bra till gällande Best practices på 93%, vilket indikerar att hemsidans Javascript ligger bra till gällande säkerhetsrisker. Det första performance hamnar på 18% och indikerar på att sidan skulle kunna spara hastighet på det viset jag tidigare beskrev genom ex. rätt bildstorlek. Accessibility, tillgänglighet, hamnar på 77%. SEO mätvärdet kontrollerar om webbsidan är optimerad i sökmotorers sökningsrankning och där får Friskis & Svettis 86% och hamnar ej på ett topp värde p.g.a. att bilder saknar alt-attribut och 1 länk saknar beskrivande text. 

Har även jämfört med en undersida på Friskis & Svettis och granskat desktop-läget. Här hamnar webbsidan mycket bättre i granskningen, 69% Performence, 95% Accessibility, 93 Best Practices och 92% SEO-värde. Det som fortfarande drar ner värdet på Performance är bildstorlek och oanvänd JavaScript. SEO-värdet hamnaer ej i topp p.g.a. en länk som ej har en beskrivande text och tillgängligheten hamnar ej på 100% p.g.a. kontrastfärgerna på sidan som ej är tillräckligt tydliga och därför ej tillgänliga för alla och p.g.a. frame element som ej har en titel. 

Devtools: 
Requests: 66st
Transferred: 84kB
Resources: 9.8MB
Finish: 4.49s


Analys
-----------------------
![diagram](%assets_url%/img/diagram.jpg){.schema}

Denna bild visar jämförelsen från Lighthouse mätningarna som gjordes enligt mobilversionen och enligt desktopversionen. Friskis & Svettis webbsida var den som hade störst skillnad på dessa två mätningar och enligt desktop versionen hamnar Friskis & Svettis på en 1:a plats, Elit hamnar på en 2:a plats och YogoBe hamnar 3:a. 

Det var ingen av sidorna som jag har undersökt som klarade granskningarna enligt mätningarna med PageSpeed. En analys är att webbsidorna fokuserar mer på innehåll änn på laddningstider och använder ofta stora bilder med omoderna eller icke effektiva bildformat med hänsyn till laddningstider. 

Elit hamnar på plats 1 enligt PageSpeed mätningarna, Friskis och Svettis på plats 2 och YogoBe på plats 3. Det stämmer väl med upplevelsen av att besöka webbsidorna. Yogobe innehåller filmbibliotek och tar lång tid att ladda. Friskis & Svettis webbsida tar också lång tid att ladda.

Tittar vi på devtools mätningarna är Elit den sidan som har kortast laddningstid med 2.2s och både Friskis & Svettis och Yogobe hamnar över 4s.

Upplevelsen av att besöka webbsidorna är att Elits sida är smidare att besöka, den laddar snabbare och när jag väger in båda mätningarna ovanför med upplevelsen av att besöka webbsidorna hamnar Elite på en första plats. Friskis & Svettis hamnar som helhet på en 2:a plats i den här undersökningen som helhet och Yogobe på plats 3. Det är förståligt att en sida som Yogobe som har bibliotek med träningsfilmer tar längre tid att ladda. 

De vanligaste förbättringsområdena för Accessibility var att det var låg kontrast på texten som inte är tillgänlig för alla, på samtliga sidor saknade bilderna alt-attribut  vilket drog ner värdet och sidorna hade länkar har inte namngivits. En annan analys är att alla webbsidor fick anmärkning på att de hade kunnat förbättra Performance genom att spara nedladdningstid genom att använda ett annat bildformat eller en annan bildstorlek.

Jag skulle uppskatta att 2-3 s är högsta nivå för laddningstider, har lite kortare tålamod om jag surfar på mobilen än om jag skall besöka t.ex. Yogobe och ladda en träningsfilm. Jag skulle säga att Yogobe:s webbsida ändå är värd att vänta på att den laddar medan Friskis & Svettis hemsida oftare känns som att den tar för lång tid att ladda. Elit känns smidig att besöka och jag upplever inte att den laddar långsamt. 

Referenser
-----------------------

PageSpeed Insights: developers.google.com/speed/pagespeed/insights/
<br>
Länk till Excel-arket finns i kommentarsfältet för inlämningen. 


Övrigt
-----------------------

Individuellt arbete skrivet av Josefine Bertvig




