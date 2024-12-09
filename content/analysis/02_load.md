---
Title: Laddningstider
Author: loading
Description: Hemsidornas laddningstider.
Template: analyser
---
Hemsidornas laddningstider
===============================
Valet av hemsidor faststår. Det blir på något sätt en påbyggnad och utförlig mätning istället för att ta tre helt nya hemsidor. Anser att detta är mer relevant och intressant för den delen. Redan i tidig skede kunde märkas likheter och intressanta ståndpunkter som hade missats om tre nya hemsidor hade valts. Viktigt att veta i förväg att mätningarna som framgår i analysarken var gjorda tills hemsidans DOMContentLoaded framkom. Därefter så fortsatte såklart hemsidorna att ladda olika element, troligen som ej var behövliga i första taget.

Innan vi raskt går vidare och tittar på analyserna och vidare läser reflektioner ska det påpekas förbättringsförslag samt en sammanfattning av bäst presterande hemsidan. På nummer ett hamnar efter många om och men samt dålig start från förra projektet. Drumvirvel... TGI Fridays. Helt klart en vinnare, kanske inte den snabbaste sidan men det är sidan som blir snabbast funktionell och visuell. Det tar lång tid att ladda alla resurser men de mest behövliga och synliga blir snabbt laddade så att besökarna kan njuta av att navigera hemsidan. På andra plats skulle nog påstå att Astrid Lindgrens värld och Jacy'z får en delad plats. Båda hemsidorna laddar långsamt på mindre bra nät. Tycker även att Jacy's förtjänar plats på grund av sina närmare 30 mb sida i storlek på just bokningssidan. Den sidan som ska ladda fortast har pumpats med massa onödig material.

Några förbättringsförslag är just att ladda viktiga element först, skippa överdrivet mycket stora element och ge tillgång till hemsidan åt besökarna, lite som TGI Fridays gör. Det minmala gränsvärdet enligt mig är att klara testerna i alla fall och det gör samtliga webbplatser på vissa sidor men inte alla och kanske inte ens de viktigaste ibland. För mig uppfattas sidorna väldig snabb men det beror också på att uppkopplingen är 1000 mbit/s.

<iframe class="analysexcel" src="https://docs.google.com/spreadsheets/d/e/2PACX-1vQ6pNJDYs29ty7o4AqvTf6q79SkWCpFAvFfFpoaOVlrUcHtj-c6Wu1OOR1Wb_Qrwml7FVstcVBWldPB/pubhtml?widget=true&amp;headers=false"></iframe>

Astrid Lindgrens värld
-----------------------
Ännu en hemsida med Core Web Vitals Assessment: Failed. På mobilen i alla fall, dator varianten passerar. Dåligt för en hemsida som förmodligen använts mer på mobiler än på datorn. Du ska snabbt kunna göra beställningar och boka. Det är mitt intryck av hemsidan huvudsakliga syfte. Återigen även här importeras fonter som inte används. Min spekulation är att eftersom hemsidan är gjord i WordPress som har vissa standardsaker hängt med i utvald tema, viktigt att avaktivera dessa. Det kluriga är att här i sverige har vi bra uppkoppling och därmed är det svårt för kunden att märka hemsidans långsamma hastighet. Tyvärr tror jag att många besökare kommer även från utlandet för att besöka och då är det viktigt att kunna leverera bra hastighet. Gav även browser errors men återigen om du har varit på Astrid Lindgrens värld så vet du att de har inte ont om besökare. Du har inget val liksom, du beställer oavsett om hemsidan är snabb eller långsam när barnen vill dit.

Utförlig mätning
----------------------------
En väsentlig sida för att mäta är just beställningssidan: <a href="https://biljett.astridlindgrensvarld.se/ticketshop/booking/huvudsasong" target="_blank">Astrid Lindgrens värld beställningssida - huvudsäsong</a>. Tog denna sida eftersom den är en viktig del av verksamheten och målet är att sälja biljetter. Nedan finner du resultaten om Core Web Vitals.

![Screenshot på laddningstid](%assets_url%/img/alv-order.png "Astrid Lindgrensvärld beställningssida - huvudsäsong- laddningstid") {.screenshot}

<table>
<caption>
Core web vitals mobil
</caption>
<thead>
<tr><th>FCB</th><th>LCP</th><th>INP</th><th>TTFB</th><th>CLS</th></tr>
</thead>
<tbody>
<tr><td>1.7s</td><td>2.2s</td><td>147ms</td><td>0.2s</td><td>0.4</td></tr>
</tbody>
</table>

<table>
<caption>
Core web vitals storskärm
</caption>
<thead>
<tr><th>FCB</th><th>LCP</th><th>INP</th><th>TTFB</th><th>CLS</th></tr>
</thead>
<tbody>
<tr><td>1.1s</td><td>1.4s</td><td>69ms</td><td>0.2s</td><td>0.12</td></tr>
</tbody>
</table>

