## Inleiding

Dit document is de *Architectuurbeschrijving* van de Samenhangende Objectenregistratie. Het beschrijft de afbakening, de ICT-inrichtingsprincipes en de conceptuele of functionele inrichting (de functionele onderdelen en samenhang) van de ICT-componenten voor de Samenhangende Objectenregistratie. Met andere woorden, de Architectuurbeschrijving beschrijft de Objectenregistratie op de Applicatielaag, laag 4 in het [NORA-vijflaagsmodel](https://www.noraonline.nl/wiki/Vijflaagsmodel)

<figure id="nora5laagsmodel">
    <img src="media/nora5laagsmodel.PNG" alt="nora5laagsmodel">
    <figcaption>Het NORA 5 laagsmodel</figcaption>
</figure>

### Doel en doelgroep

De Architectuurbeschrijving moet het mogelijk maken om  keuzes te maken voor de verdere inrichting van de ICT-voorzieningen (componenten, applicaties of systemen) voor de Samenhangende Objectenregistratie. Ook moet de Architectuurbeschrijving het mogelijk maken om de transitiestrategie te bepalen voor de overgang van de huidige voorzieningen van o.a. de BAG, BGT, BRO en BRT naar de ICT-componenten voor de Objectenregistratie. Tot slot moet de Architectuurbeschrijving het mogelijk maken om de technische en organisatorische inrichting voor de ICT-voorzieningen voor de Objectenregistratie te bepalen. De onderscheiden functies (capabilities, "wat moet kunnen") binnen het systeem worden zodanig beschreven dat een opdracht om deze verder uit te werken inhoudelijk voldoende duidelijk is voor opdrachtgever en opdrachtnemer.

De Architectuurbeschrijving geeft richting aan de nadere inrichting van de ICT-componenten voor de Objectenregistratie en is daarom met name bedoeld voor degenen die betrokken zijn bij die inrichting. Daarnaast is de Architectuurbeschrijving van belang voor de afstemming over de inrichting van de ICT-voorzieningen voor de Objectenregistratie met alle belanghebbenden: beleidsverantwoordelijke(n), bronhouders, verstrekker(s), afnemers, beheerders en (software-)leveranciers en andere belanghebbenden.

### Leeswijzer

De Architectuurbeschrijving van de Samenhangende Objectenregistratie heeft de volgende opbouw:

Het hoofdstuk [Afbakening](#afbakening) beschrijft de grenzen van de Objectenregistratie en de interactie met de omgeving. De afbakening brengt in kaart welke rollen en partijen (waaronder bronhouders en afnemers) interactie met de ICT-voorzieningen van de Objectenregistratie hebben en welke soorten interactie er zijn.

Het hoofdstuk [ICT-inrichtingsprincipes](#ict-inrichtingsprincipes) beschrijft de principes die bepalend zijn voor de functionele en deels ook technische inrichting van de ICT-voorzieningen en de bijbehorende ICT-organisatie van de Objectenregistratie.  

Het hoofdstuk [Inrichting van de Objectenregistratie](#inrichting-van-de-objectenregistratie) beschrijft de conceptuele inrichting van de ICT-voorzieningen van de Objectenregistratie op de applicatielaag van het NORA-vijflaagsmodel.

Het hoofdstuk [Componenten](#componenten) werkt de ICT-onderdelen van de Objectenregistratie verder uit en vormt het kader vormt voor de technische inrichting en biedt een gedeelte van de basis voor de organisatorische inrichting rond de ICT-voorzieningen.

Relevante bijlagen staan in het hoofdstuk [Bijlagen](#bijlagen-principes)

<p class='note'>
     Voor reviewers: In groene kaders stellen de auteurs soms een vraag. In jullie reviewcommentaar lezen we graag antwoorden.
</p>

### Het proces

<p class='note'>
     Voor auteurs: Onderstaande is standaard tekst voor alle SOR-documenten, toch? Dus geen wijzigingen aanbrengen? (WB)
</p>

De Architectuurbeschrijving van de Samenhangende Objectenregistratie is een product van een samenwerking van Geonovum, het Kadaster, het ministerie van BZK en VNG Realisatie. Bij de totstandkoming zijn diverse belanghebbenden betrokken, o.a. via een denktank en klankbordgroep.

Globale uitgangspunten voor het gegevensmodel, de voorziene pocessen voor inwinning, productie en ontsluiting van gegevens, en eerste beelden over de organisatie en governance en financiering zijn vastgelegd in een beleidsvisie samenhangende objectenregistratie die eind 2019 door het BAG BAO en de Regieraad BGT is vastgesteld.

Sindsdien wordt er gewerkt aan een verdere invulling van een drietal onderwerpen, die samenvallen met drie van de vijf lagen uit het NORA-vijflaagsmodel (figuur 1):

Een uitwerking van de governance, organisatie en financiering van een samenhangende objectenregistratie, bestaande uit onder meer een beschrijving van taken en verantwoordelijkheden, de inrichting van de besluitvormingsstructuur, financieringsafspraken en een eerste opzet van ketenprocessen (organisatorische laag / laag 2 uit het NORA-vijflaagsmodel). Hiervan zijn op dit moment nog geen documenten beschikbaar.

Een uitwerking van de inhoud van een samenhangende objectenregistratie, bestaande uit onder meer inhoudelijke uitgangspunten, de invulling van een aantal generieke onderwerpen die van belang zijn voor de informatiemodellering en een conceptuele beschrijving van de SOR-begrippen (soorten objecten), de eigenschappen die daarvan worden vastgelegd en de waarden die deze eigenschappen kunnen aannemen (informatielaag / laag 3 uit het NORA-vijflaagsmodel). Een hoodlijnenrapport is beschikbaar.

Een uitwerking van de architectuurbeschrijving van de ICT-voorzieningen voor een samenhangende objectenregistratie, bestaande uit een afbakening van de systeembegrenzing, ICT-inrichtingsprincipes en een uitwerking van de functionele onderdelen van de ICT-voorzieningen en hun onderlinge samenhang (applicatielaag / laag 4 uit het NORA-vijflaagsmodel). Het document dat u nu leest is hiervan een versie.

