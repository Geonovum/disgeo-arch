## Bijlage Principes

### Inrichtingsprincipes Digitaal Stelsel Omgevingwet

Aan de kolommen met de regel en het principe zijn twee kolommen toegevoegd: <m>Gegevens</m> en Functies.  
<m>Gegevens</m>: Een *ja* in deze kolom moet worden gezien als 'Ja' dit principe is relevant voor de gegevens in de samenhangende objectenregistratie. Scope zijn de gegevens zelf, oftewel het hart van het systeem.
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
- [Common Ground](https://commonground)

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

### De 10 golden rules data

Deze 10 golden rules zijn tot stand gekomen vanuit de best-practices rondom data management. 
<m>Deze principes zijn gebaseerd op de principes van [DAMA](https://www.dama.org/cpages/home), aangevuld met praktijkervaringen</m>
<m>In deze principes wordt het woord "data" gebruikt. In het kader van DisGEO is het woord "data" synoniem met "gegevens"</m>

|	Regel |	Omschrijving                                     |	Opmerkingen                                       | Data | Functies |
|--------|---------------------------------------------------|---------------------------------------------------|-----|---------------|
| 01	   | Data is het hart van het systeem	                | Data blijft jaren bewaard, applicaties bestaan hoogstens 15 jaar. We denken niet meer vanuit applicaties, maar vanuit de data zelf! |  Ja |               |
| 02	   | Data wordt op één plek bijgehouden	             | Er is maar 1 plek waar data wordt gecreëerd, gewijzigd en verwijderd (beëindigd). Dit is randvoorwaardelijk voor een "Single Version of the Truth" |  Ja |               |
| 03	   | Dubbele opslag is niet erg, dubbel bijhouden wel	 | Dubbel opslaan (bijvoorbeeld op een lokale kopie) kan soms nodig zijn. Het is ook helemaal niet erg, zolang de data read-only is, en je je realiseert dat je niet naar de allerlaatste versie kijkt. Dubbel bijhouden is wél erg want dan weet je niet meer "Wat is de waarheid?". Een lokale kopie is soms nodig om de beschikbaarheid van data te garanderen. Denk aan crisisorganisaties. |  Ja |               |
| 04	   | Dubbele opslag betekent synchroniseren!	          | Dubbel opslaan vereist toepassing van spelregels. Als je dubbel opslaat, moet je vastleggen welke dataset de 'master' is, en welke dataset de 'slave'. Ook moet je bedenken hoe je synchroniseert. 1x per dag, 1x per uur, near-real-time, real-time. Vuistregel: Hoe actueler de kopie, hoe duurder de oplossing. | Ja  |               |
| 05	   | Data is zelf-loggend	                            | Alle transacties die worden gedaan met de data worden gelogd. Tijdstip plus wie (of wat) de data heeft gewijzigd. Hierdoor kan een wijziging triggers veroorzaken voor afnemers die in hun proces create/update/delete triggers nodig hebben. Loggen gebeurt in ieder geval niet via een bovenliggende applicatie. Dit is nodig voor een audit-trail. | Ja  |               |
| 06	   | Data is zelf-autoriserend	                      | De data zelf bepaalt wie (of wat) de data mag wijzigingen, en niet een bovenliggende applicatie. Applicaties worden vervangen, en kunnen worden omzeild. | Ja  |               |
| 07	   | Data is zelf-controlerend	                      | De data (definitie) bepaalt welke waarden attributen kunnen krijgen, en niet bovenliggende applicaties.	Applicaties worden vervangen, en kunnen worden omzeild.| Ja   |               |
| 08	   | Data is zelf-historiserend	                      | In de data wordt een THT-datumtijd ("tenminste houdbaar tot") vastgelegd. Data heeft een houdbaarheidsdatum.	Niet alle data hoeft even lang op dezelfde manier bewaard te blijven. Met een THT kun je kiezen voor geschikte opslag (qua toegang en opslagmedium (online/offline)) én kun je invulling geven aan  archiveringsbeleid. | Ja  |               |
| 09	   | Data wordt bijgehouden aan de bron	             | De data wordt bijgehouden daar waar ze ontstaat. Achterliggende reden: aan de bron is de noodzaak en de mogelijkheid voor het hebben van goede kwalitatieve data het grootst. | Ja | Ja |
| 10		| Data en Informatie zijn twee verschillende dingen | Informatie is "bewerkte data", met andere woorden, informatie is data waaraan kennis is toegevoegd.                  |     |               |
