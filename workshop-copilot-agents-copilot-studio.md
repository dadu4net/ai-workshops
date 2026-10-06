# Workshop: Copilot Agents & Copilot Studio

**Duur:** 2,5 uur (150 minuten, inclusief 10 minuten pauze)
**Doelgroep:** Key-users, teamleiders, afdelingsbeheerders en informatiemanagers die Microsoft Copilot al gebruiken en zelf agents willen bouwen of beoordelen
**Niveau:** Gevorderd beginner (kent Copilot Chat/prompten, geen programmeerervaring nodig)
**Groepsgrootte:** 6 tot 14 deelnemers (hands-on, laptop verplicht)
**Vorm:** Demo, doe-mee, zelfstandig oefenen, reflectie

---

## 0. Trainersnotitie: actualiteitscheck (doe dit 2 dagen vooraf)

Copilot verandert snel van naam, interface en licentiemodel. Controleer vooraf:

- [ ] **Naamgeving:** Microsoft 365 Copilot wordt in recente documentatie "Microsoft Copilot" genoemd. Gebruik in de sessie de term die deelnemers in hun eigen omgeving zien.
- [ ] **Licenties:** Agent Builder zit in de Copilot-licentie. Voor Copilot Studio gelden verbruiksgebaseerde **Copilot Credits** wanneer je agent extern publiceert, gebruikers zonder Copilot-licentie bedient of autonoom draait. Controleer de actuele Microsoft-licentiegids voor jouw klant.
- [ ] **Interface:** Menunamen en tabs (Configure, Knowledge, Tools, Topics) verschuiven regelmatig. Doe de opdrachten zelf nog eens door in de testomgeving.
- [ ] **Beheer:** Controleer in het M365 admin center en Power Platform admin center of deelnemers agents mogen maken, delen en publiceren.
- [ ] **Nieuwe functies:** Kijk in de Copilot Studio release notes naar nieuwe knowledge-bronnen, MCP-ondersteuning en autonome triggers.

---

## 1. Voorbereiding

### Technisch (trainer)
- Testtenant of demo-omgeving met **Copilot-licenties voor alle deelnemers**
- Toegang tot **Copilot Studio** (maker-rechten) voor alle deelnemers
- Een **SharePoint-site "Workshop Agents"** met voorbeeldcontent:
  - `Personeelshandboek.docx` (verlof, ziekmelding, thuiswerken)
  - `Onboarding-checklist.docx`
  - `FAQ-Facilitair.docx` (printers, parkeren, werkplekken, bestellen)
  - Een **SharePointlijst "Facilitaire meldingen"** met kolommen: Titel, Locatie, Omschrijving, Urgentie (Keuze: Laag/Normaal/Hoog), Gemeld door
- Beamer/scherm, flipover, stickers of Teams-whiteboard voor Opdracht 1

### Voor deelnemers (stuur 3 dagen vooraf)
- Check dat je kunt inloggen op `m365.cloud.microsoft` en `copilotstudio.microsoft.com`
- Bedenk **1 terugkerend vraag- of afhandelingsproces** in je team dat je graag slimmer zou maken
- Laptop meenemen (geen alleen tablet of telefoon)

---

## 2. Leeruitkomsten

Na afloop van deze workshop kan de deelnemer:

1. **Uitleggen** wat een Copilot agent is en welke soorten er zijn (Bloom: begrijpen)
2. **Onderscheiden** wanneer een agent, Agent Builder, Copilot Studio of juist geen agent de juiste keuze is (analyseren/evalueren)
3. **Aanmaken** van een eenvoudige kennisagent in Agent Builder met goede instructies en gecontroleerde kennisbronnen (toepassen)
4. **Bouwen** van een agent in Copilot Studio met kennisbron, topic en actie (tool), en deze **testen** (toepassen/creëren)
5. **Benoemen** van de belangrijkste risico's, beheerafspraken en kostenaspecten rondom agents (onthouden/begrijpen)
6. **Opstellen** van een eigen use case-voorstel voor de eigen afdeling (creëren)

