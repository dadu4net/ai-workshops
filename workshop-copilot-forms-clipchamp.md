# Workshop: Copilot in Microsoft Forms en Clipchamp

**Duur:** 2,5 uur (150 minuten, incl. 10 minuten pauze)
**Vorm:** Klassikaal / hands-on (ook online te geven)
**Groepsgrootte:** 6–15 deelnemers (ideaal: max. 12 voor persoonlijke begeleiding)
**Doelgroep:** Eindgebruikers met een Microsoft 365 Copilot-licentie (communicatie, HR, projectleiders, opleiding, teamleiders)
**Niveau:** Beginner tot gemiddeld, geen voorkennis van Forms of Clipchamp nodig
**Stand van zaken:** oktober 2026. Copilot en de menu's in Forms en Clipchamp veranderen regelmatig. Doorloop de demo's en opdrachten daarom altijd een dag voor de workshop zelf.

---

## 1. Doel en leeruitkomsten

**Businessdoel:** deelnemers gebruiken Copilot om sneller en beter enquêtes, quizzen en korte video's te maken, en weten wanneer ze dat juist niet moeten doen.

Na afloop van deze workshop kan de deelnemer:

| # | Leeruitkomst | Bloom-niveau |
|---|---|---|
| 1 | Uitleggen wat Copilot in Forms en Clipchamp doet en welke licentie en accountvorm daarvoor nodig is | Begrijpen |
| 2 | Met Copilot een enquête en een quiz in Forms aanmaken, verbeteren en verspreiden | Toepassen |
| 3 | Met Copilot de reacties in Forms analyseren en de uitkomsten kritisch controleren | Analyseren |
| 4 | Met Copilot een conceptvideo in Clipchamp genereren en daarna handmatig afwerken (tekst, ondertiteling, huisstijl, export) | Toepassen |
| 5 | Per situatie beoordelen of Copilot wel of niet de juiste keuze is (kwaliteit, privacy, tijdwinst) | Evalueren |

---

## 2. Planning in één oogopslag

| Tijd | Duur | Onderdeel | Werkvorm |
|---|---|---|---|
| 0:00 – 0:15 | 15 min | Welkom, doel, licentiecheck, opwarmer | Plenair + korte praktijkcheck |
| 0:15 – 1:10 | 55 min | **Module 1: Copilot in Forms** | Demo → doe-mee → opdrachten |
| 1:10 – 1:20 | 10 min | Pauze | |
| 1:20 – 2:15 | 55 min | **Module 2: Copilot in Clipchamp** | Demo → doe-mee → opdrachten |
| 2:15 – 2:30 | 15 min | Slotcasus, wel/niet-kaart, evaluatie | Duo-opdracht + plenair |

---

## 3. Voorbereiding trainer

### Technisch (minimaal 1 week vooraf controleren)

- [ ] Elke deelnemer heeft een **Microsoft 365 Copilot-licentie** (zonder licentie ontbreekt de Copilot-chat in Forms; in Clipchamp zijn de AI-videofuncties gekoppeld aan Copilot voor werk)
- [ ] Deelnemers gebruiken een **werk- of schoolaccount** (Entra ID), geen persoonlijk Microsoft-account. Dat is een andere versie van Clipchamp met andere functies
- [ ] **Clipchamp is ingeschakeld** door de beheerder in de tenant. Als Clipchamp uitstaat, zien deelnemers een concept maar kunnen ze het project niet openen
- [ ] Forms werkt in de **webbrowser** (Edge of Chrome); de Copilot-chatpane in Forms is webgebaseerd
- [ ] Clipchamp werkt in de browser (aanbevolen: Edge of Chrome). Controleer of er voldoende bandbreedte is voor het uploaden en afspelen van video
- [ ] Wifi, koptelefoons of oordopjes (voor voice-over en voorbeeldfragmenten) en een beamer met geluid
- [ ] Een testaccount zonder Copilot-licentie om te laten zien hoe het scherm er dan uitziet

### Materiaal

- [ ] Korte stockbeelden of eigen clips (3–5 stuks, 10–30 sec) en een logo (PNG) als oefenmateriaal in een gedeelde map
- [ ] Een voorbeeld-enquête met 20+ nepreacties om analyse mee te oefenen (zie bijlage A)
- [ ] Afgedrukte of digitale **wel/niet-kaart** (hoofdstuk 7) en **cheatsheet** (bijlage B)
- [ ] Evaluatieformulier (bijlage C), zelf te maken met Forms, dat is meteen een mooie demonstratie

