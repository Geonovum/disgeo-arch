## Bijlagen

<p class='note'>
     WB: ik heb de bijlagen opgeschoond naar aanleiding van het aanpassen van de hoofdstukken Versiebeheer, Samenvatting, Inleiding en Afbakening. Ik heb eerst een backup (Bijagen_oud.md) gemaakt. Ik heb nog geen inhoudelijke review op de bijlage gedaan.
</p>

<p class='note'>
     WB: wat mij betreft nemen we in de bijlagen niet alle mogelijk relevante principes op uit andere bronnen, maar verwijzen we naar die bronnen (en alleen als de bron echt relevant blijkt te zijn). In de bijlagen kunnen we wel onze 'verantwoording' naar principes van anderen opnemen als dat zinvol is. Ik heb daarom de meeste tabellen met principes verwijderd. Ik heb eerst een backup (Bijagen_oud.md) gemaakt.
</p>

### Innrichtingsprincipes en Best practices 

#### Basisprincipes NORA 

De principes van de NORA zijn bedoeld om overheidsorganisaties richting te duiden bij het inzetten van veranderingen en het
uitvoeren van projecten. Met name bij het ontwerpen van nieuwe of aangepaste diensten is het noodzaak zichtbaar te maken hoe
invulling wordt gegeven aan de principes en welke overwegingen daarbij worden gemaakt. Hier geldt het pas-toe-of-leg-uit- principe,
waarbij afwijkingen dus zijn toegestaan mits dat met goede argumenten wordt onderbouwd en vastgelegd om daar in een later
stadium op terug te kunnen komen. Zo wordt voorkomen dat belangrijke zaken over het hoofd worden gezien. 
Bron: https://www.noraonline.nl/wiki/Principes 

#### Afgeleide principes NORA

Afgeleide principes geven meer concrete invulling aan de basisprincipes. Ze zijn te beschouwen als een checklist van 
kwaliteitskenmerken van de diensten van de overheid en geven handvatten voor operationeel niveau door hun uitwerking in concrete 
implicaties. 
Bron: https://www.noraonline.nl/wiki/Principes 

#### Inrichtingsprincipes GEMMA

GEMMA kent 8 inrichtingsprincipes.
Bron: https://www.vngrealisatie.nl/gemma 

#### Eisen aan basisregistraties

Er zijn 12 eisen aan basisregistraties waaraan een basisregistratie moet voldoen.
Bron: https://www.noraonline.nl/images/noraonline/c/c0/Stelselarchitectuur_heden.pdf 

#### Het 5-Sterren model voor Open Data