---

## 3. Programmaoverzicht

| Tijd | Min. | Blok | Werkvorm |
|---|---|---|---|
| 0:00 – 0:10 | 10 | Welkom, doelen, check-in | Plenair |
| 0:10 – 0:30 | 20 | **Module 1:** Wat zijn agents? | Uitleg + live demo |
| 0:30 – 0:45 | 15 | **Module 2:** Wanneer wel, wanneer niet? | Uitleg + sorteeropdracht |
| 0:45 – 1:15 | 30 | **Module 3:** Agent Builder (hands-on) | Doe-mee + zelfstandig |
| 1:15 – 1:25 | 10 | **Pauze** | |
| 1:25 – 2:05 | 40 | **Module 4:** Copilot Studio (hands-on) | Doe-mee + zelfstandig |
| 2:05 – 2:20 | 15 | **Module 5:** Beheer, risico's en kosten | Uitleg + casediscussie |
| 2:20 – 2:30 | 10 | Afsluiting, actieplan, evaluatie | Individueel + plenair |

---

## 4. Draaiboek per blok

### Blok 0: Welkom en check-in (10 min)

**Doel:** Verwachtingen afstemmen en het startniveau peilen.

**Trainer:**
1. Heet welkom, loop kort de agenda en leeruitkomsten door.
2. Stel drie snelle handopsteek-vragen:
   - Wie heeft al eens een eigen agent gemaakt?
   - Wie gebruikt dagelijks Copilot?
   - Wie maakt zich zorgen over controle of veiligheid van agents?
3. Laat elke deelnemer in één zin zeggen welk proces ze hopen te verbeteren (schrijf op flipover: dit is de **"use case-parkeerplaats"**).

---

### Module 1: Wat zijn agents? (20 min)

**Kernboodschap:** *Een agent is Copilot met een eigen opdracht, eigen kennis en (optioneel) eigen handelingen.*

#### 1.1 Van Copilot naar agent (5 min)

| | Copilot Chat / Copilot | Agent |
|---|---|---|
| Gedrag | Algemeen, beantwoordt elke vraag | Specifiek, vaste rol en taak |
| Kennis | Jouw werkdata + web | Alleen de bronnen die jij kiest |
| Instructies | Steeds opnieuw prompten | Eenmalig vastgelegd |
| Handelingen | Vooral tekst en samenvattingen | Kan acties uitvoeren (mail, lijst, flow) |
| Delen | Persoonlijk | Deelbaar met team of organisatie |

**Analogie voor deelnemers:** Copilot is een slimme stagiair die alles een beetje kan. Een agent is diezelfde stagiair met een functieomschrijving, een eigen map met documenten en een paar vaste taken.

#### 1.2 De vier bouwstenen (5 min)

1. **Instructies:** rol, toon, grenzen, wat de agent wel en niet doet
2. **Kennis:** SharePoint, OneDrive, websites, bestanden, Dataverse, enz.
3. **Tools/acties:** connectors, Power Automate-flows, API's, MCP
4. **Triggers en kanalen:** waar en wanneer de agent werkt (Teams, Copilot, website, of automatisch bij een gebeurtenis)

#### 1.3 De drie soorten agents (5 min)

| Soort | Waar | Wie bouwt | Voorbeeld |
|---|---|---|---|
| **Kennisagent via Agent Builder** | In Copilot | Elke Copilot-gebruiker | "Vraag het HR" op basis van het personeelshandboek |
| **Copilot Studio-agent** | Copilot Studio | Maker / key-user / IT | Meldpunt Facilitair dat een melding aanmaakt in een lijst |
| **Autonome agent** | Copilot Studio | Maker / IT | Agent die bij elke nieuwe factuurmail zelf checkt en doorzet |

Noem ook kort de kant-en-klare agents (bijv. Researcher, Analyst) als "agents die Microsoft al voor je gebouwd heeft".

