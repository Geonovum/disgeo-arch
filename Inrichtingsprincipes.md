## Inrichtingsprincipes voor de Objectenregistratie

### Context

In dit hoofdstuk worden de inrichtingsprincipes die van toepassing zijn op de Samenhangende Objecten Registratie 
bepaald. Er is voor gekozen om als uitgangspunt de [Overall Globale Architectuur Schets (OGAS)](https://aandeslagmetdeomgevingswet.nl/publish/library/219/dso_-_gas_-_overall_gas_1.pdf), 
die is opgesteld ten behoeve van de Omgevingswet te gebruiken. Dit omdat in deze OGAS reeds een toets is 
gedaan met de architectuurprincipes van diverse andere richtinggevende principes zoals [NORA](#basisprincipes-nora), [GEMMA](#inrichtingsprincipes-gemma), [Common Ground](#inrichtingsprincipes-common-ground), enz.
Daarmee wordt voorkomen dat er dubbel werk wordt gedaan, en wordt voorkomen dat er weer een afwijkende set van principes 
wordt opgesteld. Behalve naar de bestaande principes is ook gekeken naar de architectuurprincipes van W3C, en dan met 
name naar de principes uit [Spatial Data on the Web Best Practices](https://www.w3.org/TR/sdw-bp/#bp-summary)

### Doel van de samenhangende Objecten Registratie (SOR)

In de beleidsvisie wordt een vijftal doelstellingen geformuleerd:

| Doel |	Omschrijving                                                                           |
|------|-----------------------------------------------------------------------------------------|
| 01	  | Een betrouwbare, consistente en actuele samenhangende gegevensset voor heel Nederland;  |  
| 02   | Een efficiëntere inwinning en bijhouding van objecten, ook in drie dimensies (3D);      | 
| 03   | Een betere inpassing in moderne architecturen;                                          | 
| 04   | Meer en eenvoudiger gebruik van deze informatie in maatschappelijke toepassingen. De registratie gedraagt zich voor de gebruiker als één registratie;  |
| 05   | De objectenregistratie maakt onderdeel uit van een robuuste geo-informatie infrastructuur binnen de generieke digitale infrastructuur en voldoet aan de [12 eisen voor een basisregistratie](# eisen-aan-basisregistraties-GEMMA)  |

In de kern gaat het hierbij om een nadrukkelijke scheiding van de vastlegging van de gegevens, en de functionaliteiten die 
nodig zijn voor het bewerken, opvragen en het presenteren van deze gegevens tot logische informatie. 

Bron: https://www.geobasisregistraties.nl/documenten/beleidsnota/2019/11/29/beleidsvisie-samenhangende-objectenregistratie  

### Doel van de Inrichtingsprincipes

Het doel van deze inrichtinsprincipes is te zorgen en te borgen dat de Architectuur van de SOR voldoet aan de relevante principes.
Gekeken wordt naar de principes van reeds bestaande registraties (zoals NORA, GEMMA, enz) maar er wordt ook gekeken
naar de principes die zijn gekomen uit eerdere rapporten en onderzoeken (zoals DiS Geo en Common Ground) en
beschrijft hoe worden toegepast in de Objectenregistratie Architectuur. 
Er wordt vooral gekeken naar nieuwere principes om een vernieuwing door te kunnen voeren. Zouden wij enkel en alleen focussen op bestaande principes dan is het gevaar dat we "nieuwe wijn in oude zakken" stoppen.

#### Inrichtingsprincipes Digitaal Stelsel Omgevingwet

Aan de kolommen met de regel en principe zijn twee kolommen toegevoeg: Data en Functies.  
Data: Een *ja* in deze kolom moet worden gezien als 'Ja' dit principe is relevant voor de gegevens van de Samenhangende objectenregistratie. Scope zijn de gegevens zelf, oftwel het hart van het systeem.  
Functies: Een *ja* in deze kolom moet worden opgevant als 'Ja' dit principe is relevant voor de functionaliteit van de Samenhangende Objectenregistratie. Scope is de fuctionaliteit waarmee de gegevens en/of de informatie aan de gebruikers (afnemers en bronhouders)

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
| <p id='dso-10'>10</p> | Beheerfunctionaliteit is primaire functionaliteit                        |      |          |

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
| <p id='cgr-01'>01</p> | COMPONENTGEBASEERD: We werken met componenten                                     |
| <p id='cgr-02'>02</p> | OPEN: We zijn transparant waar mogelijk                                           |
| <p id='cgr-03'>03</p> | VERTROUWD: We zorgen dat informatiebeveiliging en privacy op orde zijn            |
| <p id='cgr-04'>04</p> | EENMALIGE VASTLEGGING: We leggen gegevens eenmalig vast en vragen op bij de bron  |
| <p id='cgr-05'>05</p> | REGIE OP GEGEVENS: We faciliteren regie op gegevens                               |
| <p id='cgr-06'>06</p> | STANDAARD:We standaardiseren maximaal                                             |

Bron: [Common Ground](https://www.gemmaonline.nl/images/gemmaonline/c/c7/20190130_-_Common_Ground_-_Informatiearchitectuurprincipes.pdf)


### inrichtingsprincipes voor DisGeo

In de paragrafen hieronder staan de principes en uitgangspunten die voor DisGeo belangrijk zijn. Per principe is aangegeven aan welke van de 
hiervoor genoemde principes invulling wordt gegeven.

#### Basisgegevens zijn van en voor iedereen

[DSO-01](#dso-01), [DSO-02](#dso-02), [DSO-04](#dso-04), [DSO-06](#dso-06), [SDOW-01](#sdow-01), [SDOW-02](#sdow-02), [SDOW-03](#sdow-03), [SDOW-12](#sdow-12)

Basisgegevens met identificatie, metadata basisclassificatie, locatie, geometrie
Basisgegevens hebben een altijd een *unieke sleutel* [SDOW-01](#sdow-01), deze wordt gebruikt om dat te kunnen koppelen. Daarnaast
hebben basisgegevens *identificerende kenmerken*, waarmee de objecten door mensen herkend kunnen worden. Zo is een woonadres iets dat door mensen
begrepen wordt, maar juist voor machine koppelingen voor allerlei problemen zorgt (adresproblematiek met verschillende schrijfwijzen).

Het is aan te raden ook een *eigenaarskenmerk* op te nemen bij objecten in de basisregistratie. hiermee is meteen duidelijk wie er
verantwoordelijk is voor de data. Soms wordt ook een *beheerderkenmerk* opgenomen, daarmee wordt het mogelijk om verschil te maken tussen
de eigenaarsrol en de beheerderrol.

Verder bevatten objecten in de registratie een *geldigheidsdatum*, van- en totdatum. Deze wordt gebruikt voor 'tijdreizen', maar ook voor archiveringsdoeleinden.

De unieke sleutel is sowiso belangrijk voor de basisregistratie. Immers we willen kunnen aanhaken met andere registraties op de 
objecten in de basisregistratie(s). Als we nu meteen kiezen voor een sleutel die aan de URI strategie voldoet, maken we een grote stap 
voorwaarts, en kunnen we webtechnologie gebruiken om de objecten in de registraties vindbaar en (mens en machine)ontsluitbaar te maken.

#### Basisgegevens zijn laagdrempelig beschikbaar en bruikbaar voor iedereen

[DSO-01](#dso-01), [DSO-02](#dso-02), [SDOW-02](#sdow-02), [SDOW-02](#sdow-03), [SDOW-12](#sdow-12)

Om basisgegevens voor iedereen beschikbaar en bruikbaar te maken moeten ze ook vindbaar zijn! De vindbaarheid wordt vergroot
als de basisgegevens vindbaar zijn via zoekmachines. Dat betekent dat er naast de "echte" data ook metadata nodig is.

#### Basisgegevens voldoen aan vereisten

[DSO-03](#dso-03),[DSO-05](#dso-05),[DSO-06](#dso-06), [CGR-01](#cgr-01), [CGR-03](#cgr-03)

Als data de brandstof is voor het systeem, moet deze ook betrouwbaar zijn. En betrouwbare data betekent vooraf vastgelegde
eisen: immer wanneer is de data betrouwbaar, aan welke criteria moet het voldoen. Door de data "open" te stellen creeer je een situatie
waarbij er veel mensen (en machines) de data gebruiken, en daarbij impliciet controleren. Een goede terugmeld mogelijkheid is dan
noodzakelijk, inclusief de feedback aan de melder! 

#### Bronhouders zijn verantwoordelijk voor basisgegevens

[DSO-10](#dso-10), [CGR-04](#cgr-04), [CGR-05](#cgr-05)

Bronhouders zijn en blijven te allen tijde verantwoordelijk voor de basisgegevens. Verantwoordelijk voor de vastlegging,
maar ook voor de kwaliteit en het beschikbaar stellen aan de afnemers. 


#### Bronhouders kunnen leveranciers machtigen

[DSO-10](#dso-10), [CGR-04](#cgr-04)

Bronhouders kunnen leveranciers machtigen om de gegevens bij te houden en/of te verwerken. Dit ontslaat hen echter niet
van de verantwoordelijkheid voor de basisgegevens.

#### Gegevens aanpassen kan makkelijk en goed

[DSO-04](#dso-04), [DSO-05](#dso-05], [DSO-06](#dso-06), [SDOW-12](#sdow-12), [CGR-02](#cgr-02), [CGR-04](#cgr-04)

Om kwalitatief goede gegevens te kunnen waarborgen, moet de registratie capability ervoor zorgen dat er zoveel mogelijk 
"controles bij de poort" worden gedaan. Ook moeten er regulier metingen gedaan worden die controleren of de gegevens
nog steeds aan de (eventueel strakker gezette) criteria voldoen. Daarmee moet echter het aanpassen van de gegevens
niet worden bemoeilijkt. Elke bronhouder moet in staat zijn om gegevens snel aan te passen. Vooral ook zodra er een
terugmelding is van geconstateerde fouten in de gegevens. 

#### Gebruikers en bronhouders werken samen aan de kwaliteit van gegevens

[DSO-01](#dso-01), [DSO-10](#dso-10), [CGR-02](#cgr-02), [CGR-04](#cgr-04), [CGR-05](#cgr-05)

Gebruikers (Afnemers) en Bronhouders moeten samenwerken om de gewenste gegevens kwaliteit te kunnen halen en borgen.
Afnemers kunnen een set aan kwaliteitscriteria aan de bronhouders leveren. Daarmee wordt de eerder genoemde controle aan
de poort gevoed. Kwaliteitscriteria kunnen wijzigen, dus controle over de reeds vastgelegde (geregistreerde) objecten
is ook nodig.

#### Basisgegevens zijn zo actueel en volledig als redelijkerwijs mogelijk

[DSO-04](#dso-04), [CGR-03](#cgr-03), [CGR-04](#cgr-04)

HEt is belangrijk om ons te realiseren dat we niet moeten doorslaan in het vastleggen van van-alles-en-nog-wat bij de 
basisgegevens. Er moeten heldere criteria komen voor wat een basisgegeven is, en wat niet. Een goede kosten/baten analyse
is op zijn plaats: Wat kost het om dit gegeven bij te houden, en wat levert het op?

#### Gegevens passen bij elkaar: relaties tussen gegevens zijn voor gebruikers duidelijk, en gegevens zijn in samenhang bruikbaar

[DSO-02](#dso-02), [SDOW-03](#sdow-03), [SDOW-04](#sdow-04), [CGR-04](#cgr-04)

Komende van verschillenden gegevens-sets (BAG, BGT, WOZ, enz) en gaande naar een Samenhangende Objecten Registratie is
het van belang dat er een goed gegevens en objecten model wordt gemaakt. Belangrijke is het om een basisset te maken,
maar even belangrijk, zo niet belangrijker is het dat de objecten flexibel zijn. Een attribuut moet gemakkelijk toe te voegen
zijn aan een object. Of weggehaald als het niet meer nodig is...

#### De gegevensstructuur kan snel genoeg meegroeien met de gebruiksbehoefte

[DSO-02](#dso-02), [DSO-03](#dso-03), [DSO-05](#dso-05)

zoals hiervoor ook al gezegd, de gegevensstructuur van de objecten moet meegroeien met de gebruikers behoefte.
Attributen die nu via een extere koppeling worden gekoppeld aan bijvoorbeeld een gebouw, moeten kunnen 'promoveren' tot 
onderdeel van de basisregistratie objecten!