Dessa är upplevelserna av deras kunder, troligen den större andelen är från Sverige. Som jag med till exempel 1000 mbit/s på fiber upplever inga bekymmer med laddningstiden, går blixtsnabbt. Med däremot jag slängde på en throttle i developer console, använde good 3G. Vilket är fortfarande vanligt bland mobiltelefoner. Tog otroliga 23 sekunder att ladda hemsidan, ville stänga ner sidan efter halva tiden hade gått men då dök en laddningscirkel upp som jag inte ens visste fanns. Nästa steg var att jag började se knapparna med olika typer av biljetter och några sekunder senare kom hela sidan fram. Upplevelsen var hemsk om du frågar mig.

Nöjde mig inte där, växlade upp en aning till 4G, nu snackar vi 4 mbit/s. Sidan bör laddas inom en sekund, trots allt en sida som är under 4 mb. Inte riktigt där men resultaten var en aning bättre. Tog totala 8.75 sekunder men efter cirka 7,7 sekunder kunde jag se allt det väsentliga på sidan. På Wi-Fi throttle med 30 mbit/s laddade sidan på otroliga 1.49 sekunder, då får vi ändå ha i åtanke att jag hade fonter och lite andra filer cachade redan, cirka 1.5 mb.

Om vi läser av prestanda diagnosen från PageSpeed Insights så skiljer sig värdena från besökarnas värden otroligt mycket. Du kan läsa nedan resultaten samt ta del av bildflödet som representerar upplevelsen vid första besöket.


![Screenshot på laddningstid](%assets_url%/img/alv-loading.png "Astrid Lindgrensvärld beställningssida - huvudsäsong- laddningstid") {.screenshot}

<table>
<caption>
Prestanda diagnos mobil
</caption>
<thead>
<tr><th>FCB</th><th>LCP</th><th>TBT</th><th>SI</th><th>CLS</th></tr>
</thead>
<tbody>
<tr><td>5.8s</td><td>11.7s</td><td>440ms</td><td>5.8s</td><td>0.09</td></tr>
</tbody>
</table>

På storskärmsvarianten är resultaten en aning bättre men CLS ökar markant och ger röda signaler på en score av 0.36. Detta är sämre i min mening eftersom CLS har hittils klarat sig i testerna på grönt, det enda i egentligen som klarade sig.


Jacy'z hotell och spa
-----------------------
Core Web Vitals Assessment: Failed. Ger upp snart, vill inte utvecklare skapa bra score? Trots att Jacy's uppmuntrar människor att ringa så bör ändå hemsidans laddningstid vara en viktig del. Vid scroll på webbplatsen bilderna flashade till första gången de upptäcktes med hover. Antar att detta är tecken på att javascripten inte laddades in förrän den skulle användas, det var en zoom effekt på mouseover. Det var ju bra i sig, slippa sakta ner hemsidan ännu mer.

Uförlig mätning
---------------------------
Likadant med Jacy'z var huvudtanken att mäta deras bokningssida: <a href="https://booking.jacyzhotel.com/en/package/list" target="_blank">Jacy'z bokningssida</a>. Anledning till detta var att det är där det händer. Helt enkelt dit verksamheten vill rikta folket, till att boka såklart.

![Screenshot på laddningstid](%assets_url%/img/jacyz-bokning.png "Jacy'z bokningssida - laddningstid") {.screenshot}

<table>
<caption>
Core web vitals mobil
</caption>
<thead>
<tr><th>FCB</th><th>LCP</th><th>INP</th><th>TTFB</th><th>CLS</th></tr>
</thead>
<tbody>
<tr><td>2s</td><td>2.6s</td><td>217ms</td><td>0.6s</td><td>0.16</td></tr>
</tbody>
</table>

<table>
<caption>
Core web vitals storskärm
</caption>
<thead>
<tr><th>FCB</th><th>LCP</th><th>INP</th><th>TTFB</th><th>CLS</th></tr>
</thead>
<tbody>
<tr><td>1.2s</td><td>2.8s</td><td>131ms</td><td>0.5s</td><td>0.11</td></tr>
</tbody>
</table>

Problemet med Jacy'z hemsida är att det mest väsentliga var synligt redan efter 20 sekunder på en bra 3G uppkoppling men tills allting laddades krävdes över tre minuter. Det är otroligt lång tid även för 3G, vi pratar om knappt över 3MB. En stor andel av detta var även cachad material. De hade också något script som gjorde API calls ständingt så det lade på laddningstiden i stort sett varje gång sidan tabbades ut.

Även på Jacy'z kunde besökarna uppleva en vit skärm innan någonting ens syntes på hemsidan. Inte lika länge som på Astrid Lindgrens värld dock. Måste erkänna att det gjorde saken mindre frustrerande.

![Screenshot på laddningstid](%assets_url%/img/jacyz-loading.png "Jacy'z - laddningstid") {.screenshot}

<table>
<caption>
Prestanda diagnos mobil
</caption>
<thead>
<tr><th>FCB</th><th>LCP</th><th>TBT</th><th>SI</th><th>CLS</th></tr>
</thead>
<tbody>
<tr><td>6.3s</td><td>17.6s</td><td>1,010ms</td><td>9.7s</td><td>0.111</td></tr>
</tbody>
</table>