### Rode draad

Eén **fictief bedrijf** voor alle opdrachten: *Van Dijk Techniek*, een middelgroot installatiebedrijf met 120 medewerkers en een nieuw intranet. Deelnemers mogen ook een eigen praktijkcase gebruiken, **zolang er geen persoonsgegevens, klantnamen of vertrouwelijke info in prompts of video's komt.**

---

## 4. Programma in detail

### 0:00 – 0:15 | Welkom en opwarmer (15 min)

| Min. | Wat | Hoe |
|---|---|---|
| 0–3 | Welkom, doel en programma | Trainer, plenair |
| 3–8 | **Licentiecheck:** open Forms en Clipchamp. Zie je het Copilot-icoon (rechtsonder in Forms)? Staat bij Clipchamp je werkaccount rechtsboven? | Deelnemers doen mee, trainer helpt bij problemen |
| 8–13 | **Opwarmer:** bespreek met je buur: *"Wanneer heb je voor het laatst een enquête of video moeten maken, en wat kostte het meeste tijd?"* | Duo's, 2 antwoorden terug in plenum |
| 13–15 | Afspraken: experimenteren mag, fouten maken is nuttig, geen echte persoonsgegevens gebruiken | Plenair |

**Trainerstip:** schrijf de genoemde tijdvreters op een flipover. Je komt daar aan het einde op terug ("Hebben we er iets aan gedaan?").

---

### 0:15 – 1:10 | MODULE 1: Copilot in Microsoft Forms (55 min)

#### 1.1 Uitleg en demo (15 min: 0:15 – 0:30)

**Wat is Forms?** Een webapplicatie voor enquêtes, quizzen en polls. Reacties komen automatisch in een overzicht en kunnen naar Excel.

**Wat kan Copilot in Forms?** (let op: in de praktijk verschijnt het per gebruiker en per tenant in fases)

| Functie | Wat doet het | Waar vind je het |
|---|---|---|
| **Draft with Copilot** (concept laten schrijven) | Maakt een compleet concept van een enquête of quiz op basis van jouw omschrijving | Bij het aanmaken van een nieuwe vorm |
| **Copilot-chatpane** | Chat naast je formulier: verbeter vragen, pas instellingen aan (bijv. alle vragen verplicht), schrijf een uitnodiging, analyseer reacties | Copilot-icoon rechtsonder in je formulier |
| **Rewrite / Add question** | Herschrijft een vraag of voegt vragen toe op het canvas | Direct bij de vraag |
| **Antwoordtoelichting (quiz)** | Genereert uitleg bij het goede antwoord | In quizmodus |
| **Analyse van reacties** | Vat resultaten samen, benoemt patronen en geeft inzichten | Copilot-chat in het tabblad Reacties |

> **Let op:** de Forms-chatpane is bedoeld voor gebruikers met een Microsoft 365 Copilot-licentie. Zonder licentie zie je deze functies niet.

**Demo door trainer (5 min), live:**

1. Open Forms → *Nieuw formulier* → kies **Draft with Copilot**
2. Prompt: *"Maak een enquête voor medewerkers van een installatiebedrijf over de tevredenheid met het nieuwe intranet. 8 vragen, mix van schaalvragen en open vragen, in het Nederlands, informele toon."*
3. Laat zien: wat klopt, wat is te lang of dubbel, welke vraag is stuurvraag?
4. Open de chatpane en vraag: *"Maak vraag 3 neutraler en maak alle schaalvragen verplicht."*

**Boodschap voor de groep:** Copilot maakt het concept, **jij** bent verantwoordelijk voor de vraagstelling.

#### 1.2 Opdracht 1: Enquête bouwen met Copilot (15 min: 0:30 – 0:45)

**Scenario:** Van Dijk Techniek wil weten hoe medewerkers het nieuwe intranet ervaren. Jij bouwt de enquête.

**Handelingen (stap voor stap):**

1. Ga naar **forms.office.com** (of via het Microsoft 365-portaal) en log in met je werkaccount
2. Klik op **Nieuw formulier** → kies **Draft with Copilot**
3. Schrijf je eigen prompt. Gebruik dit **prompt-skelet:**

   > *Maak een [type formulier] voor [doelgroep] over [onderwerp]. Doel: [wat wil je weten?]. [Aantal] vragen, mix van [vraagtypes]. Taal en toon: [bijv. Nederlands, informeel]. Gebruik geen suggestieve vragen.*