In het eerder in het kader van DisGeo gedane onderzoek is rapport opgesteld: 
[DisGeo Demo Lessons Learned](https://docs.geostandaarden.nl/disgeo/def-al-dll-20200219/) wordt het 
5 sterren Open Data model [genoemd](https://docs.geostandaarden.nl/disgeo/def-al-dll-20200219/#het-5-sterren-model-voor-open-data), 
Bron: https://geonovum.github.io/disgeo-demo/#governance-op-het-snijvlak

#### Inrichtingsprincipes Common Ground

Bron: https://www.gemmaonline.nl/images/gemmaonline/c/c7/20190130_-_Common_Ground_-_Informatiearchitectuurprincipes.pdf

#### 10 golden rules data

Deze 10 golden rules zijn tot stand gekomen vanuit de best-practices rondom data management. 

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


#### Inrichtingsprincipes Dis Geo

Voor het DiSGeo project is al veel onderzoek gedaan naar de eisen en inrichtingsprincipes. De resultaten zijn beschikbaar in de volgende documenten:  
Bron: https://www.geobasisregistraties.nl/documenten/beleidsnota/2019/11/29/beleidsvisie-samenhangende-objectenregistratie  
Bron: https://www.pldn.nl/file_auth.php/pilod/7/79/05_20200122_Krijtenburg_vanLeeuwen_-_DISGeo_Knowledge_Graph.pdf  

De ontwerpprincipes zijn ingedeeld in de volgende categorieën: 

| Categorie | Omschrijving                | SOR | Voorzieningen   |
|-----------|-----------------------------|-----|-----------------|
| 01        | Inhoud & scope;             |     |                 |
| 02        | Conceptueel & architectuur; | Ja  |                 |
| 03        | Organisatie;                |     |                 |
| 04        | Gebruik;                    |     | Ja              |
| 05        | Transitie.                  | Ja  | Ja              |

De relevante Architectuurprincipes zijn hieronder uitgewerkt

##### Ontwerpprincipes conceptueel en architectuur 
De volgende conceptuele en architectuur uitgangspunten worden gehanteerd bij het komen tot een nadere uitwerking van een
samenhangende objectenregistratie:  
 
| Nummer  | Beschrijving                                                                                         | Gegevens  | Functionaliteit  |
|---------|------------------------------------------------------------------------------------------------------|------|----------------|
| 01      | We laten ons bij het ontwerp en de verdere uitwerking niet beperken door de nu bestaande juridische kaders (deze kunnen in principe worden aangepast, via een traject aanpassing wet- en regelgeving). | Ja | Ja |
| 02      | In het ontwerp van een samenhangende objectenregistratie is sprake van een nadrukkelijke scheiding tussen de vastlegging van gegevens en de functionaliteit voor het bewerken, opvragen en presenteren daarvan. | Ja | Ja |
| 03      | Er wordt gebruik gemaakt van standaard infrastructurele voorzieningen die beschikbaar zijn bij de bronhouders en de gebruikers (denk hierbij aan standaardnetwerken, netwerkprotocollen en beveiligingsmechanismen). | | |
| 04      | Er wordt in de eindsituatie zoveel mogelijk uitgegaan van ‘bevragen bij de bron’. Hierbij is van belang dat de gebruiker voor verstrekkingen zoveel mogelijk uit kan gaan van één loket. Een belangrijk aandachtspunt hierbij is het gebeurtenis georiënteerd werken (nader uit te werken). Of de bronhouders gedistribueerd en decentraal werken of direct inwinning en bijhouding in een (of meerdere) voorziening(en) uitvoeren via gestandaardiseerde services moet nader bepaald worden. | | Ja |
| 05      | Er wordt ingewonnen op het niveau van de huidige schaalniveaus van BAG en BGT. De gegevens kunnen gepresenteerd worden op verschillende schaalniveaus (meest gedetailleerde weergave: 1:1.000). Autogeneralisatie voor informatie op hogere schaalniveaus moet mogelijk zijn (op basis van logica en functies). Bijvoorbeeld het (deels) afleiden van de informatie voor de BRT uit de BGT, maar ook voor het definiëren van een wegennetwerk met alle rijkswegen op basis van het gehele wegennetwerk. | | |
| 06      | Keuzen voor een technische inrichting van de registratie worden pas later in het traject gemaakt, zodat oplossingen gebaseerd zijn op recente inzichten in oplossingsmogelijkheden. | | |

Bron: https://www.geobasisregistraties.nl/documenten/beleidsnota/2019/11/29/beleidsvisie-samenhangende-objectenregistratie  

##### Ontwerpprincipes gebruik 

De volgende uitgangspunten betrekking hebbende op gebruik worden gehanteerd bij het komen tot een nadere uitwerking van een samenhangende objectenregistratie: 

| Nummer | Beschrijving                                                                                         |  SOR | Voorzieningen  |
|--------|------------------------------------------------------------------------------------------------------|------|----------------|
| 01     | Vanuit andere (basis)registraties, zoals de subjectenregistraties BRP of HR, moeten eenvoudig relaties gelegd kunnen worden naar de samenhangende objectenregistratie. | Ja | Ja |
| 02     | De registratie gedraagt zich voor gebruikers zoveel mogelijk als één registratie, of het daadwerkelijk één registratie wordt, is nog niet bepaald (nader uit te werken). Daarnaast kunnen er uit de registratie (informatie)producten afgeleid worden en beschikbaar gesteld worden. | Ja | Ja | 
| 03     | De kerngegevens en aanvullende gegevens worden in principe ontsloten als open data (waar nodig ontsloten op basis van autorisaties), dus het “open data, tenzij” regime geldt.|  | Ja |
| 04     | Op het moment dat er sprake is van nadrukkelijk gedeelde behoeften van gebruikers aan aanvullende gegevens, dan komen deze in principe in aanmerking voor opname in de basisregistratie (waarbij gedocumenteerd wordt door wie de wensen geuit zijn, en waarop gebaseerd). | Ja |  |
| 05     | Vanuit gebruikerswensen wordt gekeken naar wat dit betekent voor een objectenregistratie en pas daarna wat dit betekent voor het huidige informatiemodel (inhoud en relaties); bestaande registraties mogen niet beperkend zijn voor de doorontwikkeling. | Ja |  |
| 06     | In principe kan de informatie via meerdere kanalen, afgestemd op gebruikersbehoefte, uitgeleverd worden (nadere uitwerking in kader van DiS GEO). |  | Ja  | 
 
Bron: https://www.geobasisregistraties.nl/documenten/beleidsnota/2019/11/29/beleidsvisie-samenhangende-objectenregistratie  
 
##### Ontwerpprincipes transitie 

De volgende uitgangspunten betrekking hebbende op het transitieproces worden gehanteerd bij het komen tot een nadere uitwerking van een 
samenhangende objectenregistratie:  
 
| Nummer | Beschrijving                                                                                         | SOR  | Voorzieningen  |
|--------|------------------------------------------------------------------------------------------------------|------|----------------|
| 01     | De transitie zal geleidelijk / organisch (via tussenstappen, gericht op een ‘eindbeeld / streefbeeld’) vormgegeven worden, zo kan de impact bij bronhouders en gebruikers beperkt worden. 
| 02     | Alle gemaakte keuzen worden voor transitie en implementatie beproefd op de impact voor zowel de bronhouders als de gebruikers (inclusief afspraken over financieringswijze). Op het moment dat er sprake is van nadrukkelijk gedeelde behoeften van gebruikers aan aanvullende gegevens, dan komen deze in principe in aanmerking voor opname in de basisregistratie (waarbij expliciet wordt gedocumenteerd door wie behoeften zijn geuit en waar deze op zijn gebaseerd). De extra inwinningslast zal, waar mogelijk, zoveel mogelijk beperkt worden. |  |  |
| 03     | Alle gemaakte keuzen worden voor implementatie/transitie beproefd op de impact voor zowel de bronhouders als de gebruikers (inclusief afspraken over financiering en kosten/baten). 
| 04     | Welke stappen in het transitieproces gezet zullen worden en wat ‘permanent Beta’ betekent voor de praktijk van bronhouders en gebruikers zal nader verkend worden |  |  |

Bron: https://www.geobasisregistraties.nl/documenten/beleidsnota/2019/11/29/beleidsvisie-samenhangende-objectenregistratie  

