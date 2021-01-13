---
Title: Kmom10
Description: Part 10
Template: kmom
---

![redovisning](%assets_url%/img/redovisning.png){.redovisning}

Kmom10 - Projektet -Redovisning
==================
<h2>Uppdrag 1: Webbplats</h2>
Jag har valt att arbeta med att skapa en webbsida för sing -songwritern Art Ist. Jag har valt att behålla grunden från min portfolio som jag har arbetat med under kursen. När jag skissade sidan för artisten blev utseendet väldigt likt det jag redan skapat så jag valde att behålla det jag gjort som grund, dels för att jag är nöjd med grunden jag skapat under kursen och även för att ha utrymme för att göra fler uppgifter under projektet och ha tid för att göra analyserna.

Webbplatsen består utav tre sidor, en förstasida med en stor hero-bild som har en logga som hem-knapp. Sidan har en about-sida och en highlight-sida som visar upp olika spelningar Art Ist har gjort i ett bildgalleri. Hero-bilden skapar intresse och är stor på första sidan, jag har valt att göra bilden mindre på undersidorna för att få bättre balans och mer fokus även på innehållet på dessa sidor. Webbplatsens navigeringsmeny blir en "hamburgarmeny" i det responsiva läget. Navigeringen på första sidan hamnar på sidans above the fold, vilket är viktigt för tillgängligheten.

Webbplatsen har en egen logga som används som hem-knapp. Favicon för sidan är svarta rosor. För att få en bild till iconen använder jag https://icoconvert.com/ för att transformera bilden till .ico och bilden skapades i Canva.

Footern innehåller länkar till sociala medier (icke fungerande länkar). Tanken är att artisten är aktiv i sociala medier och gärna vill hänvisa till sina sidor. Art Ist ville motto finns också med i footern, det döljs i det responsiva läget för mobil.

Jag har använt Cimage på samma sätt som vi gjorde i kursmomentet för bildgalleriet. Bilderna visas i tre olika storlekar beroende på skärmstorlek. Fortsatte sedan att anpassa resterande bilder på webbsidan. Headerbilden anpassades på samma sätt som galleriet. För aside bilderna använder jag picture elementet och srcset och lade in olika bilder som läses in för olika skärmstorlekar.

I about-sidan berättar jag om kunden och om hur intervjuprocessen skulle kunna se ut för att förstå kundens behov. Jag berättar sedan hur jag utifrån informationen tolkat hur kunden vill att webbplatsen ska användas, vilka önskemål som framkommit.

<h2>Uppdrag 2: Tema</h2>
Jag har skapat ett tema för webbplatsen som bygger på mitt tidigare tema. Temat är anpassat till Art Ist och för att möta upp Art Ist önskemål om en webbplats som är "fräsch, tidsenlig och skapar intresse" har jag tillämpat det vi lärt oss under kursen och valt att utgå från ett minimalistiskt tema med gråskala på bilderna, ett svart/vitt tema med mycket whitespace/negativ space och har valt att använda ett monokromt schema med rött för att skapa en intressant touch till sidan. Jag har valt att inte ha en kritvit bakgrundsfärg för att minska kontrasten mellan den svarta färgen och vita bakgrunden, för att göra det behagligare att använda webbsidan.  

Temat använder SASS och är uppdelat i moduler. Det jag märkte när jag delade upp headern och footern i enskilda SASS filer var att jag fick mycket mer ordning på stylingen av dessa och det var lättare att anpassa variabler för headern och footern när de låg i egna SASS-filer.

Jag hade byggt hela min sida med variabler även tidigare, så jag lade till nya variabler och ändra de andra så att det skulle passa kundens önskemål. Att använda variabler är ett smidigt sätt att få koll på färger och det blir lätt kunna redigera färgerna vid behov.

Jag har haft fokus på designelement och designprinciper när jag skapade sidan utifrån kundens behov. Jag har fokuserat på att hitta ett modernt uttryck som skapar intresse. I tidigare analyser har jag tagit med mig att just det minimalistiska uttrycket är populärt.

På about-sidan finns en länk till en sida som är dold från menyraden via metainformationen hidden: true. Den sidan innehåller dokumentation om sidans färgpalett, dokumentation gällande färgval, typografi, designelement och designprinciper. Jag har också beskrivit vilken känsla sidan vill förmedla samt hur jag har valt att dela upp SASS koden. I början av den dolda sidan beskriver jag också kort hur webbplatsens struktur och uppbyggnad ser ut utifrån information som framkommit under about-sidan. På den dolda sidan finns figmaskissen som skapats för första sidan samt print screen bilder på undersidorna.   

<h2>Uppdrag 3: Responsivitet och tillgänglighet</h2>