4. Lees het concept en markeer in de kantlijn (of op papier): **wat laat je staan, wat pas je aan, wat verwijder je?**
5. Gebruik de **Copilot-chat** voor minimaal **twee verbeteringen**, bijvoorbeeld:
   - *"Verwijder vragen die overlappen."*
   - *"Voeg een open vraag toe over wat er beter kan."*
   - *"Maak de introductietekst korter en vriendelijker."*
6. Pas minimaal **één vraag zelf handmatig** aan
7. Open **Voorbeeld** (preview) en klik de enquête volledig door

**Resultaat:** een werkende enquête van 6–10 vragen.
**Succescriteria:** geen suggestieve vragen, duidelijke introductietekst, alle schaalvragen verplicht, minimaal één eigen handmatige aanpassing.

**Extra voor snelle deelnemers:** laat Copilot een uitnodigingsmail schrijven en pas die aan jouw tone-of-voice aan.

#### 1.3 Opdracht 2: Quiz maken en analyseren (15 min: 0:45 – 1:00)

**Deel A: quiz maken (8 min)**

1. Nieuwe **quiz** → *Draft with Copilot*
2. Prompt: *"Maak een quiz van 6 meerkeuzevragen over veilig werken op een bouwplaats voor nieuwe medewerkers. Eén juist antwoord per vraag, korte uitleg bij het juiste antwoord."*
3. Controleer **elke vraag inhoudelijk**: is het juiste antwoord ook echt juist? (Copilot kan zelfverzekerd fout zitten)
4. Gebruik **Antwoordtoelichting** voor één vraag en herschrijf de toelichting in eigen woorden

**Deel B: reacties analyseren (7 min)**

1. Open het **voorbeeldformulier met nepreacties** (bijlage A, door trainer gedeeld) of de zojuist gemaakte enquête met reacties van je buurman/buurvrouw
2. Ga naar het tabblad **Reacties** en open de **Copilot-chat**
3. Vraag bijvoorbeeld:
   - *"Vat de belangrijkste uitkomsten samen in 5 punten."*
   - *"Welke thema's komen terug in de open antwoorden?"*
   - *"Welke afdeling is het minst tevreden, en waarom denk je dat?"*
4. **Controleer de analyse:** klopt het met de cijfers in het overzicht? Stel Copilot één kritische vraag: *"Op welke antwoorden baseer je dit?"*

**Reflectievraag (plenair, 1 min):** Waar had Copilot gelijk, waar niet?

#### 1.4 Wanneer wel en wanneer niet: Forms (10 min: 1:00 – 1:10)

Zie ook hoofdstuk 7 voor de volledige tabel. **Werkvorm:** stellingenspel. Trainer leest stelling voor, deelnemers gaan staan (eens) of blijven zitten (oneens).

| Stelling | Bespreekpunt |
|---|---|
| "Ik laat Copilot een klanttevredenheidsenquête schrijven en verstuur hem direct." | Nee: altijd eerst controleren op suggestieve vragen en toon |
| "Ik laat Copilot de open reacties van 300 medewerkers samenvatten." | Ja, goede toepassing, mits je steekproefsgewijs controleert |
| "Ik gebruik Copilot voor een enquête over ziekteverzuim met namen erbij." | Nee: gevoelige persoonsgegevens, eerst AVG-check en overleg met privacy/HR |
| "Ik bouw met Copilot een quiz voor een verplichte veiligheidstraining." | Alleen met inhoudelijke controle door een expert |
| "Ik wil een snelle poll voor lunchvoorkeuren." | Ja, hier is Copilot prima, laagdrempelig en laag risico |

---

### 1:10 – 1:20 | Pauze (10 min)

Tip voor de trainer: laat het beeld met de opdracht van Module 2 al op het scherm staan.

---

### 1:20 – 2:15 | MODULE 2: Copilot in Clipchamp (55 min)

#### 2.1 Uitleg en demo (15 min: 1:20 – 1:35)

**Wat is Clipchamp?** Een online video-editor (browser en Windows-app). De **werkversie** draait op je werk- of schoolaccount; projecten worden opgeslagen in OneDrive of SharePoint.

**Waar zit Copilot in Clipchamp?**