Trots sämre resultat på tester så presterade Jacy'z en aning bättre rent visuellt och upplevelsemässigt. Skillnaden var att på Jacy'z sida kunde du se en ram och suddighet innan element laddades färdigt medan på Astrid Lindgrens värld var skärmen vit eller hade en laddnings effekt. Det positiva med Jacy'z var att du kunde i alla fall börja scrolla och titta på annat, behövde ej invänta laddning.

En sak som utmärktes vid laddning av order sidan var att den första synliga bilden laddades efter de andra bilderna som låg längre ner på sidan. Menar en sida som är cirka 25 mb bör ändå prioritera det som syns först. Med tanke på att deras andra sidor var mycket mindre i storlek, då får det mig att tänka den sidan kanske inte är så optimerad och fokuserad på syftet. Enligt mig är syftet att besökare ska göra bokningar, då är andra element inte lika viktiga.

TGI Fridays
-----------------------

Rent ut sagt kasst. Mycket third party-scripts som hemsidan är uppkopplad mot. Första gången som mina ögon märker Core Web Vitals Assessment: Failed på en hemsida för ett bolag av den storleken. Även på desktop, det var ju ännu mer ovanligt. En dubbelmacka får det bli, trots det så är maten god och det som räknas. Det tråkiga är att det kan göras order online och då förväntas att hemsidan ska vara kvick. CLS:en var bra, så något rätt gjorde utvecklarna.

![Screenshot på laddningstid](%assets_url%/img/fridayload.png "TGI Fridays laddningstid") {.screenshot}

Uförlig mätning
---------------------------
Tyvärr eftersom Cloudflare blockade mig kunde jag inte utföra en ordentlig testning på: <a href="https://order.tgifridays.com/" target="_blank">TGI Fridays order sida</a>. Ville även där se hur deras bokningssida beter sig. Lyckades dock att hämta Core web vitals värden men genom developer tools var tvungen att välja annan sida. Då valdes sida "<a href="https://locations.tgifridays.com/" target="_blank">Location</a>" eftersom den också är en viktig sida för att besökarna ska kunna hitta till restaurangerna.

![Screenshot på laddningstid](%assets_url%/img/tgi-location.png "TGI Fridays - Location sida - laddningstid") {.screenshot}

<table>
<caption>
Core web vitals mobil
</caption>
<thead>
<tr><th>FCB</th><th>LCP</th><th>INP</th><th>TTFB</th><th>CLS</th></tr>
</thead>
<tbody>
<tr><td>2.6s</td><td>2.5s</td><td>296ms</td><td>0.5s</td><td>0.01</td></tr>
</tbody>
</table>

<table>
<caption>
Core web vitals storskärm
</caption>
<thead>
<tr><th>FCB</th><th>LCP</th><th>INP</th><th>TTFB</th><th>CLS</th></tr>
</thead>
<tbody>
<tr><td>2.3s</td><td>2.4s</td><td>225ms</td><td>0.4s</td><td>0.01</td></tr>
</tbody>
</table>

Det som var intressant med TGI Fridays sida är att resultaten mellan mobil och storskärmen skiljde sig nästan ingenting. Oftast har det märkts tydliga skillnader i den bemärkelsen. En annan aspekt som uppmärksammades att deras sida även på 3G laddades på 4 sekunder såpass mycket att det mesta var synligt och användbart. Det tog cirka 21 sekunder för att resterande viktigt innehåll skulle laddas. Alltså till skillnad från Jacy'z och Astrid Lindgrens värld som behövde över 20 sekunder för att ens kunna använda sidan ordentligt på ett bra 3G nät, vilket är dåligt i vår samhälle kan vi ändå konstatera att TGI Friday på 4 sekunder levererade det mest väsentliga på sämta mätta nätverk. På Wi-Fi laddades 20 requests mer på nästan samma tid som på 4G, det gick så fort att det var svårt att hänga med på laddningstiden. Kontentan är att utvecklarna på TGI Fridays fokuserade på att viktig innehåll ska snabbt synas och kunna kommas åt. Vilket enligt mig är bra mycket viktigare än att sitta och vänta på sidor ska laddas. Redan efter en sekund var hemsidan synlig och användbar, knappt att du hinner blinka.

![Screenshot på laddningstid](%assets_url%/img/tgi-loading.png "TGI Fridays - Order sida - laddningstid") {.screenshot}

Bilden vi ser är order sidan. Men även location sidan visar ett par vita rutor innan det laddas färdigt med PageSpeed Insight. Enligt min upplevelse är detta helt fel. PageSpeed Insight beskriver att sidan testas med 4G throttle. Mina tester med 3G som är mycket lägre visade inga sådana resultat. Börjar bli tveksam om dessa tester är ens tillförlitliga. Nedan kan du även se screenshot för location sidan.

![Screenshot på laddningstid](%assets_url%/img/tgi-location-loading.png "TGI Fridays - Location sida - laddningstid") {.screenshot}