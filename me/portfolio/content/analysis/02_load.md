---
Title: Load
Description: Page load report
Template: report
---

Analys av laddningstider och användbarhet
=========================================

I den här rapporten ska tre olika webbplatser analyseras utifrån deras laddningstider.

Urval
-----------------------

Tre helt olika webbplatser kommer att analyseras, för att se om det skiljer mycket mellan stora och små sidor. Följande sidor har valts:

- <a href="https://apple.com" target="_blank" aria-label="Gå till apple.com">apple.com</a> (Stor global sida)
- <a href="https://coop.se" target="_blank" aria-label="Gå till coop.se">coop.se</a> (Stor svensk sida)
- <a href="https://fridasbakblogg.se" target="_blank" aria-label="Gå till fridasbakblogg.se">fridasbakblogg.se</a> (Mindre svensk sida)

Metod
-----------------------

Sidornas laddningstid tas fram genom <i>load</i> i webbläsarens devtool/network. Sidan uppdateras tre gånger utan cache och sedan beräknas medelvärdet av de tre <i>load</i>-värdena.

Följande verktyg har använts under analysen:

- <a href="https://pagespeed.web.dev/" target="_blank" aria-label="Gå till PageSpeed Insights">PageSpeed Insights</a>, mäter en sidas prestanda
- <i>Firefox</i>, webbläsaren som analysen gjordes i

Resultat
-----------------------

<iframe src="https://docs.google.com/spreadsheets/d/e/2PACX-1vSaXDPPelxVNFnexRH6FSZrBm4PEoMiv8U0MsgYISa17i2SdB5xr2ldqXL04aAISwyAj9gPokRGEB5L/pubhtml?gid=0&amp;single=true&amp;widget=true&amp;headers=false" class="sheet" title="Statistik"></iframe>

<a href="https://docs.google.com/spreadsheets/d/1YwWFPrBpnt6B-cJD8avu7UPTF120QjOrtcK8cpFTBTI/edit?usp=sharing" target="_blank" aria-label="Länk till rådata"><i>Länk till rådata</i></a>

<h3>Apple</h3>

![apple](../assets/img/apple.png) {.webb-img}

![förbättring](../assets/img/improve_apple.png) {.webb-img}

<h3>Coop</h3>

![coop](../assets/img/coop.png) {.webb-img}

![förbättring](../assets/img/improve_coop.png) {.webb-img}

<h3>Fridas Bakblogg</h3>

![fridasbakblogg](../assets/img/fridasbakblogg.png) {.webb-img}

![förbättring](../assets/img/improve_fbb.png) {.webb-img}

Analys
-----------------------

Diskutera och analysera de resultaten du fann.

På <a href="https://apple.com" target="_blank" aria-label="Gå till apple.com">apple.com</a> används bilder och filmer som tar ganska stor plats, och därmed ökar på laddningstiden. Hade de minskat storleken på dessa medier så hade laddningstiden såklart minskat, men på en sida som Apple, som säljer telefoner/datorer/klockor osv, är det ganska väsentligt att bilderna visas med högsta möjliga kvalitet för att sälja in produkterna så bra som möjligt. På en sådan sida känns det därför extra viktigt att istället t ex reducera onödig kod och att, som <a href="https://pagespeed.web.dev/" target="_blank">PageSpeed Insights</a> föreslår, skicka bilder i modernare format och koda bilderna mer effektivt.

På <a href="https://coop.se" target="_blank" aria-label="Gå till coop.se">coop.se</a> känns inte bildkvaliteten lika viktig, alla vet ju hur äpplen och bananer ser ut. Här föreslår <a href="https://pagespeed.web.dev/" target="_blank">PageSpeed Insights</a> att man bör använda bilder med rätt storlek och modernare bildformat precis som hos Apple. De föreslår även att aktivera textkomprimering och att reducera CSS som inte används.

På <a href="https://fridasbakblogg.se" target="_blank" aria-label="Gå till fridasbakblogg.se">fridasbakblogg.se</a>, sidan som klarade sig bäst på prestanda-testet, föreslås reducerad JavaScript, ta bort resurser som blockerar renderingen och att använda bilder med rätt storlek.

Några förbättringsförslag som dyker upp på flera av sidorna är reducerad CSS/JavaScript, bilder i modernare format/rätt storlek samt att aktivera textkomprimering.

<a href="https://coop.se" target="_blank" aria-label="Gå till coop.se">coop.se</a> fick överlägset bäst laddningstid, men <a href="https://fridasbakblogg.se" target="_blank" aria-label="Gå till fridasbakblogg.se">fridasbakblogg.se</a> fick ett väldigt bra betyg på prestanda-testet (jag jämför framför allt desktop-resultatet nu). Tiden var ganska bra där också, och jag skulle nog säga att prestandan överväger när tiden inte skiljer avsevärt mycket. <a href="https://apple.com" target="_blank" aria-label="Gå till apple.com">apple.com</a> fick sämst resultat på både prestanda och laddningstid. Därför väljer jag att ranka sidorna såhär:

1. <a href="https://fridasbakblogg.se" target="_blank" aria-label="Gå till fridasbakblogg.se">fridasbakblogg.se</a>
2. <a href="https://coop.se" target="_blank" aria-label="Gå till coop.se">coop.se</a>
3. <a href="https://apple.com" target="_blank" aria-label="Gå till apple.com">apple.com</a>

<br>
De sidorna jag har jämfört nu tycker jag inte har känts långsamma. Den längsta laddningstiden har legat på närmare tre sekunder, så jag skulle nog anse att allt under ca fyra sekunder känns okej. När en sida laddar i mer än fyra sekunder tror jag att det hade börjat klia lite i kroppen. Absolut inget problem egentligen utan det är antagligen ett resultat av dagens stressiga samhälle.

Det hade varit intressant att göra samma test i någon annan webbläsare, för att se om resultatet skiljer sig åt.

Referenser
-----------------------

Inga referenser har använts i denna studie.

Övrigt
-----------------------

Denna rapport har skrivits av: <i>Emelie Eklund</i>