| Functie | Wat doet het | Opmerking |
|---|---|---|
| **Video genereren via Copilot** (Generate a video / Visual Creator) | Op basis van een prompt: script, stockbeelden, titels, overgangen en voice-over. Je krijgt een **conceptvideo** die je in de editor verder bewerkt | Vereist werkaccount met Copilot-licentie en ingeschakelde Clipchamp |
| **Automatische ondertiteling** | Zet gesproken tekst om in ondertitels | Controleer altijd op eigennamen en vakjargon |
| **Transcript bewerken** | Pas de tekst aan en de video volgt | Handig voor het wegknippen van versprekingen |
| **Stiltes verwijderen** | Haalt automatisch pauzes uit je opname | Sneller, maar luister nog even terug |
| **AI-voice-over** (tekst-naar-spraak) | Laat een tekst voorlezen met een gekozen stem | Let op uitspraak van Nederlandse namen |
| **Huisstijl (Brand Kit)** | Vaste logo's, kleuren en lettertypen toepassen | Beschikbaarheid hangt af van je plan en tenant |

> **Let op:** welke AI-functies je precies ziet verschilt per licentie, tenant-instelling en actuele uitrol. Laat deelnemers weten dat sommige functies in hun omgeving anders heten of nog niet aanwezig zijn. Sora-gebaseerde videogeneratie kan op sommige tenants beschikbaar zijn; controleer dat vooraf en demonstreer het alleen als het werkt.

**Demo door trainer (7 min), live:**

1. Open Clipchamp en log in met je werkaccount
2. Klik op **Nieuwe video** (of **Create new video** → paneel **Generate a video**)
3. Prompt: *"Maak een 45 seconden durende welkomstvideo voor nieuwe medewerkers van een installatiebedrijf. Toon: warm en professioneel. Onderwerpen: wie we zijn, wat we doen, waar je hulp vindt."*
4. Wacht tot het concept er staat (meestal 30 sec – 1 min) en bespreek: **wat is bruikbaar, wat is generiek, wat klopt niet bij jullie bedrijf?**
5. Pas de tekst op de tijdlijn aan, verwissel één beeld en laat zien hoe je het logo toevoegt
6. Exporteer als 1080p MP4 (of toon alleen waar de knop staat)

**Boodschap voor de groep:** Copilot geeft je een **eerste draft** in een minuut. De kwaliteit zit in jouw verhaal, je eigen beeldmateriaal en je afwerking.

#### 2.2 Opdracht 3: Conceptvideo genereren en afwerken (20 min: 1:35 – 1:55)

**Scenario:** Van Dijk Techniek wil een korte intranetvideo (30–60 sec) om het nieuwe intranet aan te kondigen.

**Handelingen (stap voor stap):**

1. Open **Clipchamp** en log in met je werkaccount
2. Start een **nieuwe video** en open het **Copilot-paneel** (*Generate a video*)
3. Gebruik dit **prompt-skelet:**

   > *Maak een [duur] video voor [doelgroep] over [onderwerp]. Doel: [wat moet de kijker doen/weten?]. Toon: [bijv. enthousiast, zakelijk]. Structuur: [bijv. opening, 3 kernpunten, afsluiting met call-to-action]. Taal: Nederlands.*

4. Bekijk de preview. **Beoordeel met deze 4 vragen:**
   - Klopt de inhoud met wat wij echt doen?
   - Is de toon passend bij ons bedrijf?
   - Zijn de beelden relevant (geen verkeerde sector, geen stock-cliché)?
   - Past de lengte bij het doel?
5. Open het project in de **editor** en voer **minimaal vier aanpassingen** uit:
   - Pas het **script/tekst op beeld** aan met eigen woorden
   - **Vervang minimaal één stockbeeld** door een eigen clip of beeld uit de gedeelde map
   - Voeg het **logo** toe (PNG uit de gedeelde map) in een hoek
   - Controleer de **muziek en voice-over** (volume, tempo, uitspraak)
6. Sla het project op en exporteer als **1080p MP4**
7. Speel de video 30 seconden af aan je buur en vraag: *"Wat is de boodschap?"*

**Resultaat:** een afgewerkte intranetvideo van 30–60 seconden.
**Succescriteria:** duidelijke boodschap in de eerste 10 seconden, logo zichtbaar, minimaal één eigen beeld, geen foutieve tekst, ondertiteling controleerbaar.

