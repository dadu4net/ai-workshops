# Slides met sprekernotities: Copilot Agents & Copilot Studio

**Duur:** 2,5 uur | **Aantal slides:** 29 | **Bij dit materiaal:** deelnemerswerkboek, draaiboek

**Leeswijzer per slide:**
- **Op de slide:** wat deelnemers zien (kort houden)
- **Visual:** suggestie voor beeld of schema
- **Sprekernotities:** wat jij zegt en doet
- **Tijd:** richttijd

> **Voor de sessie:** controleer menunamen, licentiemodel en naamgeving (Microsoft 365 Copilot / Microsoft Copilot) in je testtenant. Zie het draaiboek, sectie 0.

---

# BLOK 0: OPENING (0:00 – 0:10)

## Slide 1: Titel

**Op de slide**
- Copilot Agents & Copilot Studio
- Van slimme assistent naar eigen digitale collega
- [Naam trainer] | Buro GEKKO

**Visual:** Rustig titelbeeld, logo.

**Sprekernotities**
- Welkom heten, jezelf kort voorstellen (1 minuut).
- Zeg: "Vandaag bouwen jullie zelf twee agents. Geen programmeerkennis nodig, wel een laptop."
- Laat het werkboek zien en vraag of iedereen het heeft.

**Tijd:** 1 min

---

## Slide 2: Agenda en afspraken

**Op de slide**
- 5 modules, 2 pauzemomenten (kort + pauze)
- Afspraken: laptop open, vragen stellen mag altijd, fouten maken mag (en is de bedoeling)
- Alles wat we bouwen is oefenmateriaal in een testomgeving

**Visual:** Tijdlijn met de 5 modules.

**Sprekernotities**
- Loop de agenda in 30 seconden door. Benoem dat er twee echte bouwmomenten zijn: Agent Builder (30 min) en Copilot Studio (40 min).
- Zeg dat het werkboek ook na de sessie bruikbaar is als naslag.
- Benadruk: "Als iets niet lukt, vraag het meteen. Dan loopt niemand achter."

**Tijd:** 2 min

---

## Slide 3: Wat kun je na vandaag?

**Op de slide**
- Uitleggen wat een agent is
- Kiezen: agent, Agent Builder, Copilot Studio of juist niet
- Een kennisagent maken
- Een agent bouwen die iets *doet*
- Risico's en beheer benoemen
- Een eigen use case uitwerken

**Visual:** Zes iconen of vinkjes.

**Sprekernotities**
- Dit zijn de leeruitkomsten. Lees ze niet voor, laat ze één keer zien en zeg: "Aan het eind vinken we deze af."
- Doe nu de check-in: handopsteken (1) wie heeft al eens een agent gemaakt, (2) wie gebruikt dagelijks Copilot, (3) wie maakt zich zorgen over controle of veiligheid.
- Vraag elke deelnemer één zin: welk proces zou je graag slimmer maken? Schrijf op flipover: de **use case-parkeerplaats**. Terug in de afsluiting.

**Tijd:** 7 min

---

# BLOK 1: WAT ZIJN AGENTS? (0:10 – 0:30)

## Slide 4: Van Copilot naar agent

**Op de slide**

| | Copilot | Agent |
|---|---|---|
| Gedrag | Algemeen | Specifiek, vaste rol |
| Kennis | Werkdata + web | Bronnen die jij kiest |
| Instructies | Steeds opnieuw | Eenmalig vastgelegd |
| Handelingen | Vooral tekst | Kan acties uitvoeren |

**Visual:** Twee kolommen: "slimme stagiair" versus "stagiair met functieomschrijving".

**Sprekernotities**
- Gebruik de analogie: "Copilot is een slimme stagiair die alles een beetje kan. Een agent is dezelfde stagiair, maar nu met een functieomschrijving, een eigen map met documenten en een paar vaste taken."
- Benoem dat de kracht zit in **beperking**: een agent die minder weet, maar betrouwbaarder is.
- Vraag: "Welke vraag krijg jij elke week van collega's?" (2 voorbeelden uit de zaal ophalen.)

**Tijd:** 5 min

---

## Slide 5: De vier bouwstenen

**Op de slide**
1. **Instructies**: rol, toon, grenzen
2. **Kennis**: SharePoint, bestanden, websites
3. **Tools/acties**: flows, connectors, API's
4. **Triggers en kanalen**: waar en wanneer

