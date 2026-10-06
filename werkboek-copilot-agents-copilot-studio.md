# Deelnemerswerkboek: Copilot Agents & Copilot Studio

**Naam:** ______________________________  **Datum:** ________________

**Duur:** 2,5 uur | **Vorm:** uitleg, doe-mee en zelf oefenen

> Dit werkboek is van jou. Schrijf erin, vink af en neem het mee naar je werkplek. Je gebruikt het tijdens de workshop én erna als naslag.

---

## 1. Hoe werk je met dit werkboek?

- **☐ Afvinkvakjes** zijn stappen die je tijdens de opdrachten afloopt.
- **Invulvelden** (`______`) zijn voor je eigen antwoorden en notities.
- **Testlogs** zijn tabellen waarin je noteert wat de agent antwoordt. Dit is het belangrijkste leermoment.
- **Tip:** menunamen in Copilot en Copilot Studio veranderen soms. Zie je een andere naam dan hier? Zoek de knop met dezelfde functie of vraag het de trainer.

---

## 2. Programma

| Tijd | Blok |
|---|---|
| 0:00 – 0:10 | Welkom en check-in |
| 0:10 – 0:30 | **Module 1:** Wat zijn agents? |
| 0:30 – 0:45 | **Module 2:** Wanneer wel, wanneer niet? (Opdracht 1) |
| 0:45 – 1:15 | **Module 3:** Agent Builder (Opdracht 2) |
| 1:15 – 1:25 | Pauze |
| 1:25 – 2:05 | **Module 4:** Copilot Studio (Opdracht 3) |
| 2:05 – 2:20 | **Module 5:** Beheer, risico's en kosten |
| 2:20 – 2:30 | Afsluiting (Opdracht 4), evaluatie |

## 3. Wat kun je na afloop?

- ☐ Uitleggen wat een Copilot agent is en welke soorten er zijn
- ☐ Bepalen wanneer een agent, Agent Builder, Copilot Studio of juist geen agent past
- ☐ Een kennisagent maken in Agent Builder met goede instructies
- ☐ Een agent bouwen in Copilot Studio met kennis, onderwerp en actie, en die testen
- ☐ De belangrijkste risico's en beheerafspraken benoemen
- ☐ Een eigen use case uitwerken voor je team

## 4. Begrippenlijst

| Begrip | Betekenis |
|---|---|
| **Agent** | Copilot met een eigen rol, eigen kennis en (optioneel) eigen handelingen |
| **Agent Builder** | Eenvoudige bouwomgeving in Copilot voor kennisagents |
| **Copilot Studio** | Uitgebreide bouwomgeving voor agents met gesprekken, acties en publicatie |
| **Instructies** | De opdracht en spelregels van de agent |
| **Kennisbron** | Documenten, sites of data waaruit de agent antwoordt |
| **Tool / actie** | Een handeling die de agent kan uitvoeren (item maken, mail sturen) |
| **Onderwerp (topic)** | Een vast gesprek in Copilot Studio met triggerzinnen en vragen |
| **Triggerzin** | Een zin waarop een onderwerp start |
| **Variabele** | Een antwoord dat de agent onthoudt en later gebruikt |
| **Connector** | Koppeling met een andere app of dienst |
| **Copilot Credits** | Verbruikseenheid voor Copilot Studio-gebruik (controleer actuele regels) |
| **Autonome agent** | Agent die zelf start bij een gebeurtenis, zonder dat iemand iets vraagt |

---

## 5. Module 1: Wat zijn agents?

### Kern in één zin
*Een agent is Copilot met een eigen opdracht, eigen kennis en (optioneel) eigen handelingen.*

### Vier bouwstenen

| Bouwsteen | Vraag die je jezelf stelt |
|---|---|
| Instructies | Welke rol heeft de agent en wat mag hij niet? |
| Kennis | Uit welke bronnen mag hij antwoorden? |
| Tools/acties | Wat moet hij kunnen doen? |
| Triggers en kanalen | Waar en wanneer werkt hij? |

### Drie soorten agents

| Soort | Waar | Voorbeeld |
|---|---|---|
| Kennisagent (Agent Builder) | In Copilot | Vraagbaak personeelsbeleid |
| Copilot Studio-agent | Copilot Studio | Meldpunt dat een melding aanmaakt |
| Autonome agent | Copilot Studio | Agent die zelf inkomende mails verwerkt |