<h3>Responsivitet</h3>
Gallerisidan använder CSS-grid för att skapa bildgalleriet och för att göra sidan responsiv.
Resternade sidor använder flexbox för att presentera innehållet.
Det som hjälpte till mycket att skapa bra responsivitet för aside-elementet på sidorna var att använda olika storlekar på bilderna med hjälp av picture elemenetet.
Sidan fungerar bra responsivt. Jag hade problem med "hamburgarmeny" på mobilläget och fick hjälp i Discord att byta ut ID nav mot en omslutande div och istället använda class, det fungerade bra. Har också haft en utmaning att få loggan att bli responsiv, den lade sig i början så att den blockerade menyn i det responsiva läget.

<h3>Tillgänglighet</h3>
Samtliga sidor har 100% accessibility enligt verktyget Lighthouse. Jag hade velat haft lite mindre kontrast mellan färgerna i länken till den dolda sidan, den hade först en ljusare färg av röd, men då gick det inte att få 100% i Lighthouse, så här fick tillgängligheten gå först.
Jag har tittat på verktyget Toptal - Colorblind Web Page Filter efter att jag publicerat sidan. Tittar främst att menyraden syns tydligt och att det går att se vilken sida som används i menyvalet, det ser bra ut. Har även tittat på sidorna som helhet och på länkarna i footern. Sidan är tillgänglig även för personer som är färgblinda.

<h2>Uppdrag 4: Tema alternativt</h2>
Art Ist ville ha ett mer rockigt och alternativt alternativ till sin minimalistiska sida, där hon kunde sticka ut lite mer med sin personliga och rockiga stil. Sidan skapades därför om med ett kompletterande färgschema i grönt och rosa, headerbilden gjordes om för att bli mer rockig. För att kunna använda olika headerbilder löste jag det på samma sätt som vi växlar teman, genom en if-sats som talar om att det skall vara en bild om alternativt tema är valt och en annan bild om vanliga temat är valt. Typsnitt används istället för bild i det alternativa temat för att få en mer rockig stil såsom jag sett i aktuell webbplatsanalys i uppdrag 5 att man kunde göra. Även första sidans aside bild gjordes om för att skapa en mer färgrik känsla, bilderna växlas på samma sätt som headerbilden med en if-sats och picture-element. De övriga bilderna har jag behållit likadana men tagit bort filtret som i det originella temat förmörkar bilderna i en minimalistisk anda, i detta alternativa tema får istället bilderna ta plats med sina riktiga färger. Jag har behållit samma struktur på båda temana och ändrat färger, typsnitt och några bilder. I grunden har jag utifrån det vi lärt oss i kursen behållit så mycket som möjligt likt för att få en enhetlig och sammanhållen känsla av att webbplatsen hör ihop, även om temana skiljer sig åt.
<br>
Tillvägagångssätt att skapa det nya temat var att först skissa upp ett nytt tema. Jag hade grunden för det mörka temat från förra kursmomentet och ändrade det till alternativt tema genom att uppdatera variablerna och skapa fler SASS-filer med alternativ för typsnitt och imports. För att kunna använda temat gick jag igenom hur vi skapade mörkt team och gjorde ändringarna som behövdes för att aktivera det nya temat. Det var väldigt roligt att jobba med ett alternativt tema och jag kunde vara mer kreativ och skapa ett mer färgrikt tema. I det nya temat uppnår alla sidor 100% accessibility. Jag hade problem att få 100% på about-sidans länk till den dolda sidan. Jag försökte på alla sätt att ändra färg till olika rosa nyanser, till svart och även dessa färger med vit bakgrundsfärg men det fungerade inte. Det som slutligen fungerade var svart text på länken som jag ändrade till fet-stil. Nu skall alla sidor ha 100% tillgänglighet även för det alternativa temat.

<h2>Uppdrag 5: Analys aktuell webbplatsdesign</h2>
Jag har valt tre webbsidor för att undersöka aktuella trender inom webbplatsdesign, sidorna som har valts ut är kvinnliga artisterna Lady Gaga, Billie Eilish och Taylor Swift. Detta urvalet gjordes för att även kunna analysera min egen webbplats för projeketet med de sidorna i undersökningen för att se om sidan håller enligt aktuella trender eller om den behöver  uppdateras utifrån det som framkommit i undersökningen.  

Jag har valt att analysera utifrån design-principerna symmetri/asymmetri, att undersöka om sidorna använder grid. Inom dessa områden genomfördes korta analyser och konstaterande om sidorna använder detta eller ej. En mer ingående analys gjordes i undersökningen kring elementen typografi, bilder och färg. Har tittat på användning av herobild. Först gjordes en undersökning av varje sida separat och sedan jämfördes sidorna med varandra i analysdelen. Slutligen jämförde jag resultatet i analysdelen med min egen sida och kunde därmed konstatera att webbplatsdesigning för min projektsida håller sig till aktuell webbplatsdesign.

Det har varit intressant att jämföra webbsidor och undersöka designtrender. Jag gjorde det alternativa temat efter att denna undersökning gjordes vilket gjorde att jag fick inspiration och ideér till det alternativa temat.

