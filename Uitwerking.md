## Uitwerking

### Inleiding

**Dit hoofdstuk bevat de uitwerking van de componenten van de objectenregistatie.**

Per component is eerst beschreven wat het doel is van de component. 
Vervolgens wordt aangegeven:
1.  Op welke bestaande uitwerkingen de invulling van de component is gebaseerd.
2.  Welke uitgangspunten, zoals bestaande standaarden, voor de invulling van de component gelden.
3.  Aan welke vereisten de component dient te voldoen.
4.  Welke externe afhankelijkheden de component heeft.

De uitwerking van de componenten is zoveel als mogelijk gebaseerd op bestaande, breed geaccepteerde en gehanteerde nationale of internationale uitwerkingen.

De uitwerking van de componenten is een functionele uitwerking die meerdere technische invullingen mogelijk maakt. Technische keuzes worden alleen voorgeschreven als ze essentieel zijn, bijvoorbeeld keuzes voor technische standaarden in het kader van interoperabiliteit en het voldoen aan afspraken binnen de overheid of nationale of internationale afspraken.

Onder [Algemeen](#algemeen) beschrijven we de onderwerpen die op meerdere plaatsen
in de architectuur voorkomen. Deze onderwerpen zijn daar eenmalig
uitgewerkt.

### Laag Uitvoering

Onderstaande afbeelding toont de clusters van functionaliteiten op de laag Uitvoering. Deze clustering is een functionele indeling, geen technische. Het groepeert functies die bijdragen aan hetzelfde doel.

<figure id="functiesuitvoering">
    <img src="media/inrichting-uitvoering-objectenregistratie.png" alt="inrichting uitvoering">
    <figcaption>De capabilities op de laag Uitvoering</figcaption>
</figure>

De laag **Uitvoering** bevat de functies voor het beheren van objectgegevens en voor het afnemen van objectgegevens
Algemene onderwerpen zoals Toegang en Interactie zijn uitgewerkt in het onderdeel Algemeen.

#### Registratie

De component Registratie heeft als doel om bronhouderorganisaties en gemachtigde organisaties in staat te
stellen objectgegevens en bijbehorende meta-gegevens te beheren (toevoegen en
wijzigen). Deze component biedt de services die bronhouders en gemachtigden daarvoor nodig
hebben.

De component Registratie biedt services voor informatiesystemen om
objectgegevens te beheren (toevoegen en wijzigen). 

Deze component bevat geen functionaliteit voor interactie en presentatie. 

**Invulling**

De uitwerking van deze component is onder andere gebaseerd op:

-   Voor geo-gegevens: [OGC API - Features - Part 4: Simple Transactions](http://docs.opengeospatial.org/DRAFTS/20-002.html)  
   
-   Voor administratieve gegevens: [API-strategie](https://docs.geostandaarden.nl/api/API-Strategie/)

Bovenstaande twee uitwerkingen bieden geen volledige basis voor de uitwerking
van de component Registratie, maar bij de auteurs zijn geen andere uitwerkingen
bekend die als basis kunnen dienen.

In het kader van OGC API – Features wordt gewerkt aan meer Parts. Op een later
moment wordt bepaald of deze basis vormen voor de uitwerking van de componenten.

In het kader van het GEMMA Gegevenslandschap, Common Ground en kennisplatform
API’s wordt gewerkt aan API-criteria. Op een later moment wordt bepaald of deze
basis vormen voor de uitwerking van de componenten.

In het kader van het GEMMA Gegevenslandschap en Common Ground is een uitwerking
beschikbaar van logging en registratie van verwerking van gegevens. In hoeverre
die uitwerking van toepassing is op de component Registratie moet nog worden
bepaald.

**Uitgangspunten**

Voor de uitwerking van de component gelden de volgende uitgangspunten:

-   Geen uitgangspunten.

**Vereisten**

Voor deze component gelden de volgende vereisten:

1.  Bij elke toevoeging of wijziging van een gegeven vindt vooraf validatie aan de
    gegevensregels plaats. Alleen valide gegevens worden geregistreerd. 

2.  Van iedere gegevenswijziging wordt tenminste vastgelegd: 
    welk gegeven is geregistreerd of gewijzigd, 
	de identificatie van het geregistreerde of gewijzigde object, 
	de organisatie die de wijziging heeft gedaan, 
	de voor de wijziging gebruikte dienst, 
	datum en tijdstip van registratie van de wijziging.

3.  Van ieder gebruik van een registratiedienst wordt tenminste vastgelegd: 
	datum en tijdstip van gebruik, 
	organisatie die gebruikt, 
	zodat een audit log beschikbaar is. 

N.B.

-   Gegevens worden niet verwijderd. Een beëindiging wordt geimplementeerd als een wijziging (het invullen van een einddatum of het markeren als verwijderd o.i.d.)
-   Het vastleggen en beheren van gegevensregels valt binnen de component Gegevenscatalogus en niet binnen de component Registratie.

**Externe afhankelijkheden**

Deze component heeft de volgende externe afhankelijkheden:

-   Geen externe afhankelijkheden.

#### Opslag

De component Opslag heeft als doel het duurzaam beschikbaar houden van
objectgegevens en bijbehorende metagegevens, zodat bronhouders deze gegevens
kunnen beheren en zodat de gegevens beschikbaar zijn voor de verstrekker zodat
deze ze kan verstrekken aan afnemers in de vorm van gegevens of daarvan
afgeleide informatieproducten.

**Invulling**

De uitwerking van deze component is onder andere gebaseerd op:

-   Er zijn geen nationale of internationale standaarden of andere uitwerkingen
    om de opslag-component op te baseren.

**Uitgangspunten**

Voor de uitwerking van de component gelden de volgende uitgangspunten:

-   De opslag-component is een intern onderdeel dat alleen via services
    is te benaderen. Het is daarom niet nodig om hiervoor een standaard invulling te
    hanteren. De technische wijze van opslag is verantwoordelijkheid van de
    uitvoeringspartij die dit invult.

**Vereisten**

Voor deze component gelden de volgende vereisten:

1.  De gegevens in de opslag voldoen aan het informatiemodel van de objectenregistratie en de
    eisen aan duurzaamheid en toegankelijkheid.

2.  De opslag bevat alle gegevens die nodig zijn om de bronhouders
    objectgegevens te kunnen laten beheren en om deze gegevens beschikbaar te
    maken voor de verstrekker.

3.  Door het scheiden van proceslogica van procesgegevens en gegevens zal de
    opslag naast objectgegevens ook procesgegevens moeten omvatten. Denk aan
    het bijhouden wie welke wijzigingen heeft doorgevoerd en wanneer. Procesgegevens worden samen met de gegevens opgeslagen.

4.  Procesgegevens verzorgen het opbouwen van de audit trial.

5.  De opslag is enkel en alleen benaderbaar via services.

6.  De opslag maakt data-portabiliteit mogelijk. De gegevens moeten met beperkte
    inspanning overgezet kunnen worden naar een ander opslagmechanisme.

**Externe afhankelijkheden**

Deze component heeft de volgende externe afhankelijkheden:

-   Externe eisen aan informatieveiligheid zoals Baseline Informatiebeveiliging Overheid (BIO).

#### Afname

De component Afname heeft als doel om afnemers in staat te stellen
objectgegevens en daarvan afgeleide informatieproducten af te nemen, zodat ze
deze gegevens en informatie kunnen gebruiken in hun eigen processen. Deze
component biedt toegang tot alle voor afnemers beschikbare objectgegevens,
inclusief meta-gegevens, en tot alle door de objectenregistratie beschikbaar gestelde
informatieproducten.

We onderscheiden geen aparte componenten voor afname van gegevens en voor afname
van informatie omdat de uitwerking van beide hetzelfde is en omdat het
onderscheid tussen gegevens en informatie niet eenduidig is te maken.

De component Afname biedt services voor informatiesystemen om objectgegevens en
informatieproducten af te nemen. De component bevat geen functionaliteit voor
het presenteren van deze gegevens of informatie aan gebruikers in bijvoorbeeld
een viewer. Daarvoor zijn aparte interactiecomponenten nodig die gebruik maken
van de services van de component voor Afname van Gegevens en Informatie.

**Invulling**

De uitwerking van deze component is onder andere gebaseerd op:

-   Voor geo-gegevens: [OGC API - Features - Part 1: Core](http://docs.opengeospatial.org/DRAFTS/17-069r2.html)  
    N.B.: dit is een draft en nog geen vastgestelde standaad.

-   Voor administratieve gegevens: [API-strategie](https://docs.geostandaarden.nl/api/API-Strategie/)

Bovenstaande twee uitwerkingen bieden geen volledige basis voor de uitwerking
van de component Afname, maar bij de auteurs zijn geen andere uitwerkingen
bekend die als basis kunnen dienen.

In het kader van OGC API – Features wordt gewerkt aan meer Parts. Op een later
moment wordt bepaald of deze basis vormen voor de uitwerking van de
componenten.

In het kader van het GEMMA Gegevenslandschap, Common Ground en kennisplatform
API’s wordt gewerkt aan API-criteria. Op een later moment wordt bepaald of deze
basis vormen voor de uitwerking van de componenten.

In het kader van het GEMMA Gegevenslandschap en Common Ground is een uitwerking
beschikbaar van logging en registratie van verwerking van gegevens. In hoeverre
die uitwerking van toepassing is op de component Afname van Gegevens en
Informatie moet nog bepaald worden.

**Uitgangspunten**

Voor de uitwerking van de component gelden de volgende uitgangspunten:

-   Geen uitgangspunten.

**Vereisten**

Voor deze component gelden de volgende vereisten:

1.  Gegevens en informatie zijn alleen te benaderen via services. Daarom worden
    in ieder geval alle dataservices geboden die nodig zijn om alle beschikbare
    gegevens en informatie te kunnen afnemen (in de API-strategie worden
    dataservices systeemservices genoemd).

2.  Naast dataservices biedt deze component ook gemaks- en processervices voor
    zover deze onderdeel zijn van het portfolio van de objectenregistratie.

3.  Functionaliteit voor het samenstellen van informatie uit objectgegevens
    maakt altijd gebruik van de services voor afname van objectgegevens.

4.  Van ieder gebruik van een afnamedienst wordt o.a. vastgelegd: datum en
    tijdstip, organisatie. Dit kan o.a. gebruikt worden om te meten of het
    gebruik binnen de overeengekomen grenzen van gebruik blijft. Bijvoorbeeld
    grenzen aan ‘fair use’ voor open diensten en grenzen aan gebruik van
    diensten met gegarandeerd dienstenniveau en grenzen aan gebruik van
    eventuele betaalde diensten.

<p class ='note'>
    Vraag aan de reviewers om argumenten voor of tegen de vereiste dat
    bovenliggende services altijd gebruik dienen te maken van dataservices. En of
    daarbij onderscheid gemaakt dient te worden tussen registratieservices en
    afnameservices.
</p>

**Externe afhankelijkheden**

Deze component heeft de volgende externe afhankelijkheden:

-   Geen externe afhankelijkheden

##### Afgeleide opslag

Functioneel gezien is er een Opslag.

Ten behoeve van afname van gegevens en informatie is naar verwachting in de technische uitwerking afgeleide
opslag nodig. Dit is **geen** zelfstandige component, maar een onderdeel van Afname van gegevens en informatie.

Ten behoeve van betrokkenen bij de functionaliteit Afname worden hier uitgangspunten en vereisten aan afgeleide opslag beschreven.

Afgeleide opslag heeft als doel om te voorzien in opslag van objectgegevens en
bijbehorende meta-gegevens die is afgestemd op de specifieke eisen van de afname
van objectgegevens door afnemers. Voor de afnemers is het niet relevant te weten waar of hoe de gegevens zijn opgeslagen, toegang tot de gegevens wordt immers enkel via dataservices geboden. 

Afgeleide opslag is de opslag die is afgestemd op de taken en
verantwoordelijkheden van de verstrekkingsfunctie voor de objectenregistratie. De grootte van de
afnemersgroep, het grote aantal afnames, de daarbij horende prestatie-eisen en
ook de behoefte aan diverse vormen van afname vragen om daarop afgestemde
technische opslagvormen.

Technische redenen voor afgeleide opslag zijn bijvoorbeeld performance eisen aan de afname. Denk bijvoorbeeld aan een "hot standby" om snel te kunnen zoeken (bijvoorbeeld hot standby in de vorm van linked data) of snel te kunnen in/uitzoomen en 'schuiven' (hot standby in de vorm van kaarttegeltjes) of snel massaal te kunnen afnemen (hot standby van vaakgevraagde gegevens of informatie (gegevenscombinaties) om, zeg, 1.000 bevragingen per seconde te bedienen) etcetera. 
Uitwerking van afgeleide opslag is dus een onderwerp in de architectuur van de betreffende service: de eis is en blijft dat nergens buiten de component Opslag gegevens 'leven' die als bron worden gebruikt zonder dat deze synchroon is met de gegevens in de Opslag.


**Invulling**

De uitwerking van Afgeleide Opslag is onder andere gebaseerd op:

-   Er zijn geen nationale of internationale standaarden of andere uitwerkingen
    om de afgeleide-opslag-component op te baseren.

Er zijn vele uitwerkingen en vormen van afgeleide opslag, bijvoorbeeld zoals
voor ‘business intelligence’. Er zijn, voor zover bekend, geen nationaal of
internationaal afgesproken vormen van afgeleide opslag.

De afgeleide opslag staat ten dienste van het verstrekken of afnemen van
objectgegevens en samenstellen en verstrekken van informatieproducten. Het is
met andere woorden een intern gerichte functie. We beschrijven daarom hier
vooral de vereisten aan de afgeleide opslag waar de invulling ervan aan moet
voldoen. 

**Uitgangspunten**

Voor de uitwerking van Afgeleide Opslag gelden de volgende uitgangspunten:

-   Uitgangspunt voor deze vereisten is dat het koppelvlak tussen de
    componenten Opslag en Afgeleide Opslag een intern koppelvlak is waarvoor
    geen vereisten gelden m.b.t. het gebruik van open, leveranciersonafhankelijke
    standaarden en technologieën.

**Vereisten**

Voor Afgeleide Opslag gelden de volgende vereisten:

1.  Afgeleide Opslag bevat altijd een kopie van de gegevens in de component
    Opslag. Er vindt geen bijhouding plaats in de Afgeleide Opslag anders dan
    via de Opslag.

2.  Synchronisatie van de Opslag naar Afgeleide Opslag zorgt ervoor dat de
    Afgeleide Opslag een kopie van de objectgegevens bevat die voldoet aan de
    actualiteitseisen voor verstrekking van gegevens en informatieproducten.

3.  Afgeleide Opslag bevat die gegevens die nodig zijn voor verstrekking van
    gegevens, voor het samenstellen en verstrekken van informatieproducten en
    voor het synchroon houden van de Afgeleide Opslag met de Opslag.

4.  Indien nodig kunnen meerdere vormen van afgeleide opslag naast elkaar
    bestaan. Alle vormen van afgeleide opslag voldoen aan de hier beschreven
    vereisten.

**Externe afhankelijkheden**

Afgeleide Opslag heeft de volgende externe afhankelijkheden:

-   Geen externe afhankelijkheden

#### Notificatie

De component Notificatie heeft als doel om afnemers op de hoogte te stellen van
voor hen relevante gebeurtenissen die betrekking hebben op objectgegevens, zodat
zij kunnen handelen naar die gebeurtenissen.

Notificeren over gebeurtenissen past binnen het concept van eenmalige
vastlegging en meervoudig gebruik. Binnen de gegevensuitwisseling zoals die in
de gemeenschappelijke overheidsarchitectuur (GO) is voorzien, is de capability
van notificeren een uitgangspunt. Het sluit aan op de visie van het GEMMA
Gegevenslandschap en Common Ground zoals gemeenten en andere overheden die nu
vormgeven en is complementair aan de Haal Centraal gedachte. Een
Gebeurtenisgedreven Architectuur heeft onder meer notificaties nodig, omdat
daarmee aan afnemers kennis wordt gegeven van een gebeurtenis die heeft geleid
tot een wijziging van een object. Voor afnemers kunnen deze gewijzigde gegevens
van belang zijn afhankelijk van de eigen processen en eerder gebruik van die
gegevens.

**Invulling**

De uitwerking van deze component is onder andere gebaseerd op:

-   Er is nog geen uitwerking beschikbaar om de component Notificatie op te
    baseren.

Ministerie van BZK, Kadaster en VNG en anderen werken aan een uitwerking van notificatie en
abonnementen. Op een later moment wordt bepaald of deze basis vormt voor de
uitwerking van de component Notificatie van de objectenregistratie.

Ook de volgende uitwerkingen vormen mogelijk een basis voor de uitwerking van de
component Notificatie. Dat is nader te bepalen:

-   Uitwerking van event-sourcing door Haal Centraal.
-   BRK-meldingen van het Kadaster.

**Uitgangspunten**

Voor de uitwerking van de component gelden de volgende uitgangspunten:

-   Geen uitgangspunten.

**Vereisten**

Voor deze component gelden de volgende vereisten:

1.  Afnemers die zich hebben geabonneerd op gebeurtenissen worden actief
    genotificeerd. Er is actieve publicatie van gebeurtenissen naar
    abonnementhouders. Of hiervoor een pull of push mechanisme wordt gehanteerd
    is later te bepalen.

2.  Register van (genotificeerde) gebeurtenissen is geen vereiste. Afnemers kunnen historie van gegevens raadplegen om te voorzien in de behoefte aan inzicht in opgetreden gebeurtenissen. 
	Immers, afnemen van historie is voldoende als de gegevens zelfbeschrijvend zijn.
	Het is later te bepalen of een gebeurtenissenregister toegevoegde waarde biedt voor afnemers.

3.  Er zal standaardisatie van gebeurtenissen zijn.

4.  Of notificaties ook (oude en nieuwe) objectgegevens bevatten is nader te
    bepalen.

**Externe afhankelijkheden**

Deze component heeft de volgende externe afhankelijkheden:

-   Geen externe afhankelijkheden

Afhankelijk van de ontwikkelingen van overheidsbrede afspraken en voorzieningen
met betrekking tot notificeren en abonneren ontstaan er mogelijk in de toekomst
afhankelijkheden naar gemeenschappelijke voorzieningen hiervoor, vergelijkbaar
met de bestaande voorziening Digilevering.

#### Terugmelding

De component Terugmelding heeft als doel dat meldingen van afnemers over de
juistheid van gegevens geregistreerd kunnen worden en beschikbaar zijn voor
bronhouders, zodat zij ze kunnen behandelen.

Overheidspartijen die verplicht gebruik maken van basisregistraties hebben een
terugmeldplicht. Zie [‘Eis 2: De afnemers hebben een terugmeldplicht’](https://www.digitaleoverheid.nl/overzicht-van-alle-onderwerpen/basisregistraties-en-stelselafspraken/stelsel-van-basisregistraties/twaalf-eisen-stelsel-van-basisregistraties/#Eis%202*.*)

Deze component biedt services waarmee afnemers twijfels over de juistheid van
gegevens kunnen melden bij de objectenregistratie. De component bevat geen functionaliteit voor
interactie met personen (geen terugmeldloket). Daarvoor zijn andere componenten
nodig, bijvoorbeeld vergelijkbaar met het huidige [‘Verbeter de kaart’](https://verbeterdekaart.kadaster.nl).

**Invulling**

De uitwerking van deze component is onder andere gebaseerd op:

-   Er zijn geen nationale of internationale standaarden of andere uitwerkingen
    om de opslag-component op te baseren.

**Uitgangspunten**

Voor de uitwerking van de component gelden de volgende uitgangspunten:

-   Voor deze component gaan we uit van de volgende werking. Een afnemer doet
    een terugmelding bij een gegeven (vanuit een eigen applicatie of via een
    terugmeldloket). Deze component zorgt ervoor dat deze terugmelding wordt
    geregistreerd en beschikbaar is voor bronhouders. Bronhouders zijn
    geabonneerd op terugmeldingen op de gegevens waar ze bronhouder voor zijn,
    zodat de juiste bronhouders worden genotificeerd. De bronhouders onderzoeken
    de terugmelding, wijzigen indien nodig de objectgegevens en werken de status
    van de terugmelding bij.

-   Een terugmelding op een gegeven is zowel een aanduiding bij een gegeven dat
    er twijfel over bestaat als een aanleiding voor de bronhouder van het
    gegeven om de terugmelding te onderzoeken. Vanuit de objectenregistratie vinden we dat de
    terugmelding niks anders is dan een aspect van het gegeven zelf waaruit
    blijkt dat er twijfel is over de juistheid ervan en dat het in onderzoek is.
    Hierdoor weten gebruikers dat bij dit specifieke gegeven iets aan de hand
    is. Dit is met name van belang indien dit gegeven wordt gebruikt in primaire
    werkprocessen, data-analyse, e.d.

-   De terugmelding wordt gerelateerd aan het gegeven waar het betrekking op
    heeft.

-   Een terugmelding bevat standaard gegevens zoals datum, tijd, terugmelder,
    e.d. zoals dat nu ook gebeurt.

-   Het onderzoeken van de terugmelding is de taak van de bronhouder. De
    ondersteuning hiervoor, zoals een zaaksysteem, valt buiten de scope van de
    voorzieningen van de objectenregistratie. Het resultaat van het onderzoek wordt geregistreerd
    in de objectenregistratie.

-   Een terugmelding kan betrekking hebben op 1 of meerdere bronhouders.

-   Het in onderzoek zijn is een gegeven waarop notificatie mogelijk is.

**Vereisten**

Voor deze component gelden de volgende vereisten:

1.  Eenieder kan terugmelden. Daarom kent de objectenregistratie een generieke interactiecomponent voor terugmelden. Een mens kan eventueel anoniem terugmelden.

2.  Terugmelden kan ook door een machine worden gedaan. Op basis van algoritmen
    kunnen de gegevens bij registratie maar ook periodiek of bij veranderingen
    in de gegevensstructuur gevalideerd worden. Bij validatie door een machine
    zal bij de terugmelding ook het algoritme vastgelegd worden.

3.  Er zijn services om terug te melden. De services maken het mogelijk om een
    terugmelding te registreren met een verwijzing naar het gegeven.

4.  Het is mogelijk om in bulk terug te melden.

**Externe afhankelijkheden**

Deze component heeft de volgende externe afhankelijkheden:

-   Er is een afhankelijkheid naar de generieke (toekomstige)
    terugmeldvoorzieningen zoals Digimelding en ‘Verbeter de kaart’ en de
    bijbehorende standaarden.

### Laag Inzicht

Onderstaande afbeelding toont de clusters van functionaliteiten op de laag Inzicht. Deze clustering is een functionele indeling, geen technische. Het groepeert functies die bijdragen aan hetzelfde doel.

<figure id="inrichting-inzicht">
    <img src="media/inrichting-inzicht-objectenregistratie.png" alt="inrichting inzicht">
    <figcaption>De capabilities op de laag Inzicht </figcaption>
</figure>
  
Op de laag **Inzicht** onderkennen we de volgende clusters: **Toegang**, **Gegevenscatalogus**, **Gegevenskwaliteit** en **Dienstencatalogus**. 

Algemene onderwerpen zoals Toegang en Interactie zijn uitgewerkt in het onderdeel Algemeen.

#### Gegevenscatalogus

De component Gegevenscatalogus heeft als doel om de in de objectenregistratie beschikbare
gegevens en informatieproducten te kunnen beschrijven en deze beschrijving te
ontsluiten, zodat bronhouders, afnemers en andere betrokkenen hier kennis van
kunnen nemen.

De gegevenscatalogus verbindt definities, toelichtingen en uitleg van begrippen,
waardelijsten en informatieproducten met elkaar. De gegevenscatalogus beschrijft
daarmee de inhoud van de gegevens en informatieproducten.

De uitwisselingsstandaarden en formaten om de gegevens en informatieproducten te
benaderen staan beschreven in de dienstencatalogus.

Voor het raadplegen van de gegevenscatalogus zijn applicaties of webloketten
nodig. Dit zijn zelfstandige interactiecomponenten. De aanname is dat de objectenregistratie ook
een interactiecomponent zal bieden om de gegevenscatalogus te raadplegen.

**Invulling**

De uitwerking van deze component is onder andere gebaseerd op:

-   Bestaande catalogi, zoals:

    -   De [Stelselcatalogus](https://stelselcatalogus.omgevingswet.overheid.nl/) van het stelsel van basisregistraties, Vanuit het stelsel
        van basisregistraties bestaat de verplichting om de stelselcatalogus te
        gebruiken. Deze heeft als doel om de begrippen tussen de
        basisregistraties te kunnen vergelijken. De stelselcatalogus beschrijft
        niet tot op het niveau van de waardenlijsten.

    -   Gegevenscatalogi van BAG, BGT, BRT, BRO, BRK en WOZ

**Uitgangspunten**

Voor de uitwerking van de component gelden de volgende uitgangspunten:

-   Geen uitgangspunten.

**Vereisten**

Voor deze component gelden de volgende vereisten:

1.  De gegevenscatalogus beschrijft definities, toelichting en uitleg van
    begrippen.

2.  De gegevenscatalogus beschrijft de relaties tussen de begrippen.

3.  De gegevenscatalogus beschrijft waardenlijsten waarbij elke waardenlijst een
    uitputtende opsomming van de mogelijke waarden voor dat begrip bevat.

4.  De gegevenscatalogus beschrijft definities, toelichting en uitleg van
    informatieproducten.

5.  De gegevenscatalogus bevat de wijzigingen zoals toevoegingen van begrippen,
    veranderingen van relaties, verandering van definities, etc. De
    versiegeschiedenis van de gegevenscatalogus blijft beschikbaar inclusief de
    doorgevoerde veranderingen. Op elk moment is duidelijke welke versie de
    geldige versie is.

6.  Met services kunnen de begrippen en definities worden opgevraagd uit de
    gegevenscatalogus.

7.  De objectenregistratie biedt een interactiecomponent (bijvoorbeeld een webloket) waar
    personen de gegevenscatalogus kunnen raadplegen en bevragen.

8.  De gegevenscatalogus heeft functionaliteit waarmee de stelselcatalogus en
    andere catalogi deze als een federatieve catalogus kunnen benaderen. Met
    andere woorden: de inhoud van de gegevens wordt op één plek bijgehouden,
    namelijk in de gegevenscatalogus.

9.  Gegevenscatalogus voldoet aan vereisten vanuit wetgeving zoals Europese INSPIRE wetgeving. 


**Externe afhankelijkheden**

Deze component heeft de volgende externe afhankelijkheden:

-   Er is een afhankelijkheid van de [stelselcatalogus basisregistraties](https://www.stelselcatalogus.nl/).


#### Gegevenskwaliteit

Het doel van de component Gegevenskwaliteit is om de afgesproken
kwaliteitsindicatoren vast te leggen, te meten en monitoren wat de waarde van
deze indicatoren is en zowel de indicatoren als de gemeten waarden beschikbaar
te stellen voor bronhouders, afnemers en andere betrokkenen, zoals
toezichthouders en beleidsverantwoordelijke.

De kwaliteitsmetingen helpen de bronhouders en afnemers en andere betrokkenen
(zoals toezichthouder en beleidsverantwoordelijke) met het krijgen van inzicht
en leveren tevens fouten en signalen op die de bronhouder kan gebruiken om de
gegevenskwaliteit te verbeteren.

Met kwaliteitsmetingen kan de gegevenskwaliteit beoordeeld worden tegen
vastgestelde kwaliteitsindicatoren. Het resultaat hiervan wordt inzichtelijk
gemaakt.

**Invulling**

De uitwerking van deze component is onder andere gebaseerd op:

-   Nader te bepalen.

De volgende uitwerkingen vormen mogelijk een basis voor de uitwerking van de
component Gegevenskwaliteit. Dat is nader te bepalen:

-   De opgedane kennis en ervaring vanuit de huidige kwaliteitsdashboards BAG en BGT.

-   Business Intelligence en Data Analytics kennis en ervaring van Data Science teams betrokken bij de BAG, BGT en BRT.


**Uitgangspunten**

Voor de uitwerking van de component gelden de volgende uitgangspunten:

-   De kwaliteitsindicatoren worden afgesproken met bronhouders, afnemers en
    andere betrokkenen en worden naar deze groepen transparant gemaakt.

-   Met kwaliteitsindicatoren kan de algehele kwaliteit van de opgeslagen
    gegevens gemonitord worden. De opslag bevat naast de feitelijke gegevens ook
    proces- en metagegevens (zie opslag). Dit betekent dat de
    kwaliteitsindicatoren naast de kwaliteit van de gegevens zelf ook resultaten
    kunnen geven over bijvoorbeeld gemiddelde duur van verwerking door bronhouder (procesgegevens)
    of meta-gegevens van de gegevens zelf.

-   Kwaliteitsdashboards zijn interactiecomponenten die inzicht geven in de kwaliteit van de gegevens.

**Vereisten**

Voor deze component gelden de volgende vereisten:

1.  De kwaliteitsindicatoren worden in business regels uitgewerkt.

2.  Elke business regel kan worden gekoppeld aan 1 of meer doelgroepen (niet
    elke kwaliteitsindicator is van toepassing is op elke doelgroep).

3.  De uitvoering van een business regel kan op elk moment plaatsvinden en geeft
    de uitkomst op basis van de indicator.

4.  De uitkomst is een fout of signaal (kan fout zijn).

5.  Een kwaliteitsmeting is de uitvoering van 1 of meerdere business regels.

6.  De uitvoering is reproduceerbaar over tijd.

    1.  De uitvoering van een business regel is een weergave van een indicator
        op een bepaalde tijd

    2.  De kwaliteitsmetingen hoeven niet apart te worden opgeslagen door de
        reproduceerbaarheid (of dit moet nodig zijn in verband met de tijd die
        nodig is voor een kwaliteitsmeting).

    3.  Reproduceerbaarheid leidt tot kwaliteitsmonitoring.

7.  Bepaald kan worden welke fouten en signalen een gegeven ‘in onderzoek’
    zetten.

Voor de kwaliteitsdashboards van de objectenregistratie gelden de volgende vereisten. Deze
moeten opgenomen bij de interactiecomponent Kwaliteitsdashboard op het moment dat die
component nader wordt uitgewerkt.

1.  Het kwaliteitsdashboard is een verschijningsvorm van de kwaliteitsmetingen.

2.  Het kwaliteitsdashboard geeft ook inzicht van de gegevens die ‘in onderzoek’
    zijn.

3.  Het kwaliteitsdashboard is in te richten op doelgroepen. Nationale weergave,
    nationale weergave bronhouders, nationale weergave afnemers, weergave per
    bronhouder, etc.

**Externe afhankelijkheden**

Deze component heeft de volgende externe afhankelijkheden:

-   Geen externe afhankelijkheden

#### Dienstencatalogus

De component Dienstencatalogus heeft als doel om de diensten van de
objectenregistratie te beschrijven en deze beschrijvingen (interactief) te
ontsluiten, zodat betrokkenen hier makkelijk en goed kennis van kunnen nemen.

Diensten zijn volgens een gestandaardiseerde beschrijfwijze beschreven en worden
middels een gemeenschappelijke gestandaardiseerde publicatiewijze aangeboden om
als een geheel te worden ervaren.

De uitwisselingsstandaarden en formaten om de gegevens en informatieproducten te
benaderen zijn, waar van toepassing, onderdeel van deze beschrijfwijze.

NB. De (structuur van de) inhoud van de gegevens en informatieproducten staat
beschreven in de gegevenscatalogus.

Voor afnemers van diensten wordt een overzicht geboden om te begrijpen welke
diensten beschikbaar zijn.

**Invulling**

De uitwerking van deze component is onder andere gebaseerd op inzichten die zijn
opgetekend door diverse architectuurgemeenschappen van samenwerkende
overheidsorganisaties zoals veiligheidsregio’s, omgevingsdiensten,
waterschappen, provincies, gemeentes en landelijke (uitvoerings-) organisaties.

Het [ontwikkelaarsportaal](https://aandeslagmetdeomgevingswet.nl/ontwikkelaarsportaal/) van het digitaal stelsel van de omgevingswet is een inspirerend voorbeeld. 

**Uitgangspunten**

Voor de uitwerking van de component gelden de volgende uitgangspunten:

-   De dienstencatalogus bevat naast de dienstenbeschrijvingen ook de van
    toepassing zijnde wetgeving, voorwaarden, (aanvraag)procedures,
    doorlooptijden en kosten.
-   De dienstencatalogus omvat een register van diensten die middels API’s
    (services) worden aangeboden.
-   Dit API-register voldoet aan de Nederlandse API-strategie

**Vereisten**

Voor deze component gelden de volgende vereisten:

-   De component Dienstencatalogus geeft makkelijk en goed toegang tot het
    actuele overzicht van beschikbare diensten en de beschrijvingen van de
    diensten.
-   Waar van toepassing bevat de dienstencatalogus een directe link naar de
    services waarop informatiesystemen kunnen aansluiten als organisaties voor
    die diensten een overeenkomst aangaan met de dienstaanbieder.
-   Voor afnemers van diensten biedt de beschrijving van het niveau van
    dienstverlening (service level) inzicht of de diensten geschikt zijn om de
    behoefte van de afnemer in te vullen.
-   Voor aanbieders en afnemers van diensten wordt een (volgende) versie van een
    dienst gepubliceerd voor, tijdens en eventueel na de beschikbaarheidsperiode
    van die versie van de dienst.
-   Diensten kunnen worden gepubliceerd op https://developer.overheid.nl/

**Externe afhankelijkheden**

Deze component heeft de volgende externe afhankelijkheden:

-   Er is een afhankelijkheid van vindbaarheid en toegankelijkheid van het
    overheid.nl domein voor dienstafnemers
-   Er is een afhankelijkheid van aanpasbaarheid en beheerbaarheid van het
    overheid.nl domein voor dienstaanbieders


### Laag Ondersteuning

Onderstaande afbeelding toont de clusters van functionaliteiten op de laag Ondersteuning. Deze clustering is een functionele indeling, geen technische. Het groepeert functies die bijdragen aan hetzelfde doel.

<figure id="functiesuitvoeringondersteuning">
    <img src="media/inrichting-ondersteuning-objectenregistratie.png" alt="inrichting ondersteuning">
    <figcaption>De capabilities op de laag Ondersteuning</figcaption>
</figure>

Op de **Ondersteuningslaag** onderkennen we de clusters voor de ondersteuning van bronhouders en hun gemachtigden en afnemers.
Algemene onderwerpen zoals Toegang en Interactie zijn uitgewerkt in het onderdeel Algemeen.

#### Abonnementen

De component Abonnementen heeft als doel om organisaties in staat te stellen
abonnementen te registreren en beheren. 
We onderscheiden abonnementen op notificaties en abonnementen op Afname.

##### Notificatie-abonnementen

Het kunnen registreren en beheren van abonnementen door organisaties en personen
zodat deze genotificeerd worden over gebeurtenissen die betrekking hebben op
objectgegevens waarin ze geïnteresseerd zijn.

**Invulling**

De uitwerking van deze component is onder andere gebaseerd op:
-   Er is nog geen uitwerking beschikbaar om de component Notificatie op te
    baseren.

Ministerie van BZK, Kadaster en VNG en anderen werken aan een uitwerking van notificatie en
abonnementen. Zie ook de uitwerking van de component Notificatie.

**Uitgangspunten**

Voor de uitwerking van de component gelden de volgende uitgangspunten:
-   Abonnementen zijn abonnementen op gebeurtenissoorten die betrekking hebben
    op objectgegevens. Een abonnement resulteert erin dat de abonnementhouder
    notificaties ontvangt als zich gebeurtenissen van die soort voordoen.

**Vereisten**

Voor deze component gelden de volgende vereisten:

1.  Abonnementen kunnen worden aangegaan door personen en door organisaties.

2.  Abonnementhouders kunnen kiezen uit verschillende notificatiekanalen en
    verschillende notificatie-formaten. In ieder geval zijn kanalen beschikbaar
    voor systemen (API, system-2-system) en voor personen (system-2-persoon,
    bijv. mail). Of hiervoor een pull of push mechanisme wordt gehanteerd is
    later te bepalen.

Zie ook de uitwerking van de component Notificatie.

**Externe afhankelijkheden**

Deze component heeft de volgende externe afhankelijkheden:

-   Geen externe afhankelijkheden

Afhankelijk van de ontwikkelingen van overheidsbrede afspraken en voorzieningen
met betrekking tot notificeren en abonneren ontstaan er mogelijk in de toekomst
afhankelijkheden naar gemeenschappelijke voorzieningen hiervoor, vergelijkbaar
met de bestaande voorziening Digilevering. Zie ook de uitwerking van de
component Notificatie.

##### Abonnementen op Afname

Het kunnen registreren en beheren van afnemers en abonnementen op Afname. 
Zie ook de uitwerking van de component Afname.

<p class ='note'>
    Noot voor reviewers: Willen we het nemen van een abonnement altijd randvoorwaardelijk stellen
    (ook bij gratis en open services) om een afname service te kunnen gebruiken, of vinden we dat services ook zonder abonnement beschikbaar moeten zijn?
    Bijvoorbeeld: Dit geeft enerzijds meer administratieve last maar anderzijds ook
    het voordeel dat gebruikers van de service gericht op de hoogte gebracht kunnen
    worden van veranderingen aan de service.
</p>

**Invulling**

De uitwerking van deze component is onder andere gebaseerd op:

-   API-management
-   Werkwijze Haal Centraal
-   Werkwijze PDOK
-   NLX (common ground)
-   En andere goede voorbeelden

<p class ='note'>
    NOOT voor reviewers: Kunt u ons helpen met andere goede toekomstgerichte
    voorbeelden van uitwerkingen van abonnementen op gegevens en informatie?
</p>

**Uitgangspunten**

Voor de uitwerking van de component gelden de volgende uitgangspunten:

-   Abonnementen zijn abonnementen op (eventueel betaalde) data-, gemaks- en proces-
    API’s (met gegarandeerde dienstenniveau’s).
-   Abonnementen zijn abonnementen op periodieke gegevensleveringen.

**Vereisten**

Voor deze component gelden de volgende vereisten:

1.  Abonnementen kunnen worden aangegaan door personen en door organisaties.

2.  Ondersteuning van verschillende abonnementsvormen voor data-, gemak- en proces-
    API’s, denk aan:

    -  Per request
    -  Staffelprijzen
    -  Kosteloos
    -  En andere

3.  Een periodieke gegevenslevering wordt georganiseerd met een data-API (en is
    daarmee niet anders dan de vereisten van de andere punten van deze
    paragraaf)

4.  De toegang tot de API’s wordt georganiseerd met behulp van geldige
    abonnementssleutels.

Zie ook de uitwerking van de component Afname.

**Externe afhankelijkheden**

Deze component heeft de volgende externe afhankelijkheden:

-   Geen externe afhankelijkheden

#### Betalingen

Voor het beheren van de betalingen van betaalde diensten door de gebruikers van
die diensten, indien sprake is van betaalde diensten. Betalen kan op
verschillende manieren worden ingericht, zoals vooraf, bij afname van de dienst
of achteraf.

Betalingen is 1 op 1 gekoppeld met abonnementen. Betalingen levert het
betaalmechanisme.

**Invulling**

De invulling van deze component is gebaseerd op:

-   Standaard componenten (software) voor betalingen

**Uitgangspunten**

Voor de uitwerking van de component gelden de volgende uitgangspunten:

-   De betalingen zijn 1 op 1 gekoppeld aan abonnementen. Overige betalingen
    zijn vooralsnog buiten scope.

**Vereisten**

Voor deze component gelden de volgende vereisten:

1.  Kunnen opnemen van de betaler

2.  Automatisch kunnen factureren en/of automatisch kunnen afschrijven van een
    rekening of gestort tegoed.

3.  Mechanismen om de betalingen te kunnen monitoren

**Externe afhankelijkheden**

Deze component heeft de volgende externe afhankelijkheden:

-   Er is geen externe afhankelijkheid

#### Machtigingen

De component Machtigingen heeft als doel dat een gebruikersorganisatie een
andere organisatie kan machtigen om als gegevensleverancier of gegevensafnemer
met bepaalde bevoegdheden voor bepaalde gegevenssoorten op te treden namens de
machtigende gebruikersorganisatie.

Alleen een gebruikersorganisatie in de rol van bronhouder kan gegevensleveranciers machtigen.

Of machtigen voor afnemers nodig is moet nog blijken.

Een machtiging is geldig voor een bepaalde periode, zodat toegang voor de duur
van de afspraken en contracten kan worden verleend.

**Invulling**

De invulling van deze component is gebaseerd op:

-   Het beheer van projectmachtigingen dat is beschreven en gerealiseerd in het
    [bronhouderportaal-bro](https://doc.bronhouderportaal-bro.nl/bronhouders/machtigingen/).
-   De wijze van machtigen die is beschreven en gerealiseerd in de
    [machtigingenmodule van de BGT](https://www.svb-bgt.nl/machtigingenmodule/)

**Uitgangspunten**

Voor de uitwerking van de component gelden de volgende uitgangspunten:

-   Er zijn (nog) geen uitgangspunten gedefinieerd.

**Vereisten**

Voor deze component gelden de volgende vereisten:

1.  Machtigingen worden gegeven op het niveau van organisaties. De gemachtigde
    organisatie kan ook een andere bronhouderorganisatie zijn.

2.  Autorisatie op het niveau medewerker/afdeling is de verantwoordelijkheid van
    de gemachtigde organisatie. De gemachtigde organisatie moet daar
    verantwoording over af kunnen leggen.

3.  Machtigingen kennen een geldigheidsduur. Toegang tot de services is in de
    tijd beperkt tot die geldigheidsduur.

4.  Machtigingen geven organisaties toegang tot bepaalde services. Voor het
    verkrijgen van toegang tot die services blijven de eisen gelden die bij de
    component Toegang zijn beschreven.

**Externe afhankelijkheden**

Deze component heeft de volgende externe afhankelijkheden:

-   Er is geen externe afhankelijkheid



### Algemeen

Hier worden de algemene onderwerpen Toegang en Interactie uitgewerkt.

#### Toegang

Toegang heeft als doel het bewaken van de toegang door te bepalen wie een gebruiker is en wat die gebruiker mag om de gebruiker toegang tot een dienst te verlenen.

De gebruiker kan een persoon of een informatiesysteem zijn. Toegang voor
informatiesystemen betreft de toegang tot services (Common Ground laag 2).
Toegang voor personen betreft de toegang via interactiecomponenten (Common
Ground laag 5).

De [afbeelding](https://www.noraonline.nl/wiki/Bestand:IAM_afbeelding.png) bij
het thema [Identity & Accessmanagement van de NORA](https://www.noraonline.nl/wiki/Identity_&_Access_Management_(IAM)) geeft dit
goed weer.

**Invulling**

De invulling van Toegang is onder andere gebaseerd op:

-   [GEMMA Gegevenslandschap](https://www.gemmaonline.nl/index.php/Gegevenslandschap) – Authenticatie en Autorisatie,
     en specifiek https://www.gemmaonline.nl/images/gemmaonline/7/75/GEMMA_Gegevenslandschap_-_Autorisatie_en_authenticatie_v1_0.pdf
-   [Nederlandse API-strategie](https://docs.geostandaarden.nl/api/API-Strategie/)
    , specifiek het deel over
    OAuth in combinatie met PKIoverheid en TLS
    https://docs.geostandaarden.nl/api/oauth/
-   GAS Knooppunt – Toegang van DSO-LV
    https://aandeslagmetdeomgevingswet.nl/publish/library/219/dso_-_gas_-_knooppunt_toegang_iam_1.pdf
    beschikbaar op
    https://aandeslagmetdeomgevingswet.nl/digitaal-stelsel/documenten/architectuurdocumenten/

**Uitgangspunten**

Voor de uitwerking van de component gelden de volgende uitgangspunten:

-   Toegang voor informatiesystemen betreft Organisatie-authenticatie en
    Diensten-autorisatie. Toegang voor personen betreft
    Eindgebruiker-authenticatie en Functie-autorisatie.
-   Een informatiesysteem kan toegang verkrijgen tot een dienst als het zich
    authenticeert als een organisatie die geautoriseerd is voor de dienst.
-   Een eindgebruiker (persoon) kan toegang verkrijgen tot een functie van een
    informatiesysteem als deze zich authenticeert als eindgebruiker (of
    functionaris of rol) die geautoriseerd is voor de functie.
-   Het is aan de organisatie om te verzekeren dat eindgebruikers namens de
    organisatie zich op toegestane wijze authenticeren en tevens te verzekeren
    dat de autorisatie van functionarissen alleen geldig is in de periode waarin
    de functie wordt vervuld.

**Vereisten**

Voor de component Toegang gelden de volgende vereisten.

**Toegang voor informatiesystemen van bronhouders:**

1.  Er zijn vier niveaus van toegang te onderkennen (in lijn met GAS Knooppunt –
    Toegang van DSO-LV):

    1.  Open toegang zonder gegarandeerd serviceniveau, op basis van een
        fair-use budget. Authenticatie en autorisatie vindt plaats op basis van
        een uitgegeven API-key in combinatie met enkelzijdige TLS.

    2.  Open toegang met gegarandeerd serviceniveau. Authenticatie en
        autorisatie vindt plaats op basis van identificatie van de organisatie
        met OAuth in combinatie met enkelzijdige TLS. Dit niveau wordt ook
        gehanteerd voor betaalde diensten.

    3.  Gesloten toegang met gegarandeerd serviceniveau. Authenticatie en
        autorisatie vindt plaatst op basis van identificatie van de organisatie
        met PKIoverheid en eventueel OAuth in combinatie met tweezijdige TLS.

    4.  Gesloten met doelbinding. Authenticatie en autorisatie vindt plaatst op
        basis van identificatie van de organisatie met PKIoverheid en eventueel
        OAuth in combinatie met tweezijdige TLS. Deze vierde vorm is mogelijk
        niet nodig voor de toegang voor afnemers van de objectenregistratie.

2.  Autorisatie voor diensten voor bronhouders vindt plaats op
    organisatieniveau.

3.  Autorisatie op het niveau van medewerker/afdeling is de verantwoordelijkheid
    van de bronhouderorganisatie. De bronhouderorganisatie moet daar
    verantwoording over af kunnen leggen. Zie ook paragraaf 6.1 van GEMMA
    Gegevenslandschap – Authenticatie en Autorisatie.

4.  Het is mogelijk om centrale diensten voor het bewerken van gegevens in combinatie met
    gegevenssoorten te koppelen aan bevoegdheden.  
    Bijvoorbeeld bevoegdheden als het aanmaken van een nieuw object en het veranderen
    van de gegevens van een object.

5.  Bevoegdhedenbeheer (welke medewerker/afdeling welke bevoegdheden heeft voor
    welke gegevenssoorten) is de verantwoordelijkheid van de
    bronhouderorganisatie.

6.  Per gegeven is bekend welke organisatie de bronhouder is.

   Voorwaarde hiervoor is dat relatie bronhouder – gegeven vastligt dmv een
   identificatie van de bronhouder die te relateren is aan de identificatie van
   de bronhouder bij het verlenen van de toegang.

1.  Het al dan niet toestaan van het aanroepen van een centrale dienst van de objectenregistratie door
    een organisatie voor het bewerken van gegevens wordt niet vastgelegd (niet
    gelogd). Dat een organisatie op een bepaalde dag en tijdstip wel of geen
    toegang tot een dienst is verleend wordt niet vastgelegd.  
    N.B. het ‘uitvoeren’ van een dienst van de objectenregistratie die leidt tot een verandering van
    gegevens wordt wel vastgelegd (gelogd). Dat hoort bij het onderdeel
    Registratie.

**Toegang voor informatiesystemen van afnemers:**

De vereisten aan de component Toegang voor afnemers zijn sterk afhankelijk van
de mate waarin doelbinding, authenticatie en autorisatie nodig zijn. De hier
gehanteerde aanname is dat dat nodig kan zijn.

1.  Indien van toepassing is autorisatie op het niveau van medewerker/afdeling
    de verantwoordelijkheid van de afnemende organisatie. Deze moet daar indien
    van toepassing verantwoording over af kunnen leggen.

2.  Het al dan niet toestaan van het aanroepen van een centrale dienst door
    een organisatie voor het afnemen van gegevens wordt niet vastgelegd (niet
    gelogd). Dat een organisatie op een bepaalde dag en tijdstip wel of geen
    toegang tot een dienst van de objectenregistratie is verleend wordt niet vastgelegd.

3.  Machtigingen.  
    Indien van toepassing kan een afnemer een andere organisatie machtigen als
    afnemer.

**Toegang voor personen tot functionaliteit via interactiecomponenten:**

Onderstaande vereisten zijn van toepassing op de interactiecomponenten (zoals
viewers en webloketten) die onderdeel zijn van de objectenregistratie.

1.  Authenticatie van personen (buiten de beheerorganisatie van de objectenregistratie) vindt, indien
    nodig, plaats op basis van door de overheid erkende middelen zoals DigiD,
    eHerkenning en eIDAS-erkende middelen.

2.  De inrichting van de authenticatie en autorisatie van medewerkers van de beheerorganisatie van de objectenregistratie is te bepalen door die beheerorganisatie zelf.  
    GEMMA Gegevenslandschap – Authenticatie en Autorisatie zegt hierover:  
    *“In het GEMMA Gegevenslandschap wordt voor autorisatie voor het
    applicatiefuncties en de afname van diensten bij voorkeur gebruik gemaakt
    van autorisatie op basis van attributen (ABAC). De reden hiervoor is dat
    deze autorisatiemethode ruimte biedt voor het invullen van lokale wensen en
    invulling kan geven aan de eisen die vanuit de privacywetgeving aan
    autorisatie worden gesteld. Bij deze methode van autoriseren worden
    toegangsrechten geassocieerd met een set van regels, die zijn uitgedrukt in
    meetbare parameters of attributen; vervolgens worden die toegekend aan
    subjecten die kunnen bewijzen dat zij voldoen aan de regels. ABAC geeft dus
    toegang tot IT-diensten op basis van een bewering over de eigenschappen
    (attributen) van de dienstaanvrager (subject). De attributen kunnen allerlei
    formaten of gedaantes hebben: groepen, rollen, clearance levels, context
    etc.”*

**Externe afhankelijkheden**

De component Toegang heeft de volgende externe afhankelijkheden:

-   Er is een afhankelijkheid van de functionaliteiten, standaarden,
    serviceniveaus, governance en financiering van de gebruikte
    (overheids)identificatie- en authenticatiemiddelen.
-   Er is een afhankelijkheid van gemaakte afspraken over te hanteren
    standaarden zoals PKIoverheid, eHerkenning, DigiD, OAuth, TLS e.d.

#### Interactie

De interactiecomponenten van de objectenregistratie hebben als doel om de diensten en de
gegevens en producten van de objectenregistratie aan eindgebruikers (personen in de rol van
bronhouder of afnemer) te presenteren en de mogelijkheden te bieden om er mee te
interacteren.

De objectenregistratie zal verschillende generieke interactiecomponenten bieden, bijvoorbeeld
een viewer voor het bekijken, zoeken en raadplegen van objectgegevens (inzage), portalen
voor het beheren van machtigingen en loketten voor het indienen van
terugmeldingen en het beheren van abonnementen.

<p class ='note'>
    voor reviewers: welke invullingen, uitgangspunten vereisten moeten we van
    toepassing verklaren op de interactiecomponenten van de objectenregistratie?
</p>

**Invulling**

De invulling van interactie is gebaseerd op:

-   De principes van [Gebruiker Centraal](https://www.gebruikercentraal.nl)
-   De eisen aan [Digitoegankelijkheid](https://www.digitoegankelijk.nl)

**Uitgangspunten**

Voor de uitwerking van interactie gelden de volgende uitgangspunten:

-   Nog geen uitgangspunten benoemd.

**Vereisten**

Voor interactie gelden de volgende vereisten:

-  Nog geen vereisten benoemd.

**Externe afhankelijkheden**

Interactie heeft de volgende externe afhankelijkheden:

-   Nog geen afhankelijkheden benoemd.