#### 1.4 Live demo (5 min)

Toon een **kant-en-klare agent** (bijv. de HR-agent op de workshopsite) en stel er drie vragen aan:
1. Een vraag waar het antwoord in de bron staat → agent antwoordt met verwijzing
2. Een vraag buiten de bron → agent hoort te weigeren of aan te geven dat hij het niet weet
3. Een vraag waarbij de bron tegenstrijdig is → bespreek met de groep hoe de agent omgaat met slechte brondata

> **Vraag aan de groep:** "Wat zegt dit over de kwaliteit van de bron die je aan een agent geeft?"
> **Leerpunt:** *Een agent is zo goed als zijn bron en zijn instructies.*

---

### Module 2: Wanneer wel, wanneer niet? (15 min)

**Kernboodschap:** *Niet elk probleem is een agent-probleem.*

#### 2.1 Wanneer wél een agent (5 min)

Een agent is een goede keuze als:
- De **vraag terugkomt** (minstens wekelijks, door meerdere mensen)
- Het antwoord staat in **bestaande, actuele documenten**
- Het **proces een duidelijk begin en einde** heeft
- Een **foutje beperkt risico** heeft of er een mens meekijkt
- Je **tijd wint** (denk aan 10+ minuten per keer, of veel mensen met dezelfde vraag)

**Voorbeelden uit de praktijk:**

| Use case | Type | Waarom het werkt |
|---|---|---|
| Vraagbaak personeelsbeleid (verlof, declaraties) | Agent Builder | Vaste bron, veel herhaalvragen |
| Onboarding-buddy voor nieuwe collega's | Agent Builder | Checklist + handboek, veel basisvragen |
| Facilitair meldpunt met automatische melding | Copilot Studio | Vragen beantwoorden én actie uitvoeren |
| Offerte-assistent op basis van standaardteksten | Agent Builder | Hergebruik van goedgekeurde teksten |
| IT-servicedesk eerste lijn (wachtwoord, VPN) | Copilot Studio | Standaardvragen, doorverwijzing naar mens |
| Projectstatus-agent over een Teams-kanaal | Agent Builder | Samenvatten van gedeelde content |
| Automatische triage van inkomende klantmails | Autonome agent | Vaste regels, hoog volume, mens beslist bij uitzondering |

#### 2.2 Wanneer NIET (5 min)

Een agent is **geen goede keuze** als:

| Situatie | Waarom niet | Beter alternatief |
|---|---|---|
| De bron is **verouderd, rommelig of tegenstrijdig** | Agent geeft foute antwoorden met stellige toon | Eerst opschonen (content-governance) |
| Het gaat om **eenmalige of unieke taken** | Bouwtijd is groter dan opbrengst | Gewoon Copilot Chat met een goede prompt |
| Het proces is **volledig vaststaand, zonder taal of interpretatie** | Geen AI nodig | Power Automate-flow of formulier |
| Er zijn **hoge risico's bij een fout** (juridisch, medisch, HR-besluiten, financiële goedkeuring) | Fouten zijn niet acceptabel | Mens beslist; AI hooguit voorbereiden |
| **Gevoelige data** waarvoor rechten niet op orde zijn | Agent kan data tonen aan wie het niet mag zien | Eerst rechten en labels fixen |
| Niemand **eigenaar** wil zijn van de agent | Agent verwaait, antwoorden raken achterhaald | Eerst eigenaarschap regelen |
| Je wilt **zwaar maatwerk met veel koppelingen** zonder beheer | Wordt een schaduw-IT-oplossing | Samen met IT of partner ontwerpen |

#### 2.3 Beslisboom (zet op flipover)

```
Komt de vraag/taak vaak terug?
├── Nee → Gebruik gewoon Copilot Chat
└── Ja → Staat het antwoord in bestaande, actuele documenten?
          ├── Nee → Eerst content op orde brengen
          └── Ja → Moet de agent ook iets DOEN (aanmaken, versturen, wijzigen)?
                    ├── Nee → Agent Builder (kennisagent)
                    └── Ja → Is het een vast stappenplan zonder taalbegrip?
                              ├── Ja → Power Automate
                              └── Nee → Copilot Studio
```

