---
Title: Bilder och laddningstider
Description: Analys av bilder och laddningstider
Template: kmom_analysis
---

Bilder och laddningstider
=======================

I den här undersökningen har Organisationen Valfrihet gett uppdraget att göra en analys inom design och webbplatser, sidan som skall analyseras är den aktuella sidan som skapats för Art Ist under projektet.
Analysen kommer att göras utifrån samma undersökning som genomfördes i kursmoment 5, bilder och laddningstider.

Urval
-----------------------
Jag har valt att analysera min webbsida utifrån att titta på bilder och laddingstider. Detta val görs då jag inte har analyserat detta tidigare under projektet, färger är en designprincip som jag analyserat mycket och även designprinciper och designelement har tagits upp och diskuterats tidigare. Därav detta val, då det kan tillföra ny information.

Metod
-----------------------
I den här undersökningen kommer jag använda Google Pagespeed som gör en mätning på webbsidan och även använda Devtools fliken Networks för att kontrollera laddningstiderna för webbsidorna. Jag har använt Google Chromes devtool verktyget Lighthouse och gjort mätningar som jämför mobilläget och desktop-läget.

Resultat
-----------------------
<h2>Google Pagespeed</h2>
Först undersöks webbplatsen utifrån Google Pagespeed.
I mätningen framkommer föjande resultat:<br>
-Första sidan får resultatet 93 för mobilsidan och 94 för desktop<br>
-Aboutsidan 93 för mobil och 99 för desktop<br>
-Doldsida 91 för mobil och 93 för desktop<br>
-Gallerisidan 95 för mobil och 91 för desktop<br>

Gör först en mätning av första sidan som hamnar på 84 p.g.a. att bildformatet png används på några bilder, ändrar bildformatet och får då högre resultat.

<h2>Lighthouse Performance:</h2>
Gör sedan en mätning på Lighthouse och tittar på resultat i Performance.
I mätningen framkommer föjande resultat:<br>
-Första sidan får resultatet 75 för mobilsidan och 98 för desktop<br>
-Aboutsidan 93 för mobil och 99 för desktop<br>
-Doldsida 73 för mobil och 97 för desktop<br>
-Gallerisidan 72 för mobil och 97 för desktop<br>

Undersöker vad som drar ned resultatet på mobilsidorna och kan konstatera att de största förbättringsområdena som skulle öka laddningshastigheten är eliminate render-blocking resources och preload key requests. Det finns ingen anmärkning på bilderna gällande laddningstider.

<h2>Devtools nätverk.</h2>
Slutligen tittar jag också i den här undersökningen på nätverk under Devtools-verktyget för första sidan och för bildgalleriet. .<br>
Första sidan:
Requests: 13st
Transferred: 42 KB
Resources: 830 KB
Finish: 516 s

Bildgalleriet:
Requests: 25st
Transferred: 51 KB
Resources: 551 KB
Finish: 216 s

Analys
-----------------------
Laddningstiderna för desktop är enligt Lighthouse verktyget bra. För mobilläget finns det förbättringsområden som jag inte har möjlighet att korrigera nu, dock fungerar bildformat och bildstorlekar bra gällande laddningstider. Värdena hamnar ändå för mobilläget inom ramen för måttligt bra, vilket jag i nuläget känner mig nöjd med.
Jämför jag sidorna med laddningstiderna för de sidor jag undersökte i kmom05 är jag positivt överraskad att jag fick så pass bra laddningstider som jag fick. Samtliga sidor som jag undersökte då under kmom05 fick anmärkning på att bildformatet påverkade laddningstiderna på ett negativt sätt. Även i Devtoolsverktyget för nätverk kan man se att min sida tar 516 och 216 ms, medan sidorna i min förra undersökning tog över 4 sek. De sidorna jag undersökte då är mycket större, bildrikare och vissa hade även video så det är svårt att göra någon större jämförelse.  Analysen är att det är viktigt att ha kunskap och kännedom om de saker som påverkar laddningstiderna, det gör skillnad för resultatet. Laddningstider är viktiga då man som skapare av webbplatser har en väldigt kort stund på sig att skapa intresse för vidare läsning på sidan, om dessa värdefulla sekunder läggs på laddningstid tappar man besökare. Därför har det varit väldigt värdefullt att lära sig om detta under kursen. 

Referenser
-----------------------
Google Pagespeed:
<br><br>
http://developers.google.com/speed/pagespeed/insights/
<br><br>
Använt mig av Google Chromes verktyget Lighthouse och Devtools network för att göra mätningar av hastighet och Performance.

Övrigt
-----------------------
Individuellt arbete skrivet av Josefine Bertvig.
