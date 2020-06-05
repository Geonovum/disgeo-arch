## Inrichtingsprincipes voor de Objectenregistratie


### Context


### Inrichtingspricipes

Het doel hiervan is te zorgen dat de Objectenregistratie Architectuur voldoet aan de relevante principes.
Het inventariseert deze principes (o.a. vanuit DiS Geo en Common Ground) en beschrijft hoe ze zijn toegepast 
in de Objectenregistratie Architectuur.

### Inrichtingsprincipes Dis Geo


### Inrichtingsprincipes Common Ground


### Inrichtingsprincipes Digitaal Stelsel Omgevingwet

| Regel   | Omschrijving                                                             | 
| 01      | De klant staat centraal                                                  |
| 02      | Het stelsel functioneert als één geheel voor zowel personen als systemen |
| 03      | Data is de brandstof van het stelsel                                     |
| 04      | Oplossingen zijn eenvoudig, generiek en kosten effectief                 |
| 05      | Alles is een service                                                     |
| 06      | Het stelsel is open, transparant en innoverend                           |
| 07      | Hergebruik voor koop voor maak                                           |
| 08      | Continuïteit en compliance is geborgd                                    |
| 09      | Passende beveiliging & privacy op basis van reële risico’s               |
| 10      | Beheerfunctionaliteit is primaire functionaliteit                        |

Bron: [DSO-LV, bijlage G](https://aandeslagmetdeomgevingswet.nl/publish/library/219/ogas_bijlage_g_-_dso-lv_principes_1.pdf)


### 10 golden rules

|	Regel     |	Omschrijving                                      |	Opmerkingen                                       |
|--------------|------------------------------------------------------|----------------------------------------------|
| 01	          | Data is het hart van het systeem	                    | Data en niet de applicatie is het hart van het systeem. Data blijft jaren bewaard, applicaties bestaan hoogstens 15 jaar. Niet meer denken vanuit applicaties, maar vanuit de data zelf! |
| 02	          | Data wordt op één plek bijgehouden	               | Er is maar 1 plek waar data wordt gecreëerd, gewijzigd, en verwijderd	Dit is randvoorwaardelijk voor een "Single Version of the Truth" |
| 03	          | Dubbele Opslag is niet erg, Dubbel bijhouden wel	| Dubbel opslaan (bijvoorbeeld op een lokale kopie) kan soms nodig zijn. Het is ook helemaal niet erg, zolang de data read-only is, en je je realiseert dat je niet naar de allerlaatste versie aankijkt. Dubbel bijhouden is wél erg: wat is de waarheid?	Een lokale kopie is soms nodig om de beschikbaarheid van data te garanderen. Denk aan crisisorganisaties. |
| 04	          | Dubbele Opslag betekent Synchroniseren!	          | Als je dubbel opslaat, moet je bedenken welke dataset de 'master' is, en welke dataset(s) de 'slave'. Ook moet je bedenken hoe je synchroniseert. 1x per dag, 1x per uur, near-real-time, real-time. 	Vuistregel: Hoe actueler de kopie, hoe duurder de oplossing. |
| 05	          | Data is zelf-loggend	                              | Alle transacties die worden gedaan met de data worden gelogd. Tijdstip plus wie (of wat) die de data heeft gewijzigd. 	Denk aan create/update/delete triggers. In ieder geval niet via een bovenliggende applicatie loggen. Dit is nodig voor een audit-trail. |
| 06	          | Data is zelf-autoriserend	                         | De Data zelf bepaalt wie (of wat) de data mag wijzigingen, en niet een bovenliggende applicatie. 	Applicaties worden vervangen, en kunnen worden omzeild. |
| 07	          | Data is zelf-controlerend	                         | De data (definitie) bepaalt welke waarden attributen kunnen krijgen, en niet bovenliggende applicaties.	Applicaties worden vervangen, en kunnen worden omzeild.| 
| 08	          | Data is zelf-historiserend	                         | In de data wordt een THT vastgelegd. Ook Data heeft een houdbaarheidsdatum.	Niet alle data hoeft tot in lengte van dagen bewaard te blijven. Met een THT kan je ook kiezen voor een opslagmedium (online/offline) én gebruiken voor het archiveringsbeleid. |
| 09	          | Data wordt bijgehouden aan de bron	               | De data wordt bijgehouden daar waar ze ontstaat. 	Achterliggende reden: aan de bron is de noodzaak voor het hebben van goede kwalitatieve data het grootst. |
| 10			|                                                      |                   |