**Extra toets:** *Wat is het ergste dat er kan gebeuren als de agent het fout doet?* Is dat acceptabel, of kan een mens het controleren? Zo niet, dan geen agent (of mens in de loop).

#### 2.4 Opdracht 1: Agent of niet? (5 min, in tweetallen)

Je krijgt 6 situaties. Plak elk op de juiste plek: **Copilot Chat / Agent Builder / Copilot Studio / Power Automate / Geen AI**.

| # | Situatie | Verwacht antwoord |
|---|---|---|
| 1 | Elke maandag vragen collega's hoeveel verlofdagen ze hebben volgens het handboek | Agent Builder |
| 2 | Je wilt eenmalig een samenvatting van een 40-pagina's rapport | Copilot Chat |
| 3 | Bij elke nieuwe leverancier moet een vast formulier ingevuld en doorgestuurd worden | Power Automate |
| 4 | Collega's melden een kapotte printer; er moet automatisch een melding in een lijst komen met bevestiging | Copilot Studio |
| 5 | Een agent moet bepalen of een medewerker recht heeft op een bonus | Geen AI (mens beslist) |
| 6 | Een agent moet de eerste lijn van het IT-meldpunt afhandelen en doorsturen naar de servicedesk | Copilot Studio |

**Nabespreking (laatste minuut):** Bij welke situatie waren jullie het oneens? Waarom? Bespreek dat er vaak meerdere antwoorden verdedigbaar zijn; het gaat om de redenering.

---

### Module 3: Agent Builder, je eerste agent (30 min)

**Kernboodschap:** *In 15 minuten een werkende kennisagent; de kwaliteit zit in je instructies en bronnen.*

#### 3.1 Uitleg (5 min)

Bespreek de anatomie van goede **instructies**. Gebruik dit sjabloon (zet het in de chat of op een slide):

```
ROL:        Je bent [functie/rol] van [organisatie/team].
DOEL:       Je helpt [doelgroep] met [taak].
BRONNEN:    Gebruik uitsluitend de gekoppelde kennisbronnen.
TOON:       Schrijf [helder, vriendelijk, formeel/informeel], in het Nederlands.
GRENZEN:    Als het antwoord niet in de bronnen staat, zeg dat eerlijk en
            verwijs naar [persoon/afdeling]. Verzin nooit een antwoord.
FORMAAT:    Antwoord kort (max. [x] zinnen), met een verwijzing naar de bron.
```

**Veelgemaakte fouten:**
- Te vage instructies ("Wees behulpzaam")
- Te veel bronnen ("de hele SharePoint-omgeving")
- Geen grens voor wat de agent níét mag doen
- Nooit testen met lastige vragen

#### 3.2 Opdracht 2: Bouw de "Vraag het HR"-agent (20 min)

**Scenario:** Medewerkers stellen steeds dezelfde vragen over verlof, ziekmelding en thuiswerken. Jij bouwt een agent die deze vragen beantwoordt op basis van het personeelshandboek.

**Doe-mee-stappen (trainer demonstreert, deelnemers doen mee):**

1. Open Microsoft Copilot (`m365.cloud.microsoft`) en ga naar **Agents**
2. Kies **Agent maken** (New agent / Create agent)
3. Kies voor de **Configureren**-weergave (in plaats van het gesprek) zodat je alles zelf invult
4. Vul in:
   - **Naam:** `Vraag het HR`
   - **Beschrijving:** `Beantwoordt vragen over verlof, ziekmelding en thuiswerken`
   - **Instructies:** gebruik het sjabloon uit 3.1 en pas het aan (rol, toon, grenzen)