**Visual:** Vier blokken om een centrale agent heen.

**Sprekernotities**
- Dit is het ezelsbruggetje voor de hele dag. Elke agent die we vandaag bouwen bestaat uit deze vier.
- Agent Builder gebruikt vooral 1 en 2. Copilot Studio voegt 3 en 4 toe.
- Zeg: "Als een agent niet goed werkt, kijk dan eerst naar 1 en 2. Daar zit 80% van de problemen."

**Tijd:** 5 min

---

## Slide 6: Drie soorten agents

**Op de slide**

| Soort | Waar | Voorbeeld |
|---|---|---|
| Kennisagent | Agent Builder | Vraagbaak personeelsbeleid |
| Studio-agent | Copilot Studio | Meldpunt met actie |
| Autonome agent | Copilot Studio | Verwerkt zelf inkomende mails |

**Visual:** Trap met drie treden: eenvoudig → krachtig.

**Sprekernotities**
- Zeg: "Begin op de onderste trede. De meeste organisaties hebben genoeg aan kennisagents en een paar Studio-agents."
- Noem kort dat Microsoft ook kant-en-klare agents levert (bijvoorbeeld Researcher en Analyst). "Die hoef je niet te bouwen."
- Autonome agents alleen noemen, niet bouwen: "Daar hoort extra governance bij."

**Tijd:** 5 min

---

## Slide 7: Demo: test een agent

**Op de slide**
- Drie vragen aan de HR-agent:
  1. Antwoord staat in de bron
  2. Vraag buiten de bron
  3. Tegenstrijdige bron

**Visual:** Schermopname of live demo.

**Sprekernotities**
- **Live demo** met de kant-en-klare "Vraag het HR"-agent op de workshopsite.
- Vraag 1: laat zien dat de agent een bronverwijzing geeft.
- Vraag 2 (bijvoorbeeld "Wat is de hoofdstad van Frankrijk?"): laat zien dat de agent weigert of aangeeft het niet te weten.
- Vraag 3: gebruik een bewust tegenstrijdig document en laat zien wat er gebeurt.
- Vraag aan de groep: "Wat zegt dit over de kwaliteit van de bron die je koppelt?"
- **Leerpunt, laat de groep het zeggen:** een agent is zo goed als zijn bron en zijn instructies.

**Tijd:** 5 min

---

# BLOK 2: WANNEER WEL, WANNEER NIET? (0:30 – 0:45)

## Slide 8: Wanneer wél een agent

**Op de slide**
- Vraag komt vaak terug
- Antwoord staat in actuele documenten
- Duidelijk begin en einde
- Fout is beperkt of controleerbaar
- Echte tijdwinst

**Visual:** Vijf vinkjes.

**Sprekernotities**
- Lees niet voor. Vraag de groep: "Welke van deze vijf is bij jullie use case het zwakst?"
- Benadruk "actuele documenten": een agent maakt een rommelige bron niet beter, maar zichtbaarder.
- Noem een drempelwaarde als hulpmiddel: "Als het meer dan 10 minuten per keer kost en meerdere mensen het doen, is het een kandidaat."

**Tijd:** 2 min

---

## Slide 9: Voorbeelden uit de praktijk

**Op de slide**

| Use case | Type |
|---|---|
| Vraagbaak personeelsbeleid | Agent Builder |
| Onboarding-buddy | Agent Builder |
| Facilitair meldpunt met actie | Copilot Studio |
| IT-servicedesk eerste lijn | Copilot Studio |
| Triage inkomende klantmails | Autonome agent |

**Visual:** Tabel met iconen per use case.

**Sprekernotities**
- Kies 2 of 3 voorbeelden die passen bij de zaal. Vraag: "Herkennen jullie dit?"
- Bij het meldpunt: "Dit bouwen we straks zelf."
- Bij de autonome agent: "Mens beslist bij uitzondering. De agent doet het voorwerk."

**Tijd:** 2 min

---

## Slide 10: Wanneer NIET

**Op de slide**
- Bron is verouderd of tegenstrijdig → eerst opschonen
- Eenmalige taak → gewoon Copilot Chat
- Vast proces zonder taalbegrip → Power Automate
- Hoog risico bij een fout → mens beslist
- Rechten niet op orde → eerst fixen
- Geen eigenaar → niet beginnen

**Visual:** Stopbord of rood kruis per regel.