**Extra voor snelle deelnemers:** laat Copilot een tweede variant maken met een andere toon (bijv. informeler) en vergelijk welke beter bij de doelgroep past.

#### 2.3 Opdracht 4: Ondertiteling en transcript (10 min: 1:55 – 2:05)

**Scenario:** Een collega heeft een opname van een korte uitleg (bijv. 30 sec) gemaakt. Maak die toegankelijk en strak.

**Handelingen:**

1. Importeer de **voorbeeldopname met spraak** (door trainer gedeeld) in een nieuw project, of neem zelf 20–30 sec op met de **Opnemer** (webcam + microfoon) in Clipchamp
2. Sleep de clip naar de tijdlijn en ga naar **Ondertitels / Transcript** (zie *Captions* in het zijmenu)
3. Laat **automatische ondertitels genereren** (taal: Nederlands)
4. **Controleer en corrigeer:** zoek minimaal 2 fouten (eigennamen, vakjargon, getallen)
5. Gebruik **Stiltes verwijderen** en luister terug: is het natuurlijker geworden, of worden woorden afgekapt?
6. Kies een leesbare ondertitelstijl (groot genoeg, goed contrast)

**Resultaat:** een video met gecorrigeerde ondertitels.
**Reflectie (1 min):** Hoeveel tijd kostte het corrigeren ten opzichte van handmatig typen?

#### 2.4 Wanneer wel en wanneer niet: Clipchamp (10 min: 2:05 – 2:15)

**Werkvorm:** groepjes van 3. Verdeel de situaties, bespreek 3 minuten en deel je oordeel.

| Situatie | Wel / Niet / Met voorwaarden? |
|---|---|
| Interne aankondiging van een nieuw intranet | **Wel:** laagdrempelig en intern, draft in een minuut |
| Video voor een beurs of externe klantcampagne | **Met voorwaarden:** gebruik eigen beeld en huisstijl; stock en AI-beeld kunnen generiek ogen; controleer rechten |
| Video met herkenbare medewerkers of klanten | **Niet automatisch:** altijd toestemming; geen persoonsgegevens in prompts |
| Uitlegvideo voor een technische of veiligheidsprocedure | **Met voorwaarden:** inhoud door een vakexpert laten controleren; AI-beeld kan onjuiste situaties tonen |
| Snelle ondertiteling van een teamupdate | **Wel:** grote tijdwinst, mits je controleert |
| Een directiebericht met de CEO in beeld | **Liever niet via AI-generatie:** gebruik authentiek beeld; gebruik Clipchamp alleen voor afwerking |
| Video over vertrouwelijke bedrijfsinformatie (bijv. overname) | **Niet** met generieke stock/AI-elementen en alleen binnen de tenant; overleg met Security/Compliance |

---

### 2:15 – 2:30 | Afsluiting (15 min)

