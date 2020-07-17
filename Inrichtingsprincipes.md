## Inrichtingsprincipes voor de Objectenregistratie

### Context

De richtinggevende principes van DiS Geo zijn verwoord in de beleidsvisie DiS Geo, en hieraan wordt ook wel gerefereerd als "de [houtskoolschets](https://www.geobasisregistraties.nl/basisregistraties/documenten/publicatie/2020/06/15/dis-online-als-stroom-uit-het-stopcontact)".

In dit hoofdstuk worden de inrichtingsprincipes die van toepassing zijn op de Samenhangende Objecten Registratie 
bepaald als nadere invulling van de richtinggevende visie in de houtskoolschets. 
Er is voor gekozen om als uitgangspunt de [Overall Globale Architectuur Schets (OGAS)](https://aandeslagmetdeomgevingswet.nl/publish/library/219/dso_-_gas_-_overall_gas_1.pdf) te gebruiken, die is opgesteld ten behoeve van het Digitaal Stelsel Omgevingswet. Bij het opstellen van de architectuurschets voor het DSO is in het recente verleden gekeken naar diverse andere relevante richtinggevende principes zoals [NORA](#basisprincipes-nora), [GEMMA](#inrichtingsprincipes-gemma) en [Common Ground](#inrichtingsprincipes-common-ground) en is een hanteerbare set principes afgeleid. 
Door deze set principes als uitgangspunt te nemen, ontstaan bij de doorontwikkeling van de geo basisregistraties en de implementatie van de Omgevingswet elkaar versterkende effecten. Dit is wenselijk, omdat beide ontwikkelingen gaan over gegevens die de fysieke leefwereld betreffen. Dubbel architectuurwerk wordt zo voorkomen, en principes sluiten zo goed op elkaar aan.
Naast de principes uit de DSO architectuur is ook gekeken naar de internationale architectuurprincipes van W3C, en dan met name naar de principes uit [Spatial Data on the Web Best Practices](https://www.w3.org/TR/sdw-bp/#bp-summary) die zijn opgetekend op basis van vele internationale ervaringen met het omgaan met geo gegevens. 

### Doel van de Samenhangende Objecten Registratie

In de beleidsvisie voor de samenhangende objectenregistratie wordt een vijftal doelstellingen geformuleerd:

| Doel |	Omschrijving                                                                           |
|------|-----------------------------------------------------------------------------------------|
| 01	 | Een betrouwbare, consistente en actuele samenhangende gegevensset voor heel Nederland;  |  
| 02   | Een efficiëntere inwinning en bijhouding van objecten, ook in drie dimensies (3D);      | 
| 03   | Een betere inpassing in moderne architecturen;                                          | 
| 04   | Meer en eenvoudiger gebruik van deze informatie in maatschappelijke toepassingen. De registratie gedraagt zich voor de gebruiker als één registratie. |
| 05   | De objectenregistratie maakt onderdeel uit van een robuuste geo-informatie infrastructuur binnen de generieke digitale infrastructuur en voldoet aan de [12 eisen voor een basisregistratie](# eisen-aan-basisregistraties-GEMMA)  |

In de kern gaat het hierbij om een nadrukkelijke scheiding van de vastlegging van de gegevens, en de functionaliteiten die 
nodig zijn voor het bewerken, opvragen en het presenteren van deze gegevens tot logische informatie. 

Bron: https://www.geobasisregistraties.nl/documenten/beleidsnota/2019/11/29/beleidsvisie-samenhangende-objectenregistratie  

### Doel van de Inrichtingsprincipes

Het doel van het formuleren van inrichtinsprincipes is te zorgen en te borgen dat de architectuur van de Samenhangende Objecten Registratie invulling geeft aan de architectuurvisie DiS Geo en de daarin benoemde richtinggevende uitspraken. Door de doorontwikkeling van de geobasisregistraties onder architectuur te laten plaatsvinden, realiseren de betrokken ketenpartners stapsgewijs de visie.

### Hoe komen we tot de Inrichtingsprincipes?

Er is gekeken naar de principes van reeds bestaande registraties en naar principes die zijn aangedragen vanuit DiS Geo en Common Ground.
Er is vooral gekeken naar principes die nodig zijn om de gewenste vernieuwing door te kunnen voeren.
We bouwen voort op een drietal bronnen: DSO, Best Practices en Common Ground. We lichten deze nu toe: 

#### Inrichtingsprincipes Digitaal Stelsel Omgevingwet

Aan de kolommen met de regel en het principe zijn twee kolommen toegevoegd: Data en Functies.  
Data: Een *ja* in deze kolom moet worden gezien als 'Ja' dit principe is relevant voor de gegevens in de samenhangende objectenregistratie. Scope zijn de gegevens zelf, oftewel het hart van het systeem.
Functies: Een *ja* in deze kolom moet worden opgevat als 'Ja' dit principe is relevant voor de functionaliteit van de Samenhangende Objectenregistratie. Scope is de functionaliteit waarmee de gegevens en/of de informatie aan de gebruikers wordt aangeboden.

| Regel                 | Principe                                                                 | Data | Functies | 
|-----------------------|--------------------------------------------------------------------------|------|----------|
| <p id='dso-01'>01</p> | De klant staat centraal                                                  |      |   Ja     |
| <p id='dso-02'>02</p> | Het stelsel functioneert als één geheel voor zowel personen als systemen |      |   Ja     |
| <p id='dso-03'>03</p> | Data is de brandstof van het stelsel                                     | Ja   |          |
| <p id='dso-04'>04</p> | Oplossingen zijn eenvoudig, generiek en kosten effectief                 |      |   Ja     |
| <p id='dso-05'>05</p> | Alles is een service                                                     |      |   Ja     |
| <p id='dso-06'>06</p> | Het stelsel is open, transparant en innoverend                           | Ja   |   Ja     |
| <p id='dso-07'>07</p> | Hergebruik voor koop voor maak                                           |      |          |
| <p id='dso-08'>08</p> | Continuïteit en compliance is geborgd                                    |      |          |
| <p id='dso-09'>09</p> | Passende beveiliging & privacy op basis van reële risico’s               |      |          |
| <p id='dso-10'>10</p> | Beheerfunctionaliteit is primaire functionaliteit                        |      |   Ja     |

Bron: [DSO-LV, bijlage G](https://aandeslagmetdeomgevingswet.nl/publish/library/219/ogas_bijlage_g_-_dso-lv_principes_1.pdf)

#### Best Practices Spatial Data on the Web

| Nummer                 | Best Practices Summary                                                 | Data | Functies |
|------------------------|------------------------------------------------------------------------|------|----------|
| <p id='sdow-01'>01</p> | Use globally unique persistent HTTP URIs for Spatial Things            | Ja   | Ja       |
| <p id='sdow-02'>02</p> | Make your spatial data indexable by search engines                     | Ja   | Ja       |
| <p id='sdow-03'>03</p> | Link resources together to create the Web of data                      | Ja   | Ja       |
| <p id='sdow-04'>04</p> | Use spatial data encodings that match your target audience             | Ja   | Ja       |
| <p id='sdow-05'>05</p> | Provide geometries on the Web in a usable way                          | Ja   | Ja       |
| <p id='sdow-06'>06</p> | Provide geometries at the right level of accuracy, precision, and size | Ja   | Ja       |
| <p id='sdow-07'>07</p> | Choose coordinate reference systems to suit your user's applications   | Ja   | Ja       |
| <p id='sdow-08'>08</p> | State how coordinate values are encoded                                |      |          |
| <p id='sdow-09'>09</p> | Describe relative positioning                                          |      |          |
| <p id='sdow-10'>10</p> | Use appropriate relation types to link Spatial Things                  | Ja   | Ja       |
| <p id='sdow-11'>11</p> | Provide information on the changing nature of spatial things           | Ja   | Ja       |
| <p id='sdow-12'>12</p> | Expose spatial data through 'convenience APIs'                         | Ja   | Ja       |
| <p id='sdow-13'>13</p> | Include spatial metadata in dataset metadata                           | Ja   | Ja       |
| <p id='sdow-14'>14</p> | Describe the positional accuracy of spatial data                       | Ja   | Ja       |

Bron: [Spatial Data on the Web Best Practices](https://www.w3.org/TR/sdw-bp/)


#### Inrichtingsprincipes Common Ground

| Principe              | Omschrijving                                                                      |
|-----------------------|-----------------------------------------------------------------------------------|
| <p id='cg-01'>01</p> | COMPONENTGEBASEERD: We werken met componenten                                     |
| <p id='cg-02'>02</p> | OPEN: We zijn transparant waar mogelijk                                           |
| <p id='cg-03'>03</p> | VERTROUWD: We zorgen dat informatiebeveiliging en privacy op orde zijn            |
| <p id='cg-04'>04</p> | EENMALIGE VASTLEGGING: We leggen gegevens eenmalig vast en vragen op bij de bron  |
| <p id='cg-05'>05</p> | REGIE OP GEGEVENS: We faciliteren regie op gegevens                               |
| <p id='cg-06'>06</p> | STANDAARD: We standaardiseren maximaal                                             |

Bron: [Common Ground](https://www.gemmaonline.nl/images/gemmaonline/c/c7/20190130_-_Common_Ground_-_Informatiearchitectuurprincipes.pdf)

### Inrichtingsprincipes Samenhangende Objectenregistratie

De inrichtinsprincipes voor de Samenhangende Objecten Registratie zijn, gebaseerd op DSO, best practices, en Common Ground, samengevat de volgende:

CONCEPT

#### Processen en gegevens worden gescheiden
#### Gegevens worden eenmalig bijgehouden (“op één plek”)
#### Dubbele opslag betekent synchroniseren
#### Alle handelingen worden gelogd
#### “Autorisatie op gegevens volgt uit inhoud van gegevens”
#### Data bevat metadata met link naar structuur, definities en relaties
#### Ontkoppeling en interoperabiliteit maken verandering mogelijk (middels API strategie en URI strategie)
#### Informatie is gepresenteerde data in context

CONCEPT


### Hoe passen de inrichtingsprincipes bij de visie van DiS-Geo?

In de paragrafen hieronder staan de principes ofwel richtinggevende uitspraken uit de visie van DiS-Geo. Per principe (richtinggevende uitspraak) is aangegeven hoe de 
hiervoor genoemde inrichtingsprincipes invulling geven aan deze principes.

#### Basisgegevens zijn van en voor iedereen

[DSO-01](#dso-01), [DSO-02](#dso-02), [DSO-04](#dso-04), [DSO-06](#dso-06), [SDOW-01](#sdow-01), [SDOW-02](#sdow-02), [SDOW-03](#sdow-03), [SDOW-12](#sdow-12)

Geo basisgegevens hebben identificatie, metadata, een basisclassificatie, locatie en geometrie.

Identificatie

Basisgegevens hebben een altijd een *unieke sleutel* [SDOW-01](#sdow-01), deze wordt gebruikt om gegevens te kunnen koppelen. Daarnaast
hebben basisgegevens *identificerende kenmerken*, waarmee de objecten door mensen herkend kunnen worden. Zo is een woonadres iets dat door mensen
begrepen wordt, maar juist voor machine koppelingen voor allerlei problemen zorgt (adresproblematiek met verschillende schrijfwijzen).

Het is aan te raden ook een *eigenaarskenmerk* op te nemen bij objecten in de basisregistratie. hiermee is meteen duidelijk wie er
verantwoordelijk is voor de data. Soms wordt ook een *beheerderkenmerk* opgenomen, daarmee wordt het mogelijk om verschil te maken tussen
de eigenaarsrol en de beheerderrol.

Verder bevatten objecten in de registratie een *geldigheid*, in de vorm van een van-datumtijd en/of een tot-datumtijd. Deze wordt gebruikt voor 'tijdreizen', maar ook voor archiveringsdoeleinden.

Om objectgegevens te kunnen koppelen met andere basisregistraties en sectorale (kern)registraties moet een sleutel aan de URI strategie voldoen. Zo kan webtechnologie worden  gebruikt om te zorgen dat de objecten in de registraties voor mensen en machines te vinden zijn en door mensen en machines in samenhang kunnen worden afgenomen en gebruikt .  

#### Basisgegevens zijn laagdrempelig beschikbaar en bruikbaar voor iedereen

[DSO-01](#dso-01), [DSO-02](#dso-02), [SDOW-02](#sdow-02), [SDOW-02](#sdow-03), [SDOW-12](#sdow-12)

Om basisgegevens voor iedereen beschikbaar en bruikbaar te maken moeten ze goed vindbaar zijn. De vindbaarheid wordt sterk vergroot
als de basisgegevens vindbaar zijn via zoekmachines. Daarom moeten de gegevens naast de "echte" gegevens ook metadata (gegevens over de gegevens) bevatten.

#### Basisgegevens voldoen aan vereisten

[DSO-03](#dso-03),[DSO-05](#dso-05),[DSO-06](#dso-06), [CG-01](#cg-01), [CG-03](#cg-03)

Omdat gegevens de brandstof zijn voor het systeem, moeten deze betrouwbaar zijn. Betrouwbare gegevens voldoen aan vooraf vastgelegde
eisen. Het is voor iedereen duidelijk aan welke criteria de gegevens voldoen. 

#### Bronhouders zijn verantwoordelijk voor basisgegevens

[DSO-10](#dso-10), [CG-04](#cg-04), [CG-05](#cg-05)

Bronhouders zijn en blijven te allen tijde verantwoordelijk voor de basisgegevens. Verantwoordelijk voor de vastlegging/registratie en voor de kwaliteit. 

Doordat de gegevens als "open data" beschikbaar worden gesteld, bestaat een situatie waarin veel mensen (en machines) de gegevens gebruiken, en daarbij impliciet controleren. 
Een goede terugmeld mogelijkheid is noodzakelijk, om feedback aan bronhouders te kunnen doorgeven als er twijfel bestaat over de juistheid. 
Door terugmeldingen op te volgen vullen bronhouders hun verantwoordelijkheid voor de gegevenskwaliteit in.

#### Bronhouders kunnen leveranciers machtigen

[DSO-10](#dso-10), [CG-04](#cg-04)

Bronhouders kunnen leveranciers voor een bepaalde tijdsperiode machtigen om bepaalde gegevens te beheren (bij te houden) namens de bronhouder. Dit ontslaat bronhouders niet
van de verantwoordelijkheid voor de basisgegevens.

#### Gegevens aanpassen kan makkelijk en goed

[DSO-04](#dso-04), [DSO-05](#dso-05), [DSO-06](#dso-06), [SDOW-12](#sdow-12), [CG-02](#cg-02), [CG-04](#cg-04)

Om kwalitatief goede gegevens te waarborgen, zorgt de registratie capability ervoor dat de daarvoor noodzakelijke "controles bij de poort" snel en automatisch worden uitgevoerd. 
Daarmee wordt het mogelijk om het aanpassen van de gegevens goed en snel uit te voeren. Degene die de aanpassing uitvoert blijft verantwoordelijk dat het een goede aanpassing 
van gegevens betreft, want de registratie capability heeft geen inhoudelijke kennis. 

De registratie capability biedt geen toegang tot bestaande gegevens. Dit zou de snelheid, betrouwbaarheid en flexibiliteit van de capability verminderen.

Om bestaande gegevens en nieuwe gegevens in samenhang te gebruiken, wordt daarom de standaard toegang capability benut voor de bestaande gegevens. Bij het aanpassen van gegevens is het vaak nodig om bestaande gegevens en nieuwe gegevens in samenhang te gebruiken, zodat de context duidelijk is en de verandering van gegevens op juistheid kan worden beoordeeld. De registratie capability en de toegang capability bieden samen de mogelijkheid om gegevens makkelijk aan te passen. 

Speciale aandacht is nodig voor de automatische controles aan de poort die de samenhang van de geografische gegevens borgen. Een belangrijke eis (met grote technische 
consequenties) is dat een vlakdekkende en naadloos op elkaar aansluitende opdeling in topografische objecten (op "maaiveld") en in eigendomspercelen wordt geborgd. Een tweede belangrijke eis is dat de verbondenheid van topologische netwerken (wegen, waterwegen, spoorwegen) wordt geborgd.

Uitwerking van deze borging met behoud van de mogelijkheid om makkelijk, goed en snel genoeg gegevens aan te passen is een hoofdzaak.

#### Gebruikers en bronhouders werken samen aan de kwaliteit van gegevens

[DSO-01](#dso-01), [DSO-10](#dso-10), [CG-02](#cg-02), [CG-04](#cg-04), [CG-05](#cg-05)

Gebruikers (Afnemers) en Bronhouders werken samen om de gewenste gegevenskwaliteit te kunnen behalen en borgen.

Kwaliteit van gegevens betekent enerzijds voldoen aan specificaties en vereisten, maar anderzijds vooral voldoen aan verwachtingen van gebruikers. 
Verwachtingen veranderen in de tijd en zijn verschillend per groep van gebruikers. Daarom is het essentieel dat er contact is tussen gebruikers en bronhouders van dezelfde 
gegevens. Als zij er samen aan werken om die gegevens voor iedereen bruikbaar te maken en houden, neemt de kwaliteit en daarmee de waarde van de gegevens toe.
Een capability om makkelijk te kunnen samenwerken is daarom noodzakelijk om aan veranderende kwaliteitscriteria invulling te geven. (NB de BRT gebruikersgroep van het BRT DevOps 
team is een voorbeeld).
Afnemers kunnen (veranderde) kwaliteitscriteria aan bronhouders leveren om een hogere waarde van de gegevens te bereiken. 
Als allen het eens zijn, kunnen nieuwe kwaliteitscriteria aan de vereiste kwaliteit worden toegevoegd. 

Om de vereiste en gespecificeerde kwaliteit van gegevens te kunnen waarborgen, zorgt de registratie capability dat de daarvoor noodzakelijke 
"controles bij de poort" worden uitgevoerd. 

Als kwaliteitscriteria wijzigen is controle over de reeds vastgelegde (geregistreerde) objecten ook nodig.
Reguliere interne controles om te controleren of geregistreerde gegevens (nog) aan de (eventueel in de tijd aangepaste) kwaliteitscriteria voldoen kunnen nodig zijn om de 
kwaliteit te borgen. Een "algoritme"capability kan hieraan invulling geven.

#### Basisgegevens zijn zo actueel en volledig als redelijkerwijs mogelijk

[DSO-04](#dso-04), [CG-03](#cg-03), [CG-04](#cg-04)

Basisgegevens zijn een beperkte set gegevens. Er zijn heldere criteria voor wat een basisgegeven is en wat niet. Hetzelfde geldt voor de actualiteit en volledigheid van 
basisgegevens.
Er zijn daarom basisgegevens waarvoor stricte controle op volledigheid en actualiteit wordt geautomatiseerd. Er zijn ook basisgegevens waarvoor minder stricte automatische 
controles plaatsvinden, zoals bijvoorbeeld het teruggeven van een waarschuwing bij de registratie van een gegeven dat in strijd is met niet-verplichte validatieregels 
(bijvoorbeeld in een proefperiode voorafgaand aan invoering van nieuwe criteria).  

De registratie capability voorziet in de mogelijkheid waarschuwingen (Warnings) te geven.

De registratie capability voorziet in de mogelijkheid (vooraf) te controleren tegen validatieregels zonder een gegeven daadwerkelijk te registreren.

#### Gegevens passen bij elkaar: relaties tussen gegevens zijn voor gebruikers duidelijk, en gegevens zijn in samenhang bruikbaar

[DSO-02](#dso-02), [SDOW-03](#sdow-03), [SDOW-04](#sdow-04), [CG-04](#cg-04)

Komende van verschillenden gegevens-sets (BAG, BGT, BRT, BRK, BRO, WOZ, enz) en gaande naar een Samenhangende Objecten Registratie is
het van essentieel belang dat er een bruikbaar samenhangend model van gegevens en objecten beschikbaar wordt gesteld. De "catalogus"-capability voorziet enerzijds in een voor 
mensen leesbare en duidelijke structuur, met definities en relaties. Anderzijds biedt de "catalogus"-capability in een voor machines leesbare vorm een eenduidige 
gegevensstructuur met definities en relaties.  

#### De gegevensstructuur kan snel genoeg meegroeien met de gebruiksbehoefte

[DSO-02](#dso-02), [DSO-03](#dso-03), [DSO-05](#dso-05)

Belangrijke is het om een basisset objecten te maken, maar even belangrijk, zo niet belangrijker is het dat de objectenstructuur flexibel is. Een attribuut of eigenschap moet 
gemakkelijk toe te voegen zijn aan een object. Of weggehaald als het niet meer nodig is.

De gegevensstructuur van de objecten moet meegroeien met de gebruikersbehoefte. Attributen die nu via een externe koppeling worden gekoppeld aan bijvoorbeeld een gebouw, moeten 
kunnen 'promoveren' tot onderdeel van de samenhangende basisregistratie objecten. Daarom biedt de "catalogus"-capability, die duidelijkheid biedt over de gegevensstructuur,  
periodiek een nieuwe versie aan. Afnemers en gebruikers van die capability moeten "meegroeien" door periodiek nieuwe versies over te nemen.      