**Sprekernotities**
- Dit is de slide waarmee je als adviseur geloofwaardig bent. Neem er de tijd voor.
- Geef een voorbeeld bij "rechten niet op orde": "Een agent toont wat de gebruiker mag zien. Als rechten te ruim staan, wordt oversharing ineens heel zichtbaar."
- Bij "hoog risico": bonus, ontslag, medische of juridische besluiten. "AI mag voorbereiden, de mens beslist."
- Noem de **extra toets**: wat is het ergste dat er kan gebeuren?

**Tijd:** 3 min

---

## Slide 11: Beslisboom

**Op de slide**

```
Vaak terugkerend? → Antwoord in actuele docs?
→ Moet de agent iets DOEN?
   Nee → Agent Builder
   Ja  → Vast stappenplan? → Power Automate
         Anders → Copilot Studio
```

**Visual:** Schematische beslisboom (zie werkboek).

**Sprekernotities**
- Loop de boom één keer door met het voorbeeld "vragen over verlof" (eindigt bij Agent Builder).
- Doe daarna het voorbeeld "melding aanmaken" (eindigt bij Copilot Studio).
- Wijs naar de werkboekpagina: "Deze boom zit ook in jullie werkboek."

**Tijd:** 3 min

---

## Slide 12: Opdracht 1: Agent of niet?

**Op de slide**
- In tweetallen, 5 minuten
- 6 situaties (werkboek, Opdracht 1)
- Kies: Copilot Chat / Agent Builder / Copilot Studio / Power Automate / Geen AI
- Schrijf je reden op

**Visual:** Timer van 5 minuten.

**Sprekernotities**
- Start de timer. Loop rond en luister mee.
- Nabespreking (laatste 2 minuten): vraag bij welke situatie het oneens was. Verwachte antwoorden: 1 Agent Builder, 2 Copilot Chat, 3 Power Automate, 4 Copilot Studio, 5 Geen AI, 6 Copilot Studio.
- Benadruk: "Soms zijn meerdere antwoorden verdedigbaar. Het gaat om de redenering."

**Tijd:** 5 min

---

# BLOK 3: AGENT BUILDER (0:45 – 1:15)

## Slide 13: Goede instructies

**Op de slide**
```
ROL / DOEL / BRONNEN / TOON / GRENZEN / FORMAAT
```
- "Verzin nooit een antwoord"
- "Verwijs naar [persoon] als het niet in de bron staat"

**Visual:** Instructiesjabloon als kader.

**Sprekernotities**
- Dit sjabloon staat in het werkboek en in de spiekbrief.
- Leg uit: GRENZEN is het belangrijkste onderdeel. "Zonder grens probeert een agent behulpzaam te zijn, ook als hij het niet weet."
- Laat een slechte en een goede instructie naast elkaar zien: "Wees behulpzaam" tegenover het volledige sjabloon.

**Tijd:** 3 min

---

## Slide 14: Veelgemaakte fouten

**Op de slide**
- Te vage instructies
- Te veel bronnen ("de hele SharePoint")
- Geen grens voor wat de agent niet mag
- Nooit testen met lastige vragen

**Visual:** Vier waarschuwingsiconen.

**Sprekernotities**
- Vraag: "Welke van deze fouten maak je waarschijnlijk zelf?" (Humor mag: bijna iedereen begint met te veel bronnen.)
- Leg uit: minder bronnen geeft betere antwoorden, ook al voelt het tegenintuïtief.
- Kondig de testlog aan: "Straks testen jullie systematisch, niet op gevoel."

**Tijd:** 2 min

---

## Slide 15: Opdracht 2: Bouw "Vraag het HR"

**Op de slide**
1. Copilot → Agents → Agent maken → Configureren
2. Naam, beschrijving, instructies (sjabloon)
3. Kennis: alleen `Personeelshandboek.docx`
4. 3 startprompts
5. Testen (werkboek, testlog)
6. Aanmaken, niet delen

**Visual:** Stappenplan met nummers.

**Sprekernotities**
- Doe stap 1 tot 4 **live voor**, deelnemers doen mee (8 minuten).
- Laat deelnemers daarna zelfstandig testen en aanpassen (10 minuten). Loop rond.
- Let op: veel deelnemers koppelen de hele site. Corrigeer vriendelijk: "Alleen het handboek."
- Snelle deelnemers: extra uitdaging, tweede bron toevoegen.
- Als de groep achterloopt: sla de startprompts over.

**Tijd:** 20 min

---

