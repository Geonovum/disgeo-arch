## Bijlage Principes

### Inrichtingsprincipes Digitaal Stelsel Omgevingwet

Aan de kolommen met de regel en het principe zijn twee kolommen toegevoegd: Gegevens en Functies.  
Gegevens: Een *ja* in deze kolom moet worden gezien als 'Ja' dit principe is relevant voor de gegevens in de samenhangende objectenregistratie. Scope zijn de gegevens zelf, oftewel het hart van het systeem.
Functies: Een *ja* in deze kolom moet worden opgevat als 'Ja' dit principe is relevant voor de functionaliteit van de Samenhangende Objectenregistratie. Scope is de functionaliteit waarmee de gegevens en/of de informatie aan de gebruikers wordt aangeboden.

| Regel                 | Principe                                                                 | Gegevens | Functies | 
|-----------------------|--------------------------------------------------------------------------|----------|----------|
| <p id='dso-01'>01</p> | De klant staat centraal                                                  |          |   Ja     |
| <p id='dso-02'>02</p> | Het stelsel functioneert als één geheel voor zowel personen als systemen |          |   Ja     |
| <p id='dso-03'>03</p> | Data is de brandstof van het stelsel                                     | Ja       |          |
| <p id='dso-04'>04</p> | Oplossingen zijn eenvoudig, generiek en kosten effectief                 |          |   Ja     |
| <p id='dso-05'>05</p> | Alles is een service                                                     |          |   Ja     |
| <p id='dso-06'>06</p> | Het stelsel is open, transparant en innoverend                           | Ja       |   Ja     |
| <p id='dso-07'>07</p> | Hergebruik voor koop voor maak                                           |          |          |
| <p id='dso-08'>08</p> | Continuïteit en compliance is geborgd                                    |          |          |
| <p id='dso-09'>09</p> | Passende beveiliging & privacy op basis van reële risico’s               |          |          |
| <p id='dso-10'>10</p> | Beheerfunctionaliteit is primaire functionaliteit                        |          |   Ja     |

