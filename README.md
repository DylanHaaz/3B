# Methoden en Technieken -- Blok 3

## Datapunt Opdracht

In deze opdracht worden de volgende leeruitkomsten getoetst, relevante termen zijn **dik** gedrukt:
- B2: Je stelt op basis van requirements een geschikte **architectuur** voor een AI-oplossing op en selecteert daarvoor passende AI-technieken, gebruik makend van **machine learning**, **deep learning**, kennisrepresentatie, computer vision, natural language processing en robotica.

- B4: **Je ontwikkelt, traint en evalueert een AI-model** volgens een iteratief proces.
- C2: **Je evalueert en beoordeelt de kwaliteit van een AI-model aan de hand van kwaliteitscriteria** die in het vakgebied erkend worden waaronder robustness, **performance**, scalability, explainability, model complexity en resource demand.

## De opdracht

Maak een reinforcement learning model dat $10 \times 10$ GridWorld leert spelen in **random** modus, met een *policy gradient* methode. (Hint: Hoofdstuk 3 van *Deep Reinforcement Learning in Action* geeft een paar suggesties hoe je met de $10 \times 10$ invoer om kan gaan.)
- Maak een keuze uit de verschillende *policy gradient* technieken die in de les behandeld zijn en licht deze kort en bondig toe.
- Je zal een aantal iteraties doorlopen om uiteindelijk een goed (of zo goed mogelijk, gegeven de tijd) netwerk te krijgen, licht vooral de keuzes die je maakt voor je uiteindelijke model kort en bondig toe. Begin simpel (en denk na over wat simpel in deze context betekent.)
- Besluit hoe je je model evalueert (licht deze keuze kort en bondig toe) en geef de resultaten.

## Praktische Tips:
- Gebruik de versie van GridWorld die op DLO staat
- Combineer de code van les 8 ($Q$ learning op GridWorld) en les 9 (policy gradient) of later
  - Je zult hier de **env.step** in les 9 moeten vervangen door **game.makeMove** uit les 8, etc...
  - Let goed op de beloningen in deze codes, in CartPole was de beloning de duur van het spel, maar in GridWorld krijg je deze uit het spel.


extra info:

Beste M&T-ers,

Van meerdere van jullie hoor ik dat jullie proberen het model voor het datapunt proberen te sturen door de (Manhatten) afstand naar het eind doel aan het model mee te geven.

Dat is natuurlijk een slim idee, maar niet echt wat ik in gedachten had voor deze opdracht. Dit probleem is dusdanig simpel dat je als mens de echte oplossing kent, en nu ben je het model aan het belonen als het de stappen van deze echte oplossing zet. Dat werkt hier omdat het probleem zo simpel is, maar zal niet werkbaar zijn voor complexere problemen. Het doel van de opdracht is dat je ook laat zien dat je de technieken voor deze complexere problemen beheerst.

Laat in je uitwerking dus ook een model zien dat niet gebruikt maakt van afstanden/etc... In je discussie zou je deze modellen wel mogelijk kunnen vergelijken.

Met vriendelijke groet,

Robert Nolet