## Slide 16: Testen: altijd vier soorten vragen

**Op de slide**
1. Vraag die in de bron staat
2. Vraag buiten het onderwerp
3. Vraag die niet in de bron staat
4. Vraag waarmee iemand de agent probeert te misleiden

**Visual:** Vier vragen als speelkaarten.

**Sprekernotities**
- Laat deelnemers hun testlog bekijken: hebben ze alle vier de soorten getest?
- Vraag 2 deelnemers wat ze moesten aanpassen in hun instructies en wat het effect was. Dit is het **verbeterloopje**.
- Sluit af met: "Testen en bijsturen is geen bijzaak, het is het werk."
- Reflectie in tweetallen (2 min): welke instructie had het grootste effect, welke bron koppel je nooit?

**Tijd:** 5 min

---

# PAUZE (1:15 – 1:25)

## Slide 17: Pauze

**Op de slide**
- 10 minuten
- Terug om 1:25
- Tip: laat je agent open staan

**Visual:** Koffie.

**Sprekernotities**
- Controleer tijdens de pauze of iedereen toegang heeft tot Copilot Studio (`copilotstudio.microsoft.com`) en of de SharePoint-lijst "Facilitaire meldingen" bereikbaar is.
- Open zelf je demo-omgeving in Copilot Studio.

**Tijd:** 10 min

---

# BLOK 4: COPILOT STUDIO (1:25 – 2:05)

## Slide 18: Copilot Studio in één oogopslag

**Op de slide**
- **Overzicht**: functieomschrijving
- **Kennis**: naslagwerken
- **Tools**: de handen van de agent
- **Onderwerpen**: het draaiboek
- **Testen**: proefrit
- **Publiceren / Kanalen**: waar de agent beschikbaar is
- **Analyse**: rapportage

**Visual:** Screenshot met genummerde labels.

**Sprekernotities**
- Doe een korte rondleiding (3 minuten) in de echte omgeving. Wijs elk onderdeel aan.
- Zeg: "In Agent Builder zat dit allemaal in één scherm. Hier is het uitgesplitst. Dat geeft meer macht, maar ook meer verantwoordelijkheid."
- Let op: menunamen kunnen afwijken. Zeg dat expliciet.

**Tijd:** 4 min

---

## Slide 19: Agent Builder of Copilot Studio?

**Op de slide**

| Behoefte | Agent Builder | Copilot Studio |
|---|---|---|
| Vragen beantwoorden uit M365 | Ja | Ja |
| Handeling uitvoeren | Beperkt | Ja |
| Vaste gesprekken | Nee | Ja |
| Externe systemen | Beperkt | Ja |
| Publiceren op website | Nee | Ja |
| Autonoom starten | Nee | Ja |
| Bouwtijd | Minuten | Uren/dagen |

**Visual:** Vergelijkingstabel.

**Sprekernotities**
- Zeg: "Begin klein. Veel agents blijven prima in Agent Builder. Je gaat naar Studio als de agent moet handelen of buiten Copilot moet werken."
- Licentie: Agent Builder zit in de Copilot-licentie. Bij Copilot Studio hangt het af van gebruik en publicatie (Copilot Credits). Verwijs naar slide 25.
- Een Agent Builder-agent kan later worden doorontwikkeld in Copilot Studio.

**Tijd:** 4 min

---

## Slide 20: Opdracht 3: Meldpunt Facilitair

**Op de slide**
- Agent beantwoordt vragen (kennis)
- Agent maakt een melding aan (actie)
- Beschikbaar in Teams
- 6 stappen, 30 minuten (werkboek, Opdracht 3)

**Visual:** Schema: vraag → agent → lijstitem.

**Sprekernotities**
- Leg het scenario in 1 minuut uit: collega's melden storingen via mail en op de gang, wij maken een meldpunt.
- Zeg dat ze **het werkboek volgen** en dat jij per stap kort voordoet.
- Kondig aan dat de stappen 4 en 5 het lastigst zijn.

**Tijd:** 2 min

---

## Slide 21: Het onderwerp en de actie

**Op de slide**
- Onderwerp "Storing melden" met 5 triggerzinnen
- 3 vragen → variabelen `Locatie`, `Omschrijving`, `Urgentie`
- Tool: SharePoint → Item maken
- Bericht: "Je melding is vastgelegd. Urgentie: {Urgentie}"

**Visual:** Flow met drie vragen en één actie.