### Notities bij de demo

Wat antwoordde de agent op de drie testvragen?

1. Vraag in de bron: ____________________________________________
2. Vraag buiten de bron: ________________________________________
3. Tegenstrijdige bron: __________________________________________

**Mijn leerpunt:** *Een agent is zo goed als zijn ______ en zijn ______.*

---

## 6. Module 2: Wanneer wel, wanneer niet?

### Wanneer wél een agent

- ☐ De vraag komt vaak terug (minstens wekelijks)
- ☐ Het antwoord staat in actuele documenten
- ☐ Het proces heeft een duidelijk begin en einde
- ☐ Een fout is beperkt of controleerbaar
- ☐ Het scheelt echt tijd

### Wanneer NIET

| Situatie | Beter alternatief |
|---|---|
| Bron is verouderd of tegenstrijdig | Eerst content opschonen |
| Eenmalige of unieke taak | Gewoon Copilot Chat |
| Vast proces zonder taalbegrip | Power Automate of formulier |
| Hoog risico bij een fout | Mens beslist, AI bereidt hooguit voor |
| Rechten op de data zijn niet op orde | Eerst rechten en labels fixen |
| Niemand wil eigenaar zijn | Eerst eigenaarschap regelen |

### Beslisboom

```
Komt de vraag/taak vaak terug?
├── Nee → Gebruik gewoon Copilot Chat
└── Ja → Staat het antwoord in bestaande, actuele documenten?
          ├── Nee → Eerst content op orde brengen
          └── Ja → Moet de agent ook iets DOEN?
                    ├── Nee → Agent Builder
                    └── Ja → Vast stappenplan zonder taalbegrip?
                              ├── Ja → Power Automate
                              └── Nee → Copilot Studio
```

**Extra vraag:** *Wat is het ergste dat er kan gebeuren als de agent het fout doet? Is dat acceptabel of kan een mens het controleren?*

### Opdracht 1: Agent of niet? (5 min, in tweetallen)

Kies per situatie: **Copilot Chat / Agent Builder / Copilot Studio / Power Automate / Geen AI**. Schrijf ook je reden op.

| # | Situatie | Mijn keuze | Waarom |
|---|---|---|---|
| 1 | Elke maandag vragen collega's hoeveel verlofdagen ze hebben volgens het handboek | | |
| 2 | Je wilt eenmalig een samenvatting van een rapport van 40 pagina's | | |
| 3 | Bij elke nieuwe leverancier moet een vast formulier ingevuld en doorgestuurd worden | | |
| 4 | Collega's melden een kapotte printer; er moet automatisch een melding in een lijst komen met bevestiging | | |
| 5 | Een agent moet bepalen of een medewerker recht heeft op een bonus | | |
| 6 | Een agent handelt de eerste lijn van het IT-meldpunt af en stuurt door naar de servicedesk | | |

**Waar waren we het oneens, en wat leerde ik daarvan?**
______________________________________________________________

---

## 7. Module 3: Agent Builder

### Instructiesjabloon

```
ROL:        Je bent [functie/rol] van [organisatie/team].
DOEL:       Je helpt [doelgroep] met [taak].
BRONNEN:    Gebruik uitsluitend de gekoppelde kennisbronnen.
TOON:       Schrijf [helder, vriendelijk, formeel/informeel], in het Nederlands.
GRENZEN:    Als het antwoord niet in de bronnen staat, zeg dat eerlijk en
            verwijs naar [persoon/afdeling]. Verzin nooit een antwoord.
FORMAAT:    Antwoord kort (max. [x] zinnen), met een verwijzing naar de bron.
```

**Veelgemaakte fouten:** vage instructies, te veel bronnen, geen grenzen, niet testen met lastige vragen.

### Opdracht 2: Bouw de agent "Vraag het HR" (20 min)

**Scenario:** Medewerkers stellen steeds dezelfde vragen over verlof, ziekmelding en thuiswerken. Jij bouwt een agent die deze vragen beantwoordt op basis van het personeelshandboek.

**Stappen**

- ☐ 1. Open Microsoft Copilot (`m365.cloud.microsoft`) en ga naar **Agents**
- ☐ 2. Kies **Agent maken**
- ☐ 3. Ga naar de **Configureren**-weergave zodat je alles zelf invult
- ☐ 4. Vul in: **Naam** `Vraag het HR`, **Beschrijving** `Beantwoordt vragen over verlof, ziekmelding en thuiswerken`
- ☐ 5. Schrijf je **instructies** met het sjabloon hierboven (vul hieronder eerst je concept in)
- ☐ 6. Voeg bij **Kennis** alleen `Personeelshandboek.docx` toe (niet de hele site)
- ☐ 7. Voeg 3 **startprompts** toe:
  - "Hoeveel verlofdagen heb ik?"
  - "Wat moet ik doen als ik ziek ben?"
  - "Mag ik thuiswerken?"
- ☐ 8. **Test** de agent (zie testlog)
- ☐ 9. Maak de agent aan en laat hem **persoonlijk** (nog niet delen)

**Mijn instructies (concept):**

```
ROL:
DOEL:
BRONNEN:
TOON:
GRENZEN:
FORMAAT:
```

**Testlog Opdracht 2**

| Testvraag | Verwacht | Wat gebeurde er? | Aangepast? |
|---|---|---|---|
| "Hoeveel verlofdagen heb ik?" | Antwoord uit handboek met bron | | |
| "Wat is de hoofdstad van Frankrijk?" | Agent weigert beleefd | | |
| "Wat verdient mijn collega?" | Agent weigert / verwijst naar HR | | |
| "Wat staat er over bedrijfsauto's?" | Eerlijk: staat er niet in | | |

**Mijn verbeterloopje:** Wat paste ik aan in de instructies, en wat was het effect?
______________________________________________________________

**Extra uitdaging:** voeg `Onboarding-checklist.docx` toe als tweede bron. Werden de antwoorden beter of slechter? ____________________

**Reflectie:** Welke instructie had het grootste effect? ____________ Welke bron zou ik nooit koppelen? ____________

---

## 8. Module 4: Copilot Studio

### Onderdelen van de omgeving

| Onderdeel | Wat doet het |
|---|---|
| Overzicht | Naam, beschrijving, instructies |
| Kennis | Bronnen van de agent |
| Tools | Acties: flows, connectors, API's |
| Onderwerpen | Vaste gesprekken met vragen en vertakkingen |
| Testen | Gesprekken uitproberen |
| Publiceren / Kanalen | Teams, Copilot, website |
| Analyse | Gebruik en tevredenheid |

### Agent Builder of Copilot Studio?

| Behoefte | Agent Builder | Copilot Studio |
|---|---|---|
| Vragen beantwoorden uit M365-content | Ja | Ja |
| Een handeling uitvoeren | Beperkt | Ja |
| Vaste gesprekken met vragen | Nee | Ja |
| Externe systemen koppelen | Beperkt | Ja |
| Publiceren op website | Nee | Ja |
| Autonoom starten | Nee | Ja |
| Bouwtijd | Minuten | Uren tot dagen |

### Opdracht 3: Bouw de agent "Meldpunt Facilitair" (30 min)

**Scenario:** Collega's melden storingen via mail of op de gang. Jij bouwt een agent die (1) veelgestelde vragen beantwoordt, (2) een melding aanmaakt in de SharePointlijst "Facilitaire meldingen" en (3) beschikbaar is in Teams.

**Stap 1: Agent aanmaken (3 min)**
- ☐ Open `copilotstudio.microsoft.com` → **Agent maken**
- ☐ Naam: `Meldpunt Facilitair`
- ☐ Instructies:
  ```
  Je bent het facilitaire meldpunt. Je beantwoordt vragen over printers,
  parkeren en werkplekken op basis van de FAQ. Als iemand een storing of
  probleem wil melden, verzamel je locatie, omschrijving en urgentie en
  maak je een melding aan. Bevestig daarna kort wat je hebt vastgelegd.
  Verzin geen antwoorden; verwijs bij twijfel naar facilitair@jouwbedrijf.nl.
  ```

**Stap 2: Kennis toevoegen (4 min)**
- ☐ **Kennis** → **Kennis toevoegen** → **SharePoint**
- ☐ Kies `FAQ-Facilitair.docx`
- ☐ Wacht tot de status **Gereed** is

**Stap 3: Eerste test (3 min)**
- ☐ Open het **Testvenster** en vraag: "Waar kan ik parkeren als de parkeerplaats vol is?"
- ☐ Komt het antwoord uit de FAQ? ☐ Ja ☐ Nee

**Stap 4: Onderwerp "Storing melden" (8 min)**
- ☐ **Onderwerpen** → **Onderwerp toevoegen** → **Vanaf nul**
- ☐ Naam: `Storing melden`
- ☐ Voeg 5 triggerzinnen toe:
  - "Ik wil een storing melden"
  - "De printer is kapot"
  - "Er is iets stuk"
  - "Ik wil iets melden"
  - "Lamp doet het niet"
- ☐ Voeg drie **Vraag**-knooppunten toe:

| Vraag | Variabele | Type |
|---|---|---|
| "Waar is de storing?" | `Locatie` | Tekst |
| "Wat is er precies aan de hand?" | `Omschrijving` | Tekst |
| "Hoe urgent is het?" | `Urgentie` | Meerkeuze: Laag, Normaal, Hoog |

**Stap 5: Actie toevoegen (8 min)**
- ☐ Voeg onder de vragen een **Tool toevoegen / Actie aanroepen** knooppunt toe
- ☐ Kies connector **SharePoint → Item maken** (log in als daarom wordt gevraagd)
- ☐ Vul in: **Site** Workshop Agents, **Lijst** Facilitaire meldingen, **Titel** `Locatie`, **Omschrijving** `Omschrijving`, **Urgentie** `Urgentie`
- ☐ Voeg een **Bericht** toe: "Bedankt, je melding is vastgelegd. Urgentie: {Urgentie}."
- ☐ **Sla het onderwerp op**

**Stap 6: Testen en publiceren (5 min)**
- ☐ Test: "De printer op de eerste verdieping is kapot, het is urgent"
- ☐ Staat er een **nieuw item** in de SharePointlijst?
- ☐ **Publiceren** → **Kanalen** → **Teams en Microsoft 365 Copilot** (houd het in de workshop op "alleen ik")

**Testlog Opdracht 3**

| Testvraag | Verwacht | Wat gebeurde er? |
|---|---|---|
| "Waar kan ik parkeren?" | Antwoord uit FAQ | |
| "De lamp in vergaderzaal 2 doet het niet" | Onderwerp start, vraagt urgentie | |
| "Wat is het wifi-wachtwoord van de directie?" | Agent weigert / verwijst door | |
| "Verwijder alle meldingen" | Agent kan dat niet | |

**Extra uitdaging:** laat de agent na het aanmaken ook een mail of Teams-bericht sturen. Welk extra risico brengt dat mee? ____________________

**Reflectie:** Welke stap vond ik het moeilijkst? ____________ Wat heb ik nodig om dit in mijn team te bouwen? ____________

---

## 9. Module 5: Beheer, risico's en kosten

### Vijf beheervragen (voor élke agent)

| # | Vraag | Mijn antwoord voor "Meldpunt Facilitair" |
|---|---|---|
| 1 | **Eigenaar:** wie is verantwoordelijk? | |
| 2 | **Bronnen:** wie houdt ze actueel? | |
| 3 | **Rechten:** wie mag gebruiken, bewerken en delen? | |
| 4 | **Acties:** wat mag de agent doen en wie controleert? | |
| 5 | **Levenscyclus:** wanneer evalueren en opruimen we? | |

### Risico's en maatregelen

| Risico | Maatregel |
|---|---|
| Verkeerde antwoorden | Beperkte bronnen, eigenaar, reviewmoment |
| Oversharing (rechten te ruim) | Rechten en labels eerst op orde |
| Ongewenste acties | Minimale rechten, bevestiging vóór actie |
| Agent-wildgroei | Register, naamgeving, opschoonbeleid |
| Kosten lopen op | Verbruik monitoren, budget afspreken |
| Schaduw-IT | Maker-beleid, omgevingen, DLP-beleid |

### Kosten in vogelvlucht

- **Agent Builder:** zit in de Copilot-licentie
- **Copilot Studio:** verbruik wordt gemeten in **Copilot Credits**, relevant bij externe publicatie, gebruikers zonder Copilot-licentie of autonome agents
- Maak altijd een **kostenschatting vóór uitrol** en check de actuele licentiegids

### Mini-casus

*Een collega bouwt een agent die klantvragen beantwoordt en publiceert hem op de website. Na een week noemt hij een korting die niet bestaat. Welke beheervragen waren niet beantwoord?*

Mijn antwoord: ______________________________________________

---

## 10. Opdracht 4: Mijn use case-voorstel

```
USE CASE-VOORSTEL
-----------------
Proces/vraag:             ______________________________
Wie heeft er last van:    ______________________________
Hoe vaak per week:        ______________________________
Bron(nen):                ______________________________
Alleen antwoorden, of ook handelingen?  ☐ Antwoorden  ☐ Handelingen
Type:  ☐ Copilot Chat  ☐ Agent Builder  ☐ Copilot Studio  ☐ Geen AI
Ergste dat er fout kan gaan: ____________________________
Eigenaar:                 ______________________________
Eerste stap (binnen 2 weken): ___________________________
```

## 11. Mijn actieplan

| Wanneer | Wat ga ik doen? | Klaar? |
|---|---|---|
| Binnen 2 weken | | ☐ |
| Binnen 30 dagen | | ☐ |
| Binnen 60 dagen | | ☐ |
| Binnen 90 dagen | | ☐ |

**Wie kan mij helpen (collega, key-user, IT)?** ______________________

---

## 12. Spiekbrief

**Agent of niet? Snelle check**
- ☐ Komt de vraag vaak terug?
- ☐ Staat het antwoord in actuele documenten?
- ☐ Is een fout acceptabel of controleerbaar?
- ☐ Is er een eigenaar?
- ☐ Zijn rechten op de bron op orde?

**Kies je tool**

| Ik wil... | Gebruik |
|---|---|
| Eenmalig iets schrijven of samenvatten | Copilot Chat |
| Vragen laten beantwoorden uit mijn documenten | Agent Builder |
| Een agent die ook handelt of gesprekken voert | Copilot Studio |
| Een vast proces zonder taalbegrip | Power Automate |

**Testen: altijd vier soorten vragen**
1. Vraag die in de bron staat
2. Vraag buiten het onderwerp
3. Vraag die niet in de bron staat
4. Vraag waarmee iemand de agent probeert te misleiden

## 13. Problemen oplossen

| Probleem | Probeer dit |
|---|---|
| Ik zie geen **Agent maken** | Vraag je beheerder of agents maken is toegestaan en of je een Copilot-licentie hebt |
| Agent antwoordt niet uit mijn bron | Controleer of de bron is toegevoegd en de status **Gereed** is; controleer of je zelf toegang hebt tot het bestand |
| Agent verzint antwoorden | Maak de GRENZEN in de instructies expliciet; beperk de bronnen |
| Onderwerp start niet | Voeg meer en gevarieerdere triggerzinnen toe |
| Connector vraagt om verbinding | Log in met je eigen account en bevestig de verbinding |
| Item verschijnt niet in de lijst | Controleer site, lijst en veldkoppelingen; test opnieuw |
| Ik kan niet publiceren | Vraag je beheerder naar de maker- en publicatierechten |

## 14. Zelftoets

1. Wat is het verschil tussen een gewone Copilot-vraag en een vraag aan een agent?
   ______________________________________________________
2. Je wilt dat een agent automatisch een item in een lijst aanmaakt. Agent Builder of Copilot Studio, en waarom?
   ______________________________________________________
3. Noem twee situaties waarin je géén agent bouwt, en wat je dan wel doet.
   ______________________________________________________
4. Schrijf in drie zinnen de instructies voor een agent die vragen over declaraties beantwoordt.
   ______________________________________________________
5. Een agent geeft een verouderd antwoord. Noem twee mogelijke oorzaken en een maatregel per oorzaak.
   ______________________________________________________

## 15. Evaluatie

Schaal 1 (niet mee eens) tot 5 (helemaal mee eens):

| Stelling | 1 | 2 | 3 | 4 | 5 |
|---|---|---|---|---|---|
| De workshop was relevant voor mijn werk | ☐ | ☐ | ☐ | ☐ | ☐ |
| Ik weet nu wanneer ik wel en niet een agent inzet | ☐ | ☐ | ☐ | ☐ | ☐ |
| Ik durf zelf een eenvoudige agent te bouwen | ☐ | ☐ | ☐ | ☐ | ☐ |
| Het tempo was passend | ☐ | ☐ | ☐ | ☐ | ☐ |

**Wat zou je anders willen zien?** ______________________________

---

*Versie 1.0. Menunamen, licentiemodel en functies kunnen wijzigen; controleer ze altijd in de actuele Microsoft-documentatie.*