5. Voeg bij **Kennis** de SharePoint-bron toe: kies uitsluitend het bestand `Personeelshandboek.docx` (niet de hele site)
6. Voeg 3 **startprompts** toe, bijvoorbeeld:
   - "Hoeveel verlofdagen heb ik?"
   - "Wat moet ik doen als ik ziek ben?"
   - "Mag ik thuiswerken?"
7. **Test** de agent in het voorbeeldvenster rechts (zie hieronder)
8. Klik op **Maken** en deel de agent niet; houd hem in deze fase persoonlijk

**Testscript (verplicht!):**

| Testvraag | Verwacht gedrag |
|---|---|
| "Hoeveel verlofdagen heb ik?" | Antwoord uit het handboek met bronverwijzing |
| "Wat is de hoofdstad van Frankrijk?" | Agent weigert beleefd (buiten scope) |
| "Mijn collega verdient meer dan ik, wat is zijn salaris?" | Agent weigert / verwijst naar HR |
| "Wat staat er in het handboek over bedrijfsauto's?" | Eerlijk: staat er niet in, verwijst naar HR |

**Als de agent onverwacht antwoordt:** scherp de instructies aan (zet de grens expliciet erin) en test opnieuw. Dit **verbeterloopje** is het belangrijkste leerpunt van deze opdracht.

#### 3.3 Reflectie (5 min)

In tweetallen: *Welke instructie had het grootste effect op de kwaliteit? Welke bron zou je nooit koppelen?*

**Extra uitdaging (voor snelle deelnemers):** Voeg een tweede bron toe (`Onboarding-checklist.docx`) en kijk wat er met de antwoorden gebeurt. Wordt de agent beter of juist slechter?

---

### Pauze (10 min)

---

### Module 4: Copilot Studio, een agent die iets doet (40 min)

**Kernboodschap:** *Copilot Studio is nodig als de agent moet handelen, vaste gesprekken moet voeren of buiten Copilot moet werken.*

#### 4.1 Uitleg en verkenning (8 min)

Laat de omgeving zien (`copilotstudio.microsoft.com`):

| Onderdeel | Wat doet het | Analogie |
|---|---|---|
| **Overzicht** | Naam, beschrijving, instructies | Functieomschrijving |
| **Kennis** | Bronnen van de agent | Naslagwerken |
| **Tools** | Acties: flows, connectors, API's | Handen van de agent |
| **Onderwerpen (Topics)** | Vaste gesprekken met vragen en vertakkingen | Draaiboek / script |
| **Testen** | Ruimte om gesprekken te testen | Proefrit |
| **Publiceren / Kanalen** | Teams, Copilot, website, enz. | Waar de agent beschikbaar is |
| **Analyse** | Gebruik en tevredenheid | Rapportage |

**Wanneer Copilot Studio in plaats van Agent Builder?**

| Behoefte | Agent Builder | Copilot Studio |
|---|---|---|
| Vragen beantwoorden uit M365-content | Ja | Ja |
| Een handeling uitvoeren (lijst, mail, flow) | Beperkt | Ja |
| Vaste gesprekken met vragen aan de gebruiker | Nee | Ja (topics) |
| Koppelen aan externe systemen/API's | Beperkt | Ja (connectors, MCP) |
| Publiceren op website of externe kanalen | Nee | Ja |
| Autonoom starten bij een gebeurtenis | Nee | Ja |
| Uitgebreide governance en analyse | Beperkt | Ja |
| Bouwtijd | Minuten | Uren tot dagen |

#### 4.2 Opdracht 3: Bouw de "Meldpunt Facilitair"-agent (30 min)

**Scenario:** Collega's melden storingen (printer, verlichting, koffieapparaat) via mail of de gang. Jij bouwt een agent die:
1. Veelgestelde vragen beantwoordt (kennis)
2. Een **melding aanmaakt** in de SharePointlijst "Facilitaire meldingen" (actie)
3. Beschikbaar is in **Teams**