**Sprekernotities**
- Doe stap 4 en 5 **live voor**, en laat deelnemers daarna zelf verder gaan.
- Leg het begrip **variabele** uit: "Een antwoord dat de agent onthoudt en later invult."
- Bij de connector: "Dit is een verbinding met jouw rechten. De agent kan dus alleen wat jij mag." Laat inloggen als daarom gevraagd wordt.
- Veelvoorkomend probleem: connector vraagt om verbinding. Zie probleemoplossing in het werkboek.
- Loop rond. Help gericht, geef niet direct het antwoord.

**Tijd:** 18 min (werktijd deelnemers)

---

## Slide 22: Testen en publiceren

**Op de slide**
- Test: "De printer op de eerste verdieping is kapot, het is urgent"
- Controleer: staat er een nieuw item in de lijst?
- Publiceren → Kanalen → Teams en Copilot (alleen jij)
- Test ook: "Verwijder alle meldingen"

**Visual:** SharePointlijst met nieuw item.

**Sprekernotities**
- Laat 2 deelnemers hun lijstitem laten zien. Dit is het wow-moment: een gesprek leidt tot een echte handeling.
- Vraag: "Wat gebeurde er bij 'Verwijder alle meldingen'?" Antwoord: de agent kan het niet, want er is geen tool voor. "Een agent kan alleen wat je hem geeft."
- Extra uitdaging voor snelle deelnemers: mail of Teams-bericht na aanmaken. Vraag: welk extra risico brengt dat mee?
- Reflectie (2 min): welke stap was het moeilijkst, wat heb je nodig om dit in je team te bouwen?

**Tijd:** 6 min

---

# BLOK 5: BEHEER, RISICO'S EN KOSTEN (2:05 – 2:20)

## Slide 23: Vijf beheervragen

**Op de slide**
1. **Eigenaar**: wie is verantwoordelijk?
2. **Bronnen**: wie houdt ze actueel?
3. **Rechten**: wie mag wat?
4. **Acties**: wat mag de agent doen, wie controleert?
5. **Levenscyclus**: wanneer evalueren en opruimen?

**Visual:** Vijf kaarten.

**Sprekernotities**
- Zeg: "Bouwen is makkelijk. Beheren is waar het werk zit."
- Laat deelnemers in het werkboek de vijf vragen beantwoorden voor hun Meldpunt Facilitair (3 minuten).
- Vraag: "Bij wie ligt dit bij jullie?" Vaak blijkt: bij niemand. Dat is de les.

**Tijd:** 5 min

---

## Slide 24: Risico's en maatregelen

**Op de slide**

| Risico | Maatregel |
|---|---|
| Verkeerde antwoorden | Beperkte bronnen, review |
| Oversharing | Rechten en labels eerst |
| Ongewenste acties | Minimale rechten, bevestiging |
| Agent-wildgroei | Register, opschoonbeleid |
| Kosten lopen op | Verbruik monitoren |
| Schaduw-IT | Maker-beleid, DLP |

**Visual:** Risicotabel met kleurcodering.

**Sprekernotities**
- Kies twee risico's uit en geef een voorbeeld: oversharing (agent toont wat de gebruiker toevallig mag zien) en wildgroei (80 half verlaten agents).
- Positioneer als adviseur: "Hier komt governance om de hoek. Een agent is pas volwassen als iemand hem beheert."
- Noem dat beheerders agents kunnen reguleren (wie mag maken, delen, publiceren) en dat DLP-beleid van de Power Platform ook geldt voor Copilot Studio.

**Tijd:** 4 min

---

## Slide 25: Kosten in vogelvlucht

**Op de slide**
- **Agent Builder**: in de Copilot-licentie
- **Copilot Studio**: verbruik in **Copilot Credits** (extern publiceren, gebruikers zonder Copilot-licentie, autonome agents)
- Maak vooraf een **kostenschatting**
- Check altijd de actuele licentiegids

**Visual:** Eenvoudige weergave: licentie vs. verbruik.

**Sprekernotities**
- Wees eerlijk: licentiemodellen veranderen vaak. "Ik geef de richting, controleer de details bij uitrol."
- Hoe vaker de agent gebruikt wordt en hoe meer stappen en acties hij uitvoert, hoe hoger het verbruik.
- Adviseer: begin met een pilot, meet verbruik en tevredenheid, en schaal daarna.

**Tijd:** 3 min

---

## Slide 26: Mini-casus