| Min. | Wat | Hoe |
|---|---|---|
| 0–7 | **Slotcasus (duo's):** *"Van Dijk Techniek heeft de intranetvideo uitgezonden. Maak met Copilot in Forms een korte feedbackenquête (4 vragen) om te meten of de video duidelijk was. Bedenk welke vraag je níet door Copilot laat schrijven."* | Duo's, korte presentatie van 2 duo's |
| 7–10 | **Terug naar de flipover:** welke tijdvreters uit de opwarmer kunnen nu sneller? Welke blijven mensenwerk? | Plenair |
| 10–13 | **Mijn commitment:** schrijf op een kaartje één ding dat je **morgen** doet met Forms of Clipchamp, en één ding waar je Copilot **bewust niet** voor gebruikt | Individueel |
| 13–15 | **Evaluatie:** scan de QR-code naar het evaluatieformulier (bijlage C), gemaakt in Forms | Individueel |

---

## 5. Kernprincipes voor deelnemers (laat dit op de wand staan)

1. **Copilot maakt het concept, jij maakt het product.** Controleer altijd inhoud, toon en feiten.
2. **Goede prompt = doel + doelgroep + toon + structuur.** Hoe specifieker, hoe beter.
3. **Itereren is normaal.** Eén prompt is zelden genoeg; verfijn met vervolgopdrachten.
4. **Geen persoonsgegevens of vertrouwelijke info in prompts of beeldmateriaal** zonder toestemming en AVG-check.
5. **Wees transparant.** Gebruik je AI voor een externe video of enquête? Houd je organisatiebeleid aan.

---

## 6. Veelvoorkomende valkuilen en hoe je ze herkent

| Valkuil | Herkenning | Oplossing |
|---|---|---|
| Suggestieve vragen in enquêtes | "Hoe tevreden bent u over onze uitstekende service?" | Laat Copilot de vraag neutraal herschrijven en lees zelf na |
| Te lange enquêtes | Copilot levert 15+ vragen af | Vraag expliciet om een maximum aantal vragen |
| Zelfverzekerd foute quizantwoorden | Antwoord klinkt logisch maar klopt niet | Laat een inhoudelijk expert controleren |
| Analyse zonder onderbouwing | Mooie samenvatting, onduidelijke herkomst | Vraag: "Op welke antwoorden baseer je dit?" en vergelijk met cijfers |
| Generieke video | Stock-beeld van mensen in een verkeerde sector | Vervang beeld door eigen materiaal, pas script aan |
| Ondertitelfouten | Verkeerd gespelde namen en jargon | Altijd handmatig doorlezen |
| Functie ontbreekt | Geen Copilot-icoon of geen *Generate a video* | Controleer licentie, accountsoort (werk vs. persoonlijk) en beheerinstellingen |

---

## 7. Wel/niet-kaart: wanneer gebruik je Copilot in Forms en Clipchamp?

### Copilot in Forms

| ✅ Gebruik het wel bij | ❌ Gebruik het niet (of met extra zorg) bij |
|---|---|
| Een eerste concept van een enquête of poll | Enquêtes met gevoelige persoonsgegevens (gezondheid, verzuim, beoordeling) zonder AVG-check |
| Vragen neutraler of korter maken | Juridisch of beleidsmatig bindende formulieren zonder controle |
| Uitnodigingstekst schrijven | Quizzen voor certificering of verplichte trainingen zonder vakinhoudelijke controle |
| Samenvatten van veel open antwoorden | Het enige analysemiddel voor belangrijke besluiten; controleer cijfers altijd zelf |
| Snelle interne polls en feedbackrondes | Verstuurbeslissingen overlaten aan Copilot (wie, wanneer, aan wie) |

### Copilot in Clipchamp

| ✅ Gebruik het wel bij | ❌ Gebruik het niet (of met extra zorg) bij |
|---|---|
| Interne aankondigingen, onboarding, korte updates | Externe campagnes waarvoor unieke, merkdragende beelden nodig zijn |
| Een eerste draft om snel een idee te tonen | Video's met herkenbare personen zonder toestemming |
| Ondertitels, transcript, stiltes verwijderen | Technische of veiligheidsinstructies zonder expertcontrole |
| Huisstijlvolle korte clips met eigen beeld | Vertrouwelijke bedrijfsinformatie in prompts |
| Hergebruik van een bestaand script in een nieuwe vorm | Authentieke boodschappen van directie of leiderschap volledig laten genereren |

### Snelle beslisvragen

1. **Is het risico bij een fout klein?** Dan is Copilot een goede versneller.
2. **Staat er persoonlijke of vertrouwelijke info in?** Dan eerst overleg (privacy, security, HR).
3. **Is authenticiteit of vakkennis cruciaal?** Dan alleen als hulpmiddel, nooit als eindverantwoordelijke.
4. **Kan iemand het resultaat controleren?** Zo nee: niet gebruiken.

---

## 8. Evaluatie en borging (Kirkpatrick)

| Niveau | Wat | Hoe |
|---|---|---|
| **L1 Reactie** | Tevredenheid, bruikbaarheid | Evaluatieformulier direct na afloop (bijlage C) |
| **L2 Leren** | Kunnen ze het? | Resultaten opdrachten 1 t/m 4; observatie door trainer |
| **L3 Gedrag** | Gebruiken ze het? | Vervolgvraag na 30 dagen: *"Hoeveel formulieren/video's heb je sindsdien met Copilot gemaakt?"* |
| **L4 Resultaat** | Tijdwinst en kwaliteit | Meet bij een team: tijd per enquête/video voor en na; aantal gebruikte formulieren |

### Adoptie na de workshop

- **Dag 0:** stuur de cheatsheet (bijlage B) en de promptskeletten per mail
- **Week 1:** korte reminder met één tip ("Probeer morgen één vraag in je enquête neutraler te maken met Copilot")
- **Week 2:** open spreekuur van 30 minuten voor vragen
- **Week 4:** L3-vragenlijst (Forms) en deel 2 succesvoorbeelden binnen de organisatie
- **Champions:** vraag 1–2 deelnemers per afdeling om collega's te helpen en nieuwe vragen te verzamelen

---

## Bijlage A: Voorbeeldmateriaal voor de trainer

**Nepreacties voor analyse-opdracht (maak een formulier met de volgende vragen en vul 20–25 reacties in):**

1. *Hoe tevreden ben je over het nieuwe intranet?* (1–5)
2. *Hoe makkelijk vind je wat je zoekt?* (1–5)
3. *Op welke afdeling werk je?* (Planning / Montage / Administratie / Service)
4. *Wat werkt goed?* (open)
5. *Wat zou je verbeteren?* (open)

Spreid de scores ongelijk (bijvoorbeeld lager bij Montage), en maak in de open antwoorden 2–3 terugkerende thema's (zoekfunctie, mobiele weergave, nieuwsberichten) zodat Copilot iets te vinden heeft.

**Voorbeeldopname met spraak (opdracht 4):** 30 seconden uitleg met enkele vaktermen en eigennamen, zodat de automatische ondertiteling aantoonbaar fouten maakt om te corrigeren.

---

## Bijlage B: Cheatsheet (1 pagina, uitdelen)

**Prompt-skelet Forms**
> Maak een [enquête/quiz/poll] voor [doelgroep] over [onderwerp]. Doel: [wat wil je weten?]. [Aantal] vragen, mix van [vraagtypes]. Taal en toon: [..]. Geen suggestieve vragen.

**Handige vervolgprompts Forms**
- "Maak deze vraag neutraler."
- "Verwijder dubbele vragen."
- "Maak alle schaalvragen verplicht."
- "Schrijf een korte uitnodiging van max. 80 woorden."
- "Vat de resultaten samen in 5 punten en geef aan op welke antwoorden dit is gebaseerd."

**Prompt-skelet Clipchamp**
> Maak een [duur] video voor [doelgroep] over [onderwerp]. Doel: [..]. Toon: [..]. Structuur: [opening, kernpunten, call-to-action]. Taal: Nederlands.

**Checklist na het genereren (video)**
- [ ] Klopt de inhoud met onze organisatie?
- [ ] Eigen beeld toegevoegd?
- [ ] Logo en huisstijl?
- [ ] Ondertitels gecontroleerd?
- [ ] Geen persoonsgegevens of vertrouwelijke info?

**Problemen?**
- Geen Copilot-icoon: controleer je licentie en of je met je werkaccount bent ingelogd
- Clipchamp opent niet: vraag de beheerder of Clipchamp is ingeschakeld
- Functie heet anders: het menu verandert regelmatig; zoek op trefwoord of vraag je champion

---

## Bijlage C: Evaluatieformulier (maak in Forms)

1. Hoe tevreden ben je over deze workshop? (1–5)
2. Hoe zeker voel je je om Copilot in Forms te gebruiken? (1–5)
3. Hoe zeker voel je je om Copilot in Clipchamp te gebruiken? (1–5)
4. Wat ga je **morgen** toepassen? (open)
5. Waar zou je meer uitleg over willen? (open)
6. Mag de trainer je over 30 dagen een korte opvolgvraag sturen? (ja/nee)

**Tip:** laat Copilot dit formulier genereren tijdens de demo van Module 1. Dan laat je de workshop zelf zien als praktijkvoorbeeld.

---

## Trainersnotities: timing en bijsturen

- **Loopt Module 1 uit?** Laat Opdracht 2 deel B (analyse) in duo's doen of verkort het stellingenspel tot 3 stellingen.
- **Loopt Module 2 uit?** Opdracht 4 kan als huiswerk of demo door de trainer; houd minimaal 10 minuten voor de afsluiting.
- **Deelnemers zonder licentie?** Laat ze meekijken in duo's en benadruk dat de licentie een voorwaarde is. Gebruik dit als gesprekspunt voor het uitrolplan.
- **Functies werken anders dan beschreven?** Laat dat gewoon zien: het is een goed voorbeeld van waarom je AI-resultaten én interfaces blijft controleren.
- **Online versie?** Gebruik breakoutrooms voor de duo-opdrachten en laat deelnemers hun scherm delen bij de resultaten.