**Stap 1: Agent aanmaken (3 min)**
1. Open Copilot Studio en kies **Agent maken**
2. Naam: `Meldpunt Facilitair`
3. Instructies (kopieer en pas aan):
   ```
   Je bent het facilitaire meldpunt. Je beantwoordt vragen over printers,
   parkeren en werkplekken op basis van de FAQ. Als iemand een storing of
   probleem wil melden, verzamel je locatie, omschrijving en urgentie en
   maak je een melding aan. Bevestig daarna kort wat je hebt vastgelegd.
   Verzin geen antwoorden; verwijs bij twijfel naar facilitair@jouwbedrijf.nl.
   ```

**Stap 2: Kennis toevoegen (4 min)**
1. Ga naar **Kennis** → **Kennis toevoegen**
2. Kies **SharePoint** en selecteer `FAQ-Facilitair.docx`
3. Wacht tot de status op **Gereed** staat

**Stap 3: Eerste test (3 min)**
1. Open het **Testvenster**
2. Vraag: "Waar kan ik parkeren als de parkeerplaats vol is?" → controleer dat het antwoord uit de FAQ komt

**Stap 4: Onderwerp "Storing melden" maken (8 min)**
1. Ga naar **Onderwerpen** → **Onderwerp toevoegen** → **Vanaf nul**
2. Naam: `Storing melden`
3. Triggerzinnen (voeg 5 toe): "Ik wil een storing melden", "De printer is kapot", "Er is iets stuk", "Ik wil iets melden", "Lamp doet het niet"
4. Voeg drie **Vraag**-knooppunten toe:
   - Vraag 1: "Waar is de storing?" → sla op als variabele `Locatie` (type: Tekst)
   - Vraag 2: "Wat is er precies aan de hand?" → variabele `Omschrijving` (type: Tekst)
   - Vraag 3: "Hoe urgent is het?" → variabele `Urgentie` (type: Meerkeuze: Laag, Normaal, Hoog)

**Stap 5: Actie toevoegen, melding aanmaken (8 min)**
1. Voeg onder de vragen een **Actie aanroepen** / **Tool toevoegen** knooppunt toe
2. Kies de connector **SharePoint → Item maken**
3. Vul in:
   - **Site:** Workshop Agents
   - **Lijst:** Facilitaire meldingen
   - **Titel:** `Locatie`
   - **Omschrijving:** `Omschrijving`
   - **Urgentie:** `Urgentie`
4. Voeg een **Bericht** toe: "Bedankt, je melding is vastgelegd. Urgentie: {Urgentie}."
5. **Sla het onderwerp op**

*Tip voor de trainer: de connector vraagt mogelijk om een verbinding te maken. Laat deelnemers inloggen als daarom gevraagd wordt en bespreek kort dat dit een **verbinding met eigen rechten** is.*

**Stap 6: Testen en publiceren (5 min)**
1. Test in het testvenster: "De printer op de eerste verdieping is kapot, het is urgent"
2. Controleer in de SharePointlijst dat er een **nieuw item** staat
3. Ga naar **Publiceren** en kies **Publiceren**
4. Ga naar **Kanalen** → **Teams en Microsoft 365 Copilot** → **Agent beschikbaar maken** (houd het in de workshop op "alleen ik")

**Testscript:**

| Testvraag | Verwacht gedrag |
|---|---|
| "Waar kan ik parkeren?" | Antwoord uit FAQ |
| "De lamp in vergaderzaal 2 doet het niet" | Topic "Storing melden" start, vraagt urgentie |
| "Wat is het wifi-wachtwoord van de directie?" | Agent weigert / verwijst door |
| "Verwijder alle meldingen" | Agent kan dat niet (geen tool daarvoor) |

**Extra uitdaging:** Laat de agent na het aanmaken ook een **mail sturen** naar facilitair of een **Teams-bericht** plaatsen. Welke extra risico's brengt dit mee?

#### 4.3 Reflectie (2 min)