**Op de slide**
> Een collega bouwt een agent die klantvragen beantwoordt en publiceert hem op de website. Na een week noemt hij een korting die niet bestaat.
>
> **Welke van de vijf beheervragen waren niet beantwoord?**

**Visual:** Alleen de casustekst.

**Sprekernotities**
- Laat 2 minuten in tweetallen bespreken, daarna plenair.
- Verwacht: eigenaar, bronnen en grenzen, acties en levenscyclus. Extra punt: externe publicatie vraagt een zwaardere review dan interne.
- Sluit het blok af met: "Zonder beheer is een agent geen hulpmiddel maar een risico."

**Tijd:** 3 min

---

# AFSLUITING (2:20 – 2:30)

## Slide 27: Opdracht 4: Mijn use case

**Op de slide**
- Proces, wie heeft er last van, hoe vaak
- Bronnen
- Antwoorden of handelingen?
- Type: Chat / Agent Builder / Studio / Geen AI
- Ergste dat er fout kan gaan
- Eigenaar, eerste stap binnen 2 weken

**Visual:** Het use case-kader uit het werkboek.

**Sprekernotities**
- 5 minuten individueel werken in het werkboek.
- Daarna een snel deelrondje: iedereen noemt in één zin zijn use case en eerste stap.
- Haal de **use case-parkeerplaats** van het begin erbij en vergelijk.
- Benoem trends: welke keuze komt het vaakst terug?

**Tijd:** 8 min

---

## Slide 28: Hoe nu verder?

**Op de slide**
- **Vandaag:** werkboek en spiekbrief bewaren
- **Na 2 weken:** reminder "Wat is je eerste agent geworden?"
- **Na 4 weken:** spreekuur (45 min)
- **Na 30/60/90 dagen:** meten en bijsturen
- Bouw een **champions-netwerk**

**Visual:** Tijdlijn 0 → 90 dagen.

**Sprekernotities**
- Zeg: "Een workshop verandert weinig als er daarna niets gebeurt."
- Vraag wie champion wil zijn: iemand die collega's op weg helpt.
- Noem mogelijke KPI's: aantal actieve agents, gebruikers per agent, geschatte tijdwinst, aantal agents met eigenaar en reviewdatum.

**Tijd:** 2 min (inclusief evaluatie hieronder)

---

## Slide 29: Evaluatie en afsluiting

**Op de slide**
- Vul de evaluatie in het werkboek in (4 stellingen + 1 open vraag)
- Dank voor jullie inzet
- Contact: [naam, e-mail, telefoon]

**Visual:** QR-code naar evaluatie of contactgegevens.

**Sprekernotities**
- Vraag deelnemers de evaluatie in te vullen vóór ze weggaan (2 minuten).
- Sluit af: "Begin klein, test lastig, wijs een eigenaar aan."
- Bedank de groep en geef aan dat de materialen worden nagestuurd.

**Tijd:** 2 min

---

# BIJLAGE: Tijdschema in één oogopslag

| Slide | Onderwerp | Min. | Totaal |
|---|---|---|---|
| 1–3 | Opening en check-in | 10 | 0:10 |
| 4–7 | Module 1: Wat zijn agents? | 20 | 0:30 |
| 8–12 | Module 2: Wanneer wel, wanneer niet? | 15 | 0:45 |
| 13–16 | Module 3: Agent Builder | 30 | 1:15 |
| 17 | Pauze | 10 | 1:25 |
| 18–22 | Module 4: Copilot Studio | 40 | 2:05 |
| 23–26 | Module 5: Beheer, risico's en kosten | 15 | 2:20 |
| 27–29 | Afsluiting | 10 | 2:30 |

# BIJLAGE: Bijsturen tijdens de sessie

- **Loopt Module 3 uit?** Sla de extra uitdaging over en verkort de reflectie.
- **Connector loopt vast (slide 21)?** Laat deelnemers het onderwerp afmaken met alleen berichten en toon de lijstkoppeling als demo.
- **Geen Copilot Studio-rechten?** Doe Module 4 als trainersdemo (25 min) en laat deelnemers het Meldpunt op papier ontwerpen.
- **Groep ervaren?** Voeg een tweede kennisbron of een mail-actie toe.
- **Meer tijd?** Voeg een module over autonome agents en governance in het admin center toe.

---

*Versie 1.0. Controleer menunamen, licentiemodel en functies vóór de sessie.*
