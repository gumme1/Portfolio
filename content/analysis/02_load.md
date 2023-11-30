---
Title: Load
Description: This is our load page.
Template: index
---

Laddningstid
=======================

Denna uppgift utgår på att värdera webbsidors laddningstid och prestanda

Urval
-----------------------

Till uppgiften så har jag valt att undersöka webbsidorna för Tradera, Blocket och secondhand, detta eftersom att vårt samhälle försöker återanvända saker och bidra till hållbar utveckling, och att handla begagnat är ett sätt man kan göra det på. Även för att just sånna här sidor brukar ha mycket bilder, tagna av folk i flera olika storlekar och format.

Metod
-----------------------

Metoden som används är en del verktyg för att mäta laddningstiden på webbsidorna, dessa är <a href="https://pagespeed.web.dev/">Pagespeed</a>, inspektera verktyget inbyggt i webbläsaren samt en .md fil med tabellen för att hålla koll på resultaten. Pagespeed är ett verktyg som bland annat mäter webbsidors prestanda från en skala 1-100, för enkelhetens skull så används procent som prefix här.

Resultat
-----------------------

<table id="myTable">
    <tr>
        <th><i>Sidor</i></th>
        <th><a href="https://www.tradera.com/">Tradera</a></th>
        <th><a href="https://www.blocket.se/">Blocket</a></th>
        <th><a href="https://secondhand.se/">Secondhand</a></th>
    </tr>
    
    <tr>
        <td>Pagespeed - desktop</td>
        <td>59%</td>
        <td>55%</td>
        <td>79%</td>
    </tr>

     <tr>
        <td>Pagespeed - mobile</td>
        <td>28%</td>
        <td>50%</td>
        <td>36%</td>
    </tr>
    
    <tr>
        <td>Pagespeed - medelvärde </td>
        <td>43.5%</td>
        <td>52.5%</td>
        <td>57.5%</td>
    </tr>

    <tr>
        <td>laddningstid - sek</td>
        <td>4.12s</td>
        <td>2.20s</td>
        <td>6.78s</td>
    </tr>
    
    <tr>
        <td>antal resurser</td>
        <td>86</td>
        <td>124</td>
        <td>63</td>
    </tr>

    <tr>
        <td>totala storlek</td>
        <td>5MB</td>
        <td>6.5MB</td>
        <td>6.9MB</td>
    </tr>
</table>

<div class="load-pic-container">
    <img src="../assets/img/kmom05/tradera.png">
    <p><b>Tradera:</b> Tradera hade en av de sämsta resultaten på mobilenheter och hade inte en särskilt bra laddningstid heller, för att tradera ska bättra sig rekommenderas det att de använder bilder i rätt storlek, byter till modernare bild format som webp för bättre komprimering samt att minska JavaScripten som inte används. </p>
</div>

<div class="load-pic-container">
    <img src="../assets/img/kmom05/blocket.png">
    <p><b>Blocket:</b> Blocket, även om de inte hade jätte bra resultat heller på varken desktop eller mobil så var deras laddningstider oerhört mycket bättre än resterande. Förbättringar här gäller med att reducera JavaScripten som ej används, men även att minska påverkan som tredjepartskod har.</p>
</div>

<div class="load-pic-container">
    <img src="../assets/img/kmom05/secondhand.png">
    <p><b>Secondhand:</b> Secondhand hade faktiskt bättre resultat än resterande på desktop enligt pagespeed, detta visades dock inte någon annanstans då laddningstiderna var enorma. Utveckling här skulle med vara att använda bilder i rätt storlek och format </p>
</div>



Analys
-----------------------

<b>Webbsidornas problem: </b>

Genom min undersökning över dessa 3 webbsidor så har jag märkt bilder är ett stort problem, ofta så används bilder i för stor storlek till exempel som slösar på minne. Bildformatet som används är med en stor anledning till att webbsidorna kan ta extra tid att ladda, nyare format som webp komprimerar bilder bättre och behöver då inte ladda in lika mycket jämfört med en jpg eller png bild. Javascript som inte används hänvisar pagespeed också som en stor anledning för sänkt prestanda.


<b>Ranking: </b>

Med resultatet i åtanke så ser min ranking ut så här:

<ol class="mini-list">
<li>Blocket</li>
<li>Secondhand</li>
<li>Tradera</li>
</ol>

<b>Förklaring: </b>
Blocket laddar oerhört mycket snabbare jämfört med Tradera och Secondhand, även om Blocket laddar in mest resurser. Blocket har faktiskt sämst resultat inom desktop kategorin, där Blocket marginellt förlorar mot Tradera, och rejält mot Secondhand. Inom mobil så vinner dock Blocket klart, Blocket verkar vara mycket jämnare medans de resterande svänger enormt mot desktop. Om man skulle ta medelvärdet av desktop och mobil testerna för alla webbsidor så vinner faktiskt Secondhand, men med tanke på deras hemska laddningstider så känner jag att Blocket är en mer värdigare vinnare i detta fallet. Tradera har varken bättre medelvärde eller laddningstider än Blocket och kommer därför sist.

<b>Max tillåtna laddningstid: </b>

Personligen så blir jag frustrerad om laddningen av en sida tar mer än 3 sekunder. Detta betyder med att den enda webbsidan som klarar det från mitt urval är Blocket. Allt på blocket generellt verkar gå snabbare, bilderna på produkter laddas in lika snabbt som jag kan se dem, medans det kan ta lite extra tid på Tradera och Secondhand.

Referenser
-----------------------
<ul class="mini-list">
<li><a href="https://www.tradera.com/">Tradera</a></li>
<li><a href="https://www.blocket.se/">Blocket</a></li>
<li><a href="https://secondhand.se/">Secondhand</a></li>
</ul>

Författare
-----------------------

<i>Anton Gummesson</i> - 2023/11-24


<!-- tradera resulat 
laddtid
4.05s
3.83s
4.47s 

resurser
88
85
84

storlek 5mb

blocket resultat
laddtid
2.24
2.10
2.24

resurser
125
124
124

storlek 6.5mb

secondhand resultat
laddtid
4.16s
6.93s
7.32s

resurser
63

storlek 6.9mb

ojämn, ladda in mycket i början och sidan var såg funktionell ut, men sen kom fler requests in efter 2-3 sekunder igen
-->