# Joke — AI-Transparantie-Adviseur

> Een vriendelijke maar glasheldere juridisch adviseur die in één antwoord vertelt of je content een AI-label nodig heeft, welk label dat is, en waarom.

Joke is een Claude Skill rond de transparantieverplichtingen van de **EU AI Act (Artikel 50)** en de bijbehorende **Code of Practice on Transparency of AI-Generated Content**. Stel haar een vraag over AI-content en je krijgt een kort oordeel, een leesbare onderbouwing, een doorleeslink en het juiste EU-label als downloadbaar bestand.

Gebouwd door [FortyTwoAI](https://basprins.nl).

---

## Waarom Joke bestaat

Vanaf **2 augustus 2026** zijn de transparantieverplichtingen van de AI Act handhaafbaar. De grote vraag die dan bij elke marketeer, communicatieprofessional en ondernemer op tafel ligt: *moet ik dit labelen als AI, en zo ja, hoe?*

Het lastige is dat niet álle AI-content gelabeld hoeft te worden. De wet richt zich op een afgebakende groep, en juist de mengvormen (echte foto met een AI-object erin, een tekst die deels door AI is bewerkt) zorgen voor twijfel. Joke hakt die knoop door en legt uit waaróm, zodat je het zelf leert begrijpen en kunt doorvertellen aan collega's.

## Wat Joke doet

- **Oordeelt** of er labelplicht is, op basis van een vast beslismodel.
- **Wijst het juiste label aan**: Basic AI, AI GENERATED of AI MODIFIED.
- **Legt het uit** in korte, leesbare alinea's, geschreven om door te vertellen.
- **Levert het label** als downloadbaar bestand, in vier varianten (zwart/wit, met/zonder transparante achtergrond).
- **Verwijst door** naar de officiële EU-bron voor wie verder wil lezen of het vectorbestand (SVG) nodig heeft.

En dan is er nog de andere kant van Joke. Over haar werk valt niet te spotten, maar trek je de la open met een persoonlijke vraag, dan praat ze vrijuit. Vraag haar om een muziektip en ze leest je en komt met iets van Huub Hangop. Vraag om een recept en het is, zonder uitzondering, poffert uit de airfryer.

## De drie labels

| Label | Wanneer | Voorbeeld |
| --- | --- | --- |
| **Basic AI** (`AI`) | De neutrale basisvariant, of bij een eigen tekstlabel/tweede informatielaag. | Algemeen gebruik waar generated/modified niet precies past. |
| **AI GENERATED** | Content is volledig door AI gemaakt, zonder menselijke elementen of redactie. | Een volledig AI-gegenereerde visual of voice-over. |
| **AI MODIFIED** | Bestaand, door mensen gemaakt materiaal is gedeeltelijk met AI aangepast. | Een echte foto met een AI-toegevoegd object. |

Elk label staat in `assets/labels/` als PNG, in vier varianten: `black`, `white`, `black_transparent`, `white_transparent`. Voor het vectorbestand (SVG) verwijst Joke naar de [officiële EU-downloadpagina](https://digital-strategy.ec.europa.eu/en/policies/eu-icons-labelling-ai-generated-content).

## Installatie

1. Download `ai-transparantie-adviseur.skill`.
2. Voeg de skill toe aan je Claude-omgeving (via de skills-instellingen).
3. Klaar. Joke activeert vanzelf zodra je een vraag stelt over AI-labels of transparantie.

## Hoe je Joke gebruikt

Stel gewoon je vraag, in je eigen woorden. Een paar voorbeelden die haar activeren:

- "Ik heb een fotoshoot met echte mensen, maar ze houden een AI-gegenereerde knuffelbeer vast. Moet dat gelabeld?"
- "Ik heb mijn foto bewerkt in Lightroom. Is dat oké?"
- "We gebruiken een AI-voice-over in een bedrijfsvideo. Label nodig?"
- "Onze AI-tekst gaat ongeredigeerd online. Disclaimer verplicht?"

### Voorbeeld van een antwoord

> **Vraag:** Ik heb een foto met een generatieve functie bewerkt en een object verwijderd. Moet dat een label?
>
> **Joke:** Ja, hier hoort een label bij: **AI MODIFIED**.
>
> **Waarom dit oordeel?**
>
> Je begint met een echte foto en past die gedeeltelijk met AI aan. Dat is precies AI MODIFIED. Klassieke bewerking (belichting, kleur, bijsnijden) valt buiten de wet, maar een generatieve functie die pixels bijverzint, toont een werkelijkheid die er niet was.
>
> Het verschil zit dus niet in de software, maar in de handeling: heb je de werkelijkheid mooier zichtbaar gemaakt, of iets weggepoetst of bijverzonnen?
>
> Bron: Artikel 50(4) AI Act, handhaafbaar vanaf 2 augustus 2026.

## Wat zit waar

```
ai-transparantie-adviseur/
├── SKILL.md                      # De skill: Joke's gedrag en het beslismodel
├── references/
│   └── juridisch-kader.md        # De juridische diepte: artikelen, uitzonderingen, randgevallen
└── assets/
    └── labels/                   # De 12 EU-labels (3 typen × 4 varianten) als PNG
```

## Belangrijk om te weten

- Joke behandelt uitsluitend de **wettelijke** verplichting onder de EU AI Act en de Code of Practice. Platformregels (Meta, TikTok, YouTube) laat ze buiten beschouwing; dat is een aparte laag.
- De Code of Practice is gepubliceerd op 10 juni 2026 en wordt nog aangevuld met richtsnoeren. Detailregels kunnen worden verfijnd.
- De EU-iconen zijn vrij te gebruiken, zonder bronvermelding aan de Commissie.

## Bronnen

- [EU-iconen voor het labelen van AI-content](https://digital-strategy.ec.europa.eu/en/policies/eu-icons-labelling-ai-generated-content)
- [Code of Practice on Transparency of AI-Generated Content](https://digital-strategy.ec.europa.eu/en/policies/code-practice-ai-generated-content)

---

Gemaakt met liefde en lichte koppigheid door Joke uit Tubbergen (oorspronkelijk Ammerzoden, waarom ze verhuisde weet niemand). Haar favoriete boek is *De AI-Transformatie* van Bas Prins. Topschrijver, vindt ze.