*Welke stap vond je het moeilijkst? Wat zou je nodig hebben om dit in je eigen team te bouwen?*

---

### Module 5: Beheer, risico's en kosten (15 min)

**Kernboodschap:** *Bouwen is makkelijk. Beheren is waar het werk zit.*

#### 5.1 Vijf beheervragen (5 min)

Neem deze vragen mee voor élke agent:

1. **Eigenaar:** Wie is verantwoordelijk als de agent fout antwoordt of niet meer klopt?
2. **Bronnen:** Wie houdt de gekoppelde documenten actueel?
3. **Rechten:** Wie mag de agent gebruiken, bewerken en delen? Wat kan de agent zien namens de gebruiker?
4. **Acties:** Welke handelingen mag de agent uitvoeren, en wie controleert dat?
5. **Levenscyclus:** Wanneer evalueren we of de agent nog nodig is, en wanneer ruimen we hem op?

#### 5.2 Risico's en maatregelen (5 min)

| Risico | Voorbeeld | Maatregel |
|---|---|---|
| Verkeerde antwoorden | Agent citeert oud beleid | Beperk bronnen, eigenaar, reviewmoment |
| Oversharing | Agent toont data uit map waar rechten te ruim staan | Rechten en labels eerst op orde |
| Ongewenste acties | Agent verstuurt mail of wijzigt data | Minimale rechten, bevestiging vóór actie |
| Agent-wildgroei | 80 half verlaten agents | Agentregister, naamgeving, opschoonbeleid |
| Kosten lopen op | Veel gebruik van een extern gepubliceerde agent | Verbruik monitoren, budget afspreken |
| Schaduw-IT | Teams bouwen op eigen houtje koppelingen | Maker-beleid, omgevingen, DLP-beleid |

#### 5.3 Kosten in vogelvlucht (3 min)

- **Agent Builder:** zit in de Copilot-licentie (per gebruiker)
- **Copilot Studio:** gebruik wordt gemeten in **Copilot Credits** (verbruik). Relevant bij externe publicatie, gebruikers zonder Copilot-licentie of autonome agents
- **Houd rekening met:** hoe vaak de agent gebruikt wordt, hoeveel stappen en acties hij uitvoert
- Laat altijd een **kostenschatting maken** vóór uitrol. Check de actuele licentiegids voor de exacte regels

#### 5.4 Mini-casus (2 min, plenair)

> *Een collega bouwt een agent die klantvragen beantwoordt en publiceert hem op de website. Na een week blijkt dat hij een korting noemt die niet bestaat. Welke van de vijf beheervragen waren niet beantwoord?*

(Verwacht: eigenaar, bronnen/grenzen, acties en levenscyclus. Bespreek ook dat externe publicatie extra review vraagt.)

---

### Afsluiting (10 min)

#### Opdracht 4: Mijn use case-voorstel (5 min, individueel)

Vul dit kader in voor één echte situatie in je eigen werk:

```
USE CASE-VOORSTEL
-----------------
Proces/vraag:             ______________________________
Wie heeft er last van:    ______________________________
Hoe vaak per week:        ______________________________
Bron(nen) waar het antwoord staat: ______________________
Alleen antwoorden, of ook handelingen?  ☐ Antwoorden  ☐ Handelingen
Type:                     ☐ Copilot Chat  ☐ Agent Builder  ☐ Copilot Studio  ☐ Geen AI
Wat is het ergste dat er fout kan gaan?  ________________
Wie wordt eigenaar:       ______________________________
Eerste stap (binnen 2 weken): ___________________________
```

#### Deelrondje (3 min)

Elke deelnemer noemt in één zin zijn use case en eerste stap. Vergelijk met de "use case-parkeerplaats" van het begin.

#### Evaluatie (2 min)

Korte enquête (Kirkpatrick niveau 1), 4 vragen op schaal 1 tot 5:
1. De workshop was relevant voor mijn werk
2. Ik weet nu wanneer ik wel en niet een agent inzet
3. Ik durf zelf een eenvoudige agent te bouwen
4. Het tempo was passend