<h2>Uppdrag 6: Analys valfri</h2>
Jag har valt att analysera min webbsida utifrån att titta på bilder och laddningstider. Detta val görs då jag inte har analyserat detta tidigare under projektet, färger är en designprincip som jag analyserat mycket och även designprinciper och designelement har tagits upp och diskuterats tidigare. Därav detta val, då det kan tillföra ny information.
Det först jag gjorde var att använda Google pagespeed och såg direkt när jag analyserade första sidan att bildformatet png drog ned värdet väldigt mycket, sidan hamnade på 83/100. Jag hade tänkt ha några bilder kvar i png då jag så gärna vill att det skall se bra ut med bilderna. När jag ändrade till jpg höjdes värdet till 94 vilket var en stor förbättring. Jag körde sedan sidan i Lighthouse och fick liknande resultat, förutom att mobilsidan för förstasidan hamnade lägre. Det fanns även andra saker som påverkade laddningstider förutom bilderna, dessa saker är inte något som jag hade möjlighet att ändra nu. Även Devtools verktyget och fliken nätverk användes för att se över laddningstider.
Över lag är jag nöjd med min webbsida inom detta projekt med hänsyn till laddningstider. Jag kollade igenom undersökningen vi gjorde i kmom05 gällande laddningstider och min sida hamnar i toppen om man jämför med deras sidor. Samtliga sidor som jag undersökte då fick anmärkning i Lighthouse att de hade behövt använda ett modernare bildformat. För mig höjdes värdet mycket genom att använda mig av ett annat bildformatet. Det var roligt att se att sidan fick så pass höga värden i jämförelse och jag tänker att de kunskaper som vi har fått under denna kursen har varit värdefulla och till stor hjälp för att nå höga resultat på de undersökta mätningarna.

<h2>Slutligen:</h2>

<h3>1.2 Allmänt om projektet.</h3>
Det har gått bra att genomföra projektet. Det var en hel del planerade och förberedelse innan det var dags att få ihop webbsidan, likadant för det alternativa temat där jag funderade mycket innan, skissade, fördjupade mig inom designprinciper och designelement, läste kursboken igen. Jag har haft problem med cashade bilder och att det upplevts som segt att arbeta med SASS-filer. För det mesta har det gått bra, men ibland läste Cimage inte in någon fil och ibland var det svårt att se ändringarna jag gjorde då webbläsarna hade cashe och inte laddade om trots att jag använde "Ctrl+R". Jag löste det genom att ha 3 olika webbläsare att växla mellan.
Undersökningen  i uppdrag 6, gjorde jag innan det alternativa temat, för att få idéer och inspiration till det nya temat. Det var roligt att se vilka trender som fanns och sedan kunna använda informationen för att designa ett nytt tema.
Jag hade till en början lite svårt att få picture elementet att fungera, men jag har googlat och fördjupat mig och sedan gick det bra. Hade lite problem att få menyraden i "ipad" responsiva läget att fungera då menyraden splittrades och inte hamnade bredvid varandra. Jag googlade och hittade att "display: inline-block" skulle ligga under nav li-elementet, jag hade det bara på ul-elementet och då löste det sig. Det börjar bli enklare att hitta lösningar när jag stöter på problem, jag vet mer hur jag ska söka efter information och då finns det hur mycket kunskap som helst och är inte alls svårt att hitta lösningar. Det som varit enkelt har varit själva designandet, det är väldigt roligt att vara kreativ och skapa teman och alternativa teman. Jag tycker också att det var bra att det fanns fördjupningsuppgifter med analyser, det är utvecklande och lärorikt och det upplevs som att analyserna följer med som en röd tråd genom kursen vilket uppskattas.
Projektet har tagit ungefär så lång tid som var avsatt för kursmomentet och det är ett rimligt projekt för kursen.

<h3>1.3 Tankar om kursen.</h3>
Jag tycker att kursen har varit mycket lärorik, utvecklande och givande. Jag har lärt mig om designprinciper och designelement och materialet har varit välgjort och enkelt att följa. Jag har lärt mig om att design inte alltid behöver anpassas för att passa alla utan att den kan anpassas utifrån målgrupp och önskemål hos kunden, att det ibland är bättre att anpassa till en smalare skala för att göra ett intryck och sticka ut. Det har varit lite krångligt att få flödet att fungera för mig med cashade bilder o.s.v. och det har allmännt känts mer trögt att jobba via SASS-filerna. Men på ett sätt är det enklare med Markdown-koden, så att man har kunnat fokusera på designen. Jag har tyckt mycket om analyserna, det har varit givande och lärorikt. Har kunnat ta med mig det jag har lärt mig från att analysera andras webbsidor när jag skulle påbörja projektet. Mycket bra upplägg på kursen, bra feedback vid inlämningar och snabba rättningar på uppgifterna, även snabb och  bra hjälp om man behöver i Discord. Tack för en bra kurs.
Jag skulle helt klart kunna rekommendera den här kursen till min omgivning. Kursen får en 10:a av mig.
