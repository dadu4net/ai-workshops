# Workshop: Aan de slag met Microsoft 365 Copilot Notebooks

**Duur:** 2 uur (120 minuten, incl. 10 minuten pauze)
**Vorm:** Klassikaal of online, hands-on (demo → doe-mee → zelfstandig oefenen → reflectie)
**Groepsgrootte:** 6–15 deelnemers (bij meer: extra begeleider)
**Niveau:** Beginners tot licht gevorderden Copilot-gebruikers (kennen Copilot Chat al een beetje)

> **Let op voor de trainer:** Copilot Notebooks verandert snel (namen van knoppen, limieten, functies in preview). Doorloop deze workshop **uiterlijk een dag vooraf** zelf in de omgeving van de deelnemers en pas knopnamen en limieten aan. Waar dit document concrete limieten noemt, is dat een momentopname (oktober 2026) — controleer ze op Microsoft Learn.

---

## 1. Doel en leeruitkomsten

**Businessdoel:** Deelnemers gebruiken Copilot Notebooks voor werk waarbij ze **veel bronmateriaal** moeten overzien en verwerken, in plaats van losse prompts in Copilot Chat te blijven stellen.

Na afloop van deze workshop kan de deelnemer:

1. **Uitleggen** wat een Copilot Notebook is en hoe het verschilt van Copilot Chat, Copilot Pages en OneNote. *(Begrijpen)*
2. **Aanmaken** van een notebook met relevante referenties (bestanden, pagina's, links) en daar gerichte vragen over stellen. *(Toepassen)*
3. **Beoordelen** of een taak geschikt is voor Notebooks, of dat een andere aanpak beter past. *(Evalueren)*
4. **Gebruiken** van notebook-instructies en *Quick create* (samenvatting, audio-overzicht, concept-document) om sneller tot een bruikbaar resultaat te komen. *(Toepassen)*
5. **Controleren** van antwoorden op bronverwijzingen en juistheid, en rekening houden met rechten en vertrouwelijkheid. *(Evalueren)*

---

## 2. Randvoorwaarden en voorbereiding

### Voor de deelnemers
- Licentie: Microsoft 365 Copilot (of Copilot Chat, met beperktere mogelijkheden) en een actieve SharePoint- of OneDrive-licentie om notebooks te kunnen aanmaken.
- Toegang tot de **Microsoft 365 Copilot-app** (m365.cloud.microsoft) in de browser.
- Eigen laptop. Mobiel is niet geschikt voor de opdrachten.
- Vraag deelnemers vooraf om **één echte werksituatie** mee te nemen waarbij ze veel documenten moeten doorgronden (voor Opdracht 4). Zorg dat ze daarbij geen vertrouwelijke stukken gebruiken die niet in hun eigen M365-omgeving mogen staan.

### Voor de trainer
- Zet de **oefenmap** klaar in SharePoint of OneDrive en deel die met alle deelnemers (zie hieronder).
- Test of audio-overzichten werken in jullie tenant (dagelijkse limieten en taalondersteuning kunnen verschillen).
- Heb een **plan B** voor als Copilot traag is of een functie ontbreekt: schermopname van de demo's en een vooraf gemaakt voorbeeldnotebook.
- Print of deel de **cheatsheet** (bijlage A).

### Oefenmap "Project Nieuw Intranet" (fictieve casus)
Maak 6 korte documenten (elk 1–3 pagina's). Inhoud mag fictief zijn:

| Bestand | Inhoud |
|---|---|
| `Projectplan Nieuw Intranet.docx` | Doel, scope, planning, budget |
| `Notulen stuurgroep januari.docx` | Besluiten en actiepunten |
| `Notulen stuurgroep februari.docx` | Besluiten, met één besluit dat **afwijkt** van januari |
| `Offerte leverancier A.docx` | Prijs en voorwaarden |
| `Offerte leverancier B.docx` | Prijs en voorwaarden (andere opbouw) |
| `Risicolijst.xlsx` of `.docx` | 8–10 risico's met eigenaar en status |

Voeg bewust **een tegenstrijdigheid** toe (bijvoorbeeld twee verschillende opleverdata) en **een lacune** (geen informatie over migratiekosten). Die gebruik je in Opdracht 2.

---

## 3. Programma in één oogopslag

| Tijd | Min. | Onderdeel | Werkvorm |
|---|---|---|---|
| 0:00 – 0:10 | 10 | Welkom, doel en opwarmer | Uitleg + poll |
| 0:10 – 0:25 | 15 | Module 1: Wat is Copilot Notebooks? | Uitleg + demo |
| 0:25 – 0:50 | 25 | Module 2: Je eerste notebook bouwen | Doe-mee + **Opdracht 1** |
| 0:50 – 1:05 | 15 | Module 3: Wanneer wel, wanneer niet? | Discussie + **Opdracht 2** |
| 1:05 – 1:15 | 10 | **Pauze** | |
| 1:15 – 1:40 | 25 | Module 4: Verdiepen met instructies en Quick create | Demo + **Opdracht 3** |
| 1:40 – 1:55 | 15 | Module 5: Eigen casus | **Opdracht 4** + delen |
| 1:55 – 2:00 | 5 | Afsluiting en vervolgacties | Reflectie |

---

## 4. Uitwerking per onderdeel

### Welkom, doel en opwarmer (10 min)

**Trainer doet:**
1. Heet welkom en benoem het doel: *"Aan het eind weet je wanneer je een Notebook opent in plaats van een gewone Copilot-chat, en heb je er één gebouwd voor je eigen werk."*
2. Laat de agenda zien.
3. Stel een **poll** (hand opsteken of Teams-poll):
   - Wie gebruikt dagelijks Copilot Chat?
   - Wie heeft wel eens een Notebook geopend?
   - Wie heeft wel eens 5+ documenten in één keer willen laten samenvatten of vergelijken?
4. Vraag: *"Waar loop je tegenaan bij Copilot Chat als je met veel documenten werkt?"* Noteer 2–3 antwoorden op een flipover. Kom hierop terug in Module 1.

**Typische antwoorden:** Copilot "vergeet" context; antwoorden gaan over alles in het bedrijf, niet over mijn project; ik moet steeds opnieuw bestanden aanwijzen.

---

### Module 1: Wat is Copilot Notebooks? (15 min)

**Kernboodschap:** Een Notebook is een werkruimte waarin Copilot **alleen put uit de bronnen die jij erin zet** (plus je instructies), en waarin je resultaten bewaart.

**Uitleg (7 min)**

- **Wat het is:** een AI-werkruimte met drie delen: *referenties* (bronnen), *chat* (vragen en opdrachten) en *aangemaakte content* (pagina's, samenvattingen, audio-overzichten).
- **Welke referenties kun je toevoegen:** onder andere Word-, Excel-, PowerPoint- en PDF-bestanden, OneNote-pagina's, Copilot Pages, Loop-componenten, links, vergaderrecaps en tekst die je plakt. Afhankelijk van licentie en uitrol ook SharePoint-sites en -mappen als "levende" bron. *(Controleer wat bij jullie beschikbaar is.)*
- **Limieten:** er geldt een maximum aantal referenties per notebook (bij het schrijven: orde van 100 losse bestanden). Check de actuele limiet.
- **Bronvermelding:** antwoorden verwijzen naar de referenties, zodat je kunt nagaan waar iets vandaan komt.
- **Delen:** je kunt een notebook delen met collega's. Let op: wie je uitnodigt kan bewerken, en collega's zien alleen referenties waar ze zelf rechten op hebben.
- **Opslag:** notebooks staan niet in OneDrive-mappen zoals je gewone bestanden, maar in een eigen opslagcontainer die aan de maker gekoppeld is. Wat gebeurt er als de maker vertrekt? Bespreek dit met jullie beheerder.

**Vergelijking (5 min), laat dit zien op een slide of flipover:**

| | Copilot Chat | Copilot Notebooks | Copilot Pages | OneNote |
|---|---|---|---|---|
| **Zoekt in** | Web en/of je werkdata | **Alleen de referenties in het notebook** (plus instructies) | Wat jij erin plakt of laat genereren | Wat jij erin schrijft |
| **Geheugen** | Per gesprek | **Blijft per project bewaard** | Document dat je samen bewerkt | Langdurig notitieboek |
| **Beste voor** | Snelle vraag, brainstorm | **Project of onderwerp met veel bronnen** | Iets uitwerken en delen | Notities en naslag |
| **Resultaat** | Chat-antwoord | Antwoorden, pagina's, samenvattingen, audio | Gezamenlijk document | Notities |

**Demo (3 min):** Open een leeg notebook en laat de drie delen zien. Nog geen inhoud, alleen de indeling. Laat de **bronverwijzing** zien in een antwoord uit een voorbeeldnotebook.

**Terug naar de opwarmer:** Koppel de problemen die deelnemers noemden aan wat een Notebook oplost.

---

### Module 2: Je eerste notebook bouwen (25 min)

**Aanpak:** Trainer demonstreert elke stap (5 min), deelnemers voeren daarna zelf uit.

#### Demo (5 min)
1. Open de Microsoft 365 Copilot-app en kies **Notebooks**.
2. Kies **Nieuw notebook** en geef een duidelijke naam (bijv. *Project Nieuw Intranet*).
3. Voeg referenties toe via **Referenties toevoegen**. Laat zien hoe je kiest uit OneDrive/SharePoint.
4. Stel een eerste vraag in de chat en laat zien dat het antwoord naar de bronnen verwijst.

#### Opdracht 1: Bouw je notebook en stel gerichte vragen (20 min)

**Doel:** Een werkend notebook met 6 referenties en 4 bruikbare antwoorden.

**Handelingen:**

1. Maak een notebook met de naam **"Project Nieuw Intranet – [jouw naam]"**.
2. Voeg alle 6 bestanden uit de oefenmap toe als referentie.
3. Stel de volgende vragen één voor één en lees elk antwoord kritisch:

   | # | Vraag (prompt) | Wat je leert |
   |---|---|---|
   | a | *"Geef een samenvatting van dit project in maximaal 5 zinnen: doel, planning en budget."* | Basissamenvatting over meerdere bronnen |
   | b | *"Welke besluiten zijn genomen in de stuurgroepen en wie heeft welke actie?"* | Gegevens combineren uit twee notulen |
   | c | *"Vergelijk de twee offertes in een tabel: prijs, looptijd, voorwaarden, risico's."* | Vergelijken en structureren |
   | d | *"Welke drie risico's zijn het meest urgent en waarom?"* | Beoordeling op basis van de risicolijst |

4. Klik bij minstens twee antwoorden op de **bronverwijzing** en controleer of het klopt.
5. **Experimenteer:** zet één bestand tijdelijk uit of verwijder het uit de referenties en stel vraag (a) opnieuw. Wat verandert er?

**Reflectievragen (plenair, 3 min):**
- Hoe verschilden de antwoorden van wat je in gewone Copilot Chat zou krijgen?
- Waren er antwoorden waar je de bron niet kon terugvinden?

**Tip voor de trainer:** Loop rond en let op deelnemers die vage vragen stellen ("vertel me over het project"). Laat ze dezelfde vraag specifieker maken: rol, taak, doel, vorm.

**Prompt-formule om te delen:** *Context (waar gaat het over) + Taak (wat moet er gebeuren) + Vorm (tabel, lijst, aantal woorden) + Doelgroep.*

---

### Module 3: Wanneer wel, wanneer niet? (15 min)

**Kernboodschap:** Notebooks is sterk als je **veel bronnen** hebt en **één onderwerp**. Het is niet de beste tool voor alles.

#### Uitleg (5 min)

**Gebruik Notebooks wanneer:**

| Situatie | Voorbeeld |
|---|---|
| Je werkt aan een **project of onderwerp met veel documenten** | Projectdossier, aanbesteding, klantdossier |
| Je moet **meerdere bronnen vergelijken of samenvoegen** | Offertes, beleidsstukken, notulen over meerdere maanden |
| Je wilt **terugkerend** vragen kunnen stellen aan hetzelfde materiaal | Nieuwe collega inwerken, dossier overdragen |
| Je wilt een **concept maken op basis van bestaand materiaal** | Statusrapportage, memo, presentatie-opzet |
| Je wilt materiaal **snel doornemen** (ook onderweg) | Audio-overzicht van een lang rapport |
| Je wilt **bronnen kunnen controleren** | Antwoord met verwijzing naar de bron |

**Gebruik Notebooks (nog) niet of met voorzichtigheid wanneer:**

| Situatie | Waarom niet | Beter alternatief |
|---|---|---|
| **Snelle losse vraag** of brainstorm | Overkill, bronnen toevoegen kost tijd | Copilot Chat |
| Je hebt **actuele of externe informatie** nodig | Notebook put uit je referenties, niet uit het hele web of hele organisatie | Copilot Chat met webzoekopdracht |
| Je zoekt **iets in alle bedrijfsdata** en weet nog niet waar | Je moet eerst bronnen kiezen | Copilot Chat / zoeken |
| Het gaat om **zeer gevoelige of vertrouwelijke** informatie zonder duidelijke afspraken | Delen en bewaren moet passen bij jullie beleid | Eerst met IT/Security afspreken |
| Je moet **exacte cijfers of berekeningen** garanderen | AI kan fouten maken in rekenwerk | Excel met formules, daarna Copilot voor toelichting |
| Je hebt een **juridisch of medisch bindend** antwoord nodig | AI geeft geen garantie | Specialist raadplegen |
| Je wilt **samen live schrijven** aan één document | Daar is Pages/Word voor | Copilot Pages of Word |
| De bronnen zijn **slecht van kwaliteit** (scans, verouderd, tegenstrijdig) | Afval erin, afval eruit | Eerst bronnen opschonen |
| **Groepsbeheerd, formeel kennisbeheer** is nodig | Notebooks zijn persoonlijk eigendom van de maker | SharePoint-site, kennisbank of agent |

**Vuistregel:** *Heb ik 3 of meer bronnen, één onderwerp en wil ik er meerdere keren iets mee doen? → Notebook. Anders → Chat.*

**Drie werkregels voor verantwoord gebruik:**
1. **Controleer** altijd de bronverwijzing bij belangrijke uitspraken.
2. **Deel bewust:** weet wie toegang krijgt en of die persoon ook de referenties mag zien.
3. **Zet alleen in wat erin hoort:** persoonsgegevens en vertrouwelijke stukken volgen het beleid van jullie organisatie.

#### Opdracht 2: Sorteer de situaties en test de grenzen (10 min)

**Deel A: Kaartensorteren in tweetallen (5 min)**
Geef elk duo 8 situatiekaarten (of toon ze op het scherm). Plaats elke kaart onder **"Notebook"**, **"Chat"** of **"Iets anders"**.

| # | Situatie |
|---|---|
| 1 | Je krijgt vandaag een dossier met 12 documenten en moet morgen een advies schrijven. |
| 2 | Je wilt weten wat de huidige btw-regels zijn voor een specifieke dienst. |
| 3 | Je wilt een nieuwe collega inwerken op een lopend project met veel stukken. |
| 4 | Je zoekt een idee voor een naam van een interne nieuwsbrief. |
| 5 | Je wilt de totale kosten in een Excel-model controleren op rekenfouten. |
| 6 | Je wilt de bevindingen uit vijf evaluatierapporten naast elkaar zetten. |
| 7 | Je wilt een vertrouwelijk HR-dossier laten samenvatten, maar er zijn nog geen afspraken over AI en HR-data. |
| 8 | Je wilt snel een e-mail laten herschrijven in een vriendelijkere toon. |

**Antwoorden (voor de trainer):** 1 Notebook · 2 Chat (actueel, web) · 3 Notebook · 4 Chat · 5 Iets anders (Excel zelf, formules) · 6 Notebook · 7 Eerst afspraken maken met IT/HR · 8 Chat of Copilot in Outlook.

**Deel B: Test de grenzen in je notebook (5 min)**
Ga terug naar je notebook uit Opdracht 1 en stel deze twee vragen:

1. *"Wat zijn de verwachte migratiekosten?"* (Er staat hierover niets in de bronnen.)
   → Hoe gaat Copilot om met ontbrekende informatie? Verzint het iets of geeft het aan dat het niet in de bronnen staat?
2. *"Wanneer wordt het intranet opgeleverd?"* (Tegenstrijdigheid tussen de bronnen.)
   → Signaleert Copilot het verschil, of kiest het stilzwijgend één datum?

**Bespreking (plenair):** Wat zagen jullie? Welke les trek je voor je eigen werk? *(Verwacht: altijd zelf controleren; bij twijfel expliciet vragen "Zijn er tegenstrijdigheden tussen de bronnen?")*

---

### Pauze (10 min)

Laat op het scherm een tip staan: *"Vraag je notebook tijdens de pauze: 'Welke vragen zou een nieuwe projectmedewerker waarschijnlijk stellen?'"*

---

### Module 4: Verdiepen met instructies en Quick create (25 min)

#### Demo (8 min)

**1. Notebook-instructies (3 min)**
Laat zien hoe je instructies instelt die voor **elke** vraag in het notebook gelden. Voorbeeld:

> *"Antwoord altijd in het Nederlands, in heldere taal (B1). Geef eerst de conclusie, dan de onderbouwing. Noem altijd de bron. Als iets niet in de bronnen staat, zeg dat expliciet en verzin niets."*

**2. Quick create (5 min)**
Laat zien welke opties er zijn onder *Quick create* / *Create with Copilot* (afhankelijk van uw tenant), bijvoorbeeld:
- **Samenvatting of briefing** van de hele notebook
- **Audio-overzicht**: een gesproken, gesprekachtige samenvatting. Heeft minstens één referentie nodig, kent dagelijkse limieten en is beperkt tot ondersteunde talen. Controleer dat Nederlands bij jullie werkt, anders in het Engels laten genereren.
- **Concept-document of presentatie** op basis van het notebook (afhankelijk van uitrol, bijvoorbeeld via Word- of PowerPoint-agent)
- **Studiehulpen** zoals een mindmap of studiegids (indien beschikbaar)

Laat zien dat aangemaakte content in het notebook bewaard blijft en dat je het resultaat altijd kunt bewerken.

#### Opdracht 3: Maak een bruikbaar eindproduct (17 min)

**Doel:** Van losse bronnen naar een product dat je morgen kunt gebruiken.

**Handelingen:**

1. **Stel notebook-instructies in** (3 min)
   Plak of schrijf eigen instructies. Neem minimaal op: taal, toon, structuur (conclusie eerst), bronvermelding en wat te doen bij ontbrekende informatie.

2. **Maak een statusupdate voor de directie** (6 min)
   Stel deze prompt aan het notebook:
   > *"Schrijf een statusupdate voor de directie van maximaal 200 woorden over het project Nieuw Intranet. Neem op: stand van zaken, belangrijkste besluiten, top 3 risico's en de volgende stappen. Toon: zakelijk, kort, geen jargon."*
   
   Controleer: klopt alles met de bronnen? Pas aan met een vervolgvraag, bijvoorbeeld *"Maak de toon iets directer en voeg het totaalbudget toe."*

3. **Maak een tweede product naar keuze** (6 min), kies er één:
   - **Audio-overzicht** voor een collega die het project overneemt (luister 1 minuut mee en beoordeel kwaliteit).
   - **Vragenlijst voor de eerstvolgende stuurgroep**: *"Welke 5 vragen moet de stuurgroep volgende maand beantwoorden, op basis van de risico's en open acties?"*
   - **Concept-presentatie of -document** op basis van het notebook, als die optie beschikbaar is.

4. **Vergelijk** (2 min): Wissel met je buur. Wat heeft jouw instructie anders gemaakt dan die van je buur?

**Plenaire reflectie (kort):** Wat was het tijdbesparende moment? Waar moest je zelf nog aanpassen? Welke instructie was het meest effectief?

**Trainer-tip:** Laat 1–2 deelnemers hun instructie voorlezen. Laat zien hoe een instructie met "verzin niets" en "noem de bron" het gedrag aanscherpt.

---

### Module 5: Eigen casus (15 min)

#### Opdracht 4: Bouw een notebook voor je eigen werk (10 min + 5 min delen)

**Doel:** Een eerste notebook waarmee je direct na de workshop verder kunt.

**Handelingen:**

1. Kies de werksituatie die je hebt meegenomen (project, klantdossier, onderzoek, onboarding, beleidsstukken, enzovoort).
2. Maak een **nieuw notebook** met een duidelijke naam.
3. Voeg **minimaal 3 echte referenties** toe (zie de werkregels: geen materiaal dat niet in jullie omgeving hoort).
4. Stel **notebook-instructies** in (hergebruik of pas aan uit Opdracht 3).
5. Stel **drie vragen** die je écht nodig hebt voor je werk.
6. Noteer in je werkboek: *Wat werkte? Wat werkte niet? Wat ga ik volgende week doen?*

**Delen (5 min):** Drie vrijwilligers laten in 60 seconden zien wat ze hebben gebouwd en wat het hen oplevert.

**Als iemand geen eigen casus heeft:** laat die persoon een notebook maken voor *"Mijn eigen onboarding"*, met interne beleidsdocumenten, het personeelshandboek en een paar teamdocumenten.

---

### Afsluiting en vervolgacties (5 min)

**Trainer doet:**

1. **Terugblik op leeruitkomsten:** loop de 5 leeruitkomsten langs en vraag per uitkomst om een duim omhoog of omlaag.
2. **Drie vragen aan de groep:**
   - Wat is je belangrijkste inzicht?
   - Welke taak ga je deze week in een notebook doen?
   - Wat heb je nog nodig?
3. **Vervolgacties** (laat deelnemers één kiezen en opschrijven):
   - Binnen 3 dagen: een eigen notebook voor een lopend project afmaken.
   - Binnen 1 week: een collega laten zien wat je hebt gebouwd.
   - Binnen 2 weken: instructies verfijnen en een herbruikbare "standaardinstructie" delen met het team.
4. **Deel de cheatsheet** en het evaluatieformulier.

---

## 5. Evaluatie (Kirkpatrick)

| Niveau | Wat | Hoe |
|---|---|---|
| **1. Reactie** | Tevredenheid en relevantie | Korte enquête direct na afloop (3 vragen + 1 open vraag), bijvoorbeeld via Microsoft Forms |
| **2. Leren** | Kunnen ze het? | Observatie tijdens Opdracht 1, 3 en 4; ingevulde werkregels en wanneer-wel/niet-sorteren |
| **3. Gedrag** | Gebruiken ze het? | Na 30 dagen: korte check ("Hoeveel notebooks heb je gemaakt? Waarvoor? Wat levert het op?"); eventueel gebruiksrapportage van Copilot via de beheerder |
| **4. Resultaat** | Effect op werk | Gemeten tijdwinst bij 2–3 terugkerende taken (bijv. statusupdate schrijven: van 60 naar 20 minuten) |

**Voorgestelde enquêtevragen (schaal 1–5):**
1. De workshop was relevant voor mijn werk.
2. Ik weet nu wanneer ik een Notebook gebruik en wanneer niet.
3. Ik ga Copilot Notebooks de komende weken zelf gebruiken.
4. Open: *Wat zou je anders willen zien in deze workshop?*

---

## 6. Adoptie na de workshop

- **Dag 0:** Deel de cheatsheet, de standaardinstructie en een voorbeeldnotebook.
- **Week 1:** Korte reminder-mail met één tip per dag (5 dagen) of een korte Teams-post.
- **Week 2:** 30 minuten vragenuurtje (online) voor deelnemers die zijn vastgelopen.
- **Week 4:** Champions delen voorbeelden in een Teams-kanaal of Viva Engage-community ("Wat heb jij gebouwd?").
- **Doorlopend:** Verzamel goede instructies en prompts in een gedeelde bibliotheek.

**Veelvoorkomende bezwaren en antwoorden:**

| Bezwaar | Antwoord |
|---|---|
| "Ik vertrouw het niet, het verzint dingen." | Daarom werk je met bronnen en bronverwijzing. Je controleert altijd zelf. Laat Opdracht 2B zien. |
| "Het kost me meer tijd dan het oplevert." | Bij één documentje klopt dat. Notebooks loont bij veel bronnen en herhaald gebruik. |
| "Mijn documenten zijn vertrouwelijk." | Notebooks volgt je bestaande rechten, maar deel bewust en volg het beleid van de organisatie. Check bij twijfel met IT. |
| "Waarom niet gewoon Copilot Chat?" | Chat voor snelle vragen, Notebook voor project en bronnen. Zie de vuistregel. |

---

## Bijlage A: Cheatsheet (1 pagina, voor deelnemers)

### Wanneer Notebook?
**3+ bronnen · één onderwerp · meerdere keren gebruiken** → Notebook. Anders → Copilot Chat.

### In 5 stappen een goed notebook
1. **Naam:** duidelijk en specifiek.
2. **Referenties:** alleen relevante, actuele bronnen.
3. **Instructies:** taal, toon, structuur, bronvermelding, "verzin niets".
4. **Vragen:** Context + Taak + Vorm + Doelgroep.
5. **Controleer:** klik de bronverwijzing aan bij belangrijke punten.

### Standaardinstructie (kopieer en pas aan)
> Antwoord in het Nederlands, in heldere taal. Geef eerst de conclusie, daarna de onderbouwing in maximaal 5 punten. Noem altijd de bron. Als iets niet in de bronnen staat, zeg dat expliciet en verzin niets. Wijs op tegenstrijdigheden tussen bronnen.

### Handige prompts
- *"Vat dit notebook samen in 5 zinnen voor iemand die het project niet kent."*
- *"Welke besluiten zijn genomen en wie heeft welke actie?"*
- *"Zijn er tegenstrijdigheden tussen de bronnen? Zet ze in een tabel."*
- *"Vergelijk [A] en [B] op prijs, looptijd, voorwaarden en risico's."*
- *"Welke informatie ontbreekt nog om een besluit te kunnen nemen?"*
- *"Welke 5 vragen zou een nieuwe collega stellen? Beantwoord ze."*
- *"Schrijf een statusupdate van maximaal 200 woorden voor de directie."*

### Controleer altijd
- Klopt het met de bron?
- Staat alles erin wat ik nodig heb, of mist er iets?
- Mag deze informatie in dit notebook en mag ik dit delen?

### Niet gebruiken voor
Snelle losse vragen · actuele webinformatie · exacte berekeningen · juridisch/medisch bindend advies · gevoelige stukken zonder afspraken.

---

## Bijlage B: Voorbereidingschecklist voor de trainer

- [ ] Licenties en toegang van alle deelnemers gecontroleerd (Copilot + SharePoint/OneDrive)
- [ ] Oefenmap aangemaakt en gedeeld, met tegenstrijdigheid en lacune erin
- [ ] Workshop zelf doorlopen in de eigen tenant; knopnamen en limieten bijgewerkt
- [ ] Audio-overzicht getest (werkt de taal? dagelijkse limiet?)
- [ ] Voorbeeldnotebook en schermopnamen klaar als plan B
- [ ] Cheatsheet en evaluatieformulier klaar
- [ ] Afspraken met IT/Security over delen en vertrouwelijke data bekend
- [ ] Deelnemers hebben een eigen casus voorbereid
- [ ] Flipover, situatiekaarten (Opdracht 2) en timer klaar

---

## Bijlage C: Tijdsbuffers en inkorten

Loopt de workshop uit? Schrap in deze volgorde:
1. Deel B van Opdracht 2 (grenzen testen) → laat de trainer dit als demo tonen (−5 min)
2. Tweede product in Opdracht 3 → alleen de statusupdate (−6 min)
3. Delen in Opdracht 4 → alleen één voorbeeld (−3 min)

Blijft er tijd over? Voeg toe:
- Een gesprek over **notebook delen met een collega** en wat er met rechten gebeurt.
- Een live demo van een notebook gebouwd rond **vergaderrecaps** van een terugkerend overleg.