Plus één open vraag: *Wat zou je anders willen zien?*

---

## 5. Naslag voor deelnemers: spiekbrief

### Agent of niet: snelle check
- [ ] Komt de vraag vaak terug?
- [ ] Staat het antwoord in actuele documenten?
- [ ] Is een fout acceptabel of controleerbaar?
- [ ] Is er een eigenaar?
- [ ] Zijn rechten op de bron op orde?

### Instructiesjabloon
```
ROL / DOEL / BRONNEN / TOON / GRENZEN / FORMAAT
```

### Kies je tool
| Ik wil... | Gebruik |
|---|---|
| Eenmalig iets laten schrijven of samenvatten | Copilot Chat |
| Vragen laten beantwoorden uit mijn documenten | Agent Builder |
| Een agent die ook handelingen uitvoert of gesprekken voert | Copilot Studio |
| Een vast proces zonder taalbegrip | Power Automate |

### Testen: altijd vier soorten vragen
1. Vraag die in de bron staat
2. Vraag buiten het onderwerp
3. Vraag die niet in de bron staat
4. Vraag waarmee iemand de agent probeert te misleiden

---

## 6. Transfer en vervolg (adoptie)

Een workshop alleen verandert weinig. Plan daarom:

| Moment | Actie |
|---|---|
| **Direct na afloop** | Stuur deze spiekbrief + de ingevulde use case-voorstellen terug naar deelnemers |
| **Na 2 weken** | Reminder-mail: "Wat is je eerste agent geworden?" + link naar naslag |
| **Na 4 weken** | Optionele **spreekuur-sessie** (45 min) voor vragen en demo's van gebouwde agents |
| **Na 30 / 60 / 90 dagen** | Meet het aantal gebouwde agents, gebruik en tevredenheid (Kirkpatrick niveau 3) |
| **Doorlopend** | Bouw een **champions-netwerk** van deelnemers die collega's helpen |

**Mogelijke KPI's:** aantal actieve agents, aantal gebruikers per agent, bespaarde tijd (schatting door eigenaar), aantal agents met benoemde eigenaar en reviewdatum.

---

## 7. Toetsvragen (optioneel, formatief)

1. **Begrijpen:** Wat is het verschil tussen een gewone Copilot-vraag en een vraag aan een agent?
2. **Onderscheiden:** Je wilt dat een agent bij een melding automatisch een item in een lijst aanmaakt. Agent Builder of Copilot Studio? Waarom?
3. **Evalueren:** Noem twee situaties waarin je geen agent zou bouwen en wat je dan wel doet.
4. **Toepassen:** Schrijf in drie zinnen de instructies voor een agent die vragen over declaraties beantwoordt.
5. **Analyseren:** Een agent geeft een verouderd antwoord. Noem twee mogelijke oorzaken en een maatregel per oorzaak.

---

## 8. Tijdsbuffers en alternatieven voor de trainer

- **Loopt Module 3 uit?** Sla de extra uitdaging over en verkort de reflectie naar 2 minuten.
- **Loopt de SharePoint-connector vast in Module 4?** Laat deelnemers de stappen 4.2 t/m 4.4 afmaken met alleen berichten, en toon de koppeling met de lijst als demo.
- **Geen Copilot Studio-rechten voor deelnemers?** Vervang Module 4 door een **trainersdemo** van 25 minuten plus Opdracht 3 als individuele "ontwerp op papier"-opdracht (topic, vragen, actie).
- **Groep ervaren?** Voeg in Module 4 een **tweede kennisbron** toe, of laat de agent een **mail** versturen met bevestiging.
- **Meer tijd (halve dag)?** Voeg een module toe over **autonome agents (triggers)** en **governance in het admin center**.

---

*Versie 1.0. Controleer menunamen, licentiemodel en functies altijd vóór de sessie in de actuele Microsoft-documentatie.*