Bron: [DSO-LV, bijlage G](https://aandeslagmetdeomgevingswet.nl/publish/library/219/ogas_bijlage_g_-_dso-lv_principes_1.pdf)

### Architectuurprincipes GEMMA Gegevenslandschap en Common Ground 

| Principe             | Omschrijving                                                                      |
|----------------------|-----------------------------------------------------------------------------------|
| <p id='cg-01'>01</p> | COMPONENTGEBASEERD: We werken met componenten                                     |
| <p id='cg-02'>02</p> | OPEN: We zijn transparant waar mogelijk                                           |
| <p id='cg-03'>03</p> | VERTROUWD: We zorgen dat informatiebeveiliging en privacy op orde zijn            |
| <p id='cg-04'>04</p> | EENMALIGE VASTLEGGING: We leggen gegevens eenmalig vast en vragen op bij de bron  |
| <p id='cg-05'>05</p> | REGIE OP GEGEVENS: We faciliteren regie op gegevens                               |
| <p id='cg-06'>06</p> | STANDAARD: We standaardiseren maximaal                                            |

Bronnen: 
- [GEMMA Gegevenslandschap](https://www.gemmaonline.nl/index.php/Gegevenslandschap)
- [Common Ground](https://commonground.nl)

### Basisprincipes NORA 

De principes van de NORA zijn bedoeld om overheidsorganisaties richting te duiden bij het inzetten van veranderingen en het
uitvoeren van projecten. Met name bij het ontwerpen van nieuwe of aangepaste diensten is het noodzaak zichtbaar te maken hoe
invulling wordt gegeven aan de principes en welke overwegingen daarbij worden gemaakt. Hier geldt het pas-toe-of-leg-uit- principe,
waarbij afwijkingen dus zijn toegestaan mits dat met goede argumenten wordt onderbouwd en vastgelegd om daar in een later
stadium op terug te kunnen komen. Zo wordt voorkomen dat belangrijke zaken over het hoofd worden gezien. 
Bron: https://www.noraonline.nl/wiki/Principes 

### Afgeleide principes NORA

Afgeleide principes geven meer concrete invulling aan de basisprincipes. Ze zijn te beschouwen als een checklist van 
kwaliteitskenmerken van de diensten van de overheid en geven handvatten voor operationeel niveau door hun uitwerking in concrete 
implicaties. 
Bron: https://www.noraonline.nl/wiki/Principes 

### Eisen aan basisregistraties

Er zijn 12 eisen aan basisregistraties waaraan een basisregistratie moet voldoen.
Bron: https://www.noraonline.nl/images/noraonline/c/c0/Stelselarchitectuur_heden.pdf 

### Woorden en Begrippenlijst

| begrip	                    | synoniem	                         | Omschrijving	                                                                      | link                   |
|-----------------------------|---------------------------------------|------------------------------------------------------------------------------------|------------------------|
| Afgeleide gegevens          | 		                              | gegevens ontstaan uit filteren, selecteren en combineren van gegevens	          |                        |
| Afgeleide gegevens service  | Convenience of process API            | Een technische dienst waarmee operaties op afgeleide gegevens mogelijk zijn, zoals lezen, toevoegen of aanpassen | |
| Afgeleide Opslag            |                                       | Een replicatie van een deel van de opslag ||
| API 		               |                                       | Application Programming Interface, de technische invulling van een service         | [API Strategie](https://docs.geostandaarden.nl/api/API-Strategie/#wat-is-een-api) | 
| Attributen	               | Gegevens		                    | | | 
| Audit-trail 	               |                                       | Vastgelegde gegevens waaruit is vast te stellen wie wanneer een bewerking van een gegeven heeft doorgevoerd | |	
| Authenticatie               | 		                              | Ben je wie je zegt dat je bent                                                     | [NORA](https://www.noraonline.nl/wiki/Authenticatie(middelen)beheer) | 
| Autorisatie                 | 		                              | Wat mag je                                                                         | [NORA](https://www.noraonline.nl/wiki/Bevoegdhedenbeheer) | 
| Begrip                      |                                       |  door mensen begrepen woord of term in vocabulaire dat in meerdere informatiemodellen gebruikt kan worden, zie MIM | [MIM](https://docs.geostandaarden.nl/mim/def-st-mim-20201023/#metagegeven-begrip) | 
| Begrippenlijst              | Informatiemodel level-1	          | | |
| Conceptueel Informatiemodel	| Informatiemodel level-2	          | | |
| CRUD Actie	               | Gegevensoperatie                         | Create, Read, Update, Delete Actie op een gegeven. De Actie  'D' is bij basisregistraties een 'U',  immers het gegeven wordt gewijzigd naar "beëindigd" | | 
| Data 	                    | Gegevens		                    | | |
| Data model                  | Informatiemodel level-4	          | | |
| Data service                | System API                            | Service waarmee operaties op gegevens mogelijk zijn, zoals lezen, toevoegen of aanpassen. Verwijderen wordt niet ondersteund in een basisregistratie | |
| Dienst                      |                                       | Levering van prestaties door dienstverlener aan afnemer op basis van vraag en behoefte | | 
| Fysiek model                | Informatiemodel level-4	          | | |
| Gegevens	               | Data                                  | Vastgelegde eigenschappen van een object | | 
| Gegevens service            | Data service 		                              |  | | 
| Gemaksservice               | Convenience API                       | API die een generieke gebruikersvraag beantwoordt | |
| Geo gegevens                | Geografische gegevens                       | Gegevens met locatie en geometrie | |
| Identificatie	          | 	                                   | Wie ben je                                                                         | [API Strategie](https://docs.geostandaarden.nl/api/API-Strategie-ext/#identification) | 
| Informatiemodel level-1	| Begrippenlijst		               |  zie MIM | [MIM](https://docs.geostandaarden.nl/mim/def-st-mim-20201023/#niveau-1-model-van-begrippen) | 
| Informatiemodel level-2	| Conceptueel Informatiemodel           | zie MIM | [MIM](https://docs.geostandaarden.nl/mim/def-st-mim-20201023/#niveau-2-conceptueel-informatiemodel )| 
| Informatiemodel level-3	| Logisch- of Gegevensmodel 	          |  zie MIM | [MIM](https://docs.geostandaarden.nl/mim/def-st-mim-20201023/#niveau-3-logisch-informatie-of-gegevensmodel) | 
| Informatiemodel level-4     | Fysiek -of Technisch gegevensmodel    |  zie MIM | [MIM](https://docs.geostandaarden.nl/mim/def-st-mim-20201023/#niveau-4-fysiek-of-technisch-gegevens-of-datamodel) | 
| Logging	                    | 	                                   | Het bijhouden van metadata over de wijziging, wanneer en door welke organisatie/bronhouder	| | 
| Logisch gegevensmodel       | Informatiemodel level-3	          | | |
| Logisch Informatiemodel     | Informatiemodel level-3	          | | |
| Metamodel Informatie Modellering (MIM)                              | | | [MIM](https://docs.geostandaarden.nl/mim/mim10/) |
| Object 	                    | 	                                   | Een ding, een tastbaar iets, in de werkelijkheid, zoals daarnaar gekeken wordt vanuit een bepaald domein.	| [MIM](https://docs.geostandaarden.nl/mim/def-st-mim-20201023/#objecten-en-objecttype) | 
| Objecten in de objectenregistratie | 	                              | Objecten die in het terrein zichtbaar zijn, zoals gebouwen, wegen, water, spoorlijnen en bomen, terreindelen, aangevuld met enkele (registratieve) objecten als woonplaatsen, gemeentegrenzen en openbare ruimten | | 
| Objectgegevens              |                                       | Vastgelegde eigenschappen van een object | | 
| Processervice               | process API, orchestration API        | API die meerdere system API's ofwel dataservices aanroept | |
| Replicatie                  |                                       | Een kopie van gegevens (maken) die gelijk is aan het origineel | | 
| Service 		          |                                       | Technische functie die leveringen van diensten mogelijk maakt	| | 
| Technisch gegevens model	| Informatiemodel level-4	          | | |
