## Inleiding


Het stelsel van basisregistraties is in Nederland een belangrijke grondlegger voor de informatiehuishouding van de (digitale) overheid. Binnen dit stelsel is een belangrijke plek weggelegd voor de geo-basisregistraties, die gegevens bevatten met een locatiecomponent. Meer samenhang tussen deze registraties is gewenst om efficiënte inwinning en bijhouding en integraal gebruik mogelijk te maken. Om een integrale doorontwikkeling mogelijk te maken is het Ministerie van BZK de Doorontwikkeling in Samenhang van de geo(basis)registraties (DiS Geo) gestart. Een belangrijke eerste stap daarbinnen is de totstandbrenging van een samenhangende objectenregistratie.

De [samenhangende objectenregistratie](https://www.geobasisregistraties.nl/basisregistraties/doorontwikkeling-in-samenhang/objectenregistratie) als volgt gedefinieerd:

Een samenhangende objectenregistratie is een uniforme registratie met daarin basisgegevens over objecten in de fysieke werkelijkheid die zich voor gebruikers als één registratie gedraagt. Daaronder verstaan we objecten die in het terrein zichtbaar zijn, zoals gebouwen, wegen, water, spoorlijnen en bomen, terreindelen, aangevuld met enkele (administratieve) objecten als woonplaatsen, gemeentegrenzen en openbare ruimten. De samenhangende objectenregistratie gedraagt zich als een geheel waar bronhouders gegevens ‘in stoppen’ en afnemers gegevens ‘uit halen’.

Dit document is de **Architectuurbeschrijving Voorzieningen** van de Samenhangende Objectenregistratie. Het beschrijft de afbakening, de inrichtingsprincipes en de conceptuele of functionele inrichting (de functionele onderdelen en samenhang) van de ICT-componenten voor de Samenhangende Objectenregistratie. Met andere woorden, de Architectuurbeschrijving Voorzieningen beschrijft de Objectenregistratie op de Applicatielaag, laag 4 in het [NORA-vijflaagsmodel](https://www.noraonline.nl/wiki/Vijflaagsmodel)

De scope van de architectuur omvat de gemeenschappelijke voorzieningen voor het registreren, bewaren en ontsluiten van de objectgegevens in de objectenregistratie. Voorzieningen die bronhouders gebruiken voor het inwinnen van objectgegevens (zoals voor beeldmateriaal) vallen buiten de scope. Ook de voorzieningen van afnemers voor het gebruiken van de gegevens en voor het, indien nodig, lokaal opslaan van kopieën van de gegevens vallen buiten de scope.

<figure id="scope-in-nora5laagsmodel">
    <img src="media/scope-in-nora5laagsmodel.png" alt="scope in nora5laagsmodel">
    <figcaption>Scope in het NORA 5 laagsmodel</figcaption>
</figure>

### Doel en doelgroep

Deze architectuurbeschrijving moet het mogelijk maken om keuzes te maken voor de verdere inrichting van de ICT-voorzieningen (componenten, applicaties of systemen) voor de Samenhangende Objectenregistratie. Ook moet de architectuurbeschrijving input het mogelijk maken om de transitiestrategie te bepalen voor de overgang van de huidige voorzieningen van o.a. de BAG, BGT en BRT naar de ICT-componenten voor de Objectenregistratie. Tot slot moet de architectuurbeschrijving input bieden voor de technische en organisatorische inrichting van de ICT-voorzieningen voor de Objectenregistratie. De onderscheiden functies binnen het systeem worden zodanig beschreven dat een opdracht om deze verder uit te werken inhoudelijk voldoende duidelijk is voor opdrachtgever en opdrachtnemer.

De architectuurbeschrijving geeft richting aan de nadere inrichting van de ICT-componenten voor de Objectenregistratie en is daarom met name bedoeld voor degenen die betrokken zijn bij die inrichting. Daarnaast is de Architectuurbeschrijving van belang voor de afstemming over de inrichting van de ICT-voorzieningen voor de Objectenregistratie met alle belanghebbenden: beleidsverantwoordelijke(n), bronhouders, verstrekker(s), afnemers, beheerders en (software-)leveranciers en andere belanghebbenden.

### Leeswijzer

De Architectuurbeschrijving van de Samenhangende Objectenregistratie heeft de volgende opbouw:

Het hoofdstuk [Afbakening](#afbakening) beschrijft de grenzen van de Objectenregistratie en de interactie met de omgeving. De afbakening brengt in kaart welke soorten interactie bronhouders en afnemers hebben met de ICT-voorzieningen van de Objectenregistratie.

Het hoofdstuk [Inrichtingsprincipes](#inrichtingsprincipes) beschrijft de principes die bepalend zijn voor de functionele en indirect ook technische inrichting van de ICT-voorzieningen en de bijbehorende ICT-organisatie van de Objectenregistratie.  

Het hoofdstuk [Inrichting](#inrichting) beschrijft de functionele inrichting van de ICT-voorzieningen van de Objectenregistratie op de applicatielaag van het NORA-vijflaagsmodel.

Het hoofdstuk [Uitwerking](#uitwerking) werkt de ICT-onderdelen van de Objectenregistratie verder uit, vormt het kader voor de technische inrichting en biedt input voor de organisatorische inrichting rond de ICT-voorzieningen.

Relevante bijlagen staan in het hoofdstuk [Bijlagen](#bijlage-principes)

### Context

Dit document is een product van een samenwerking van Geonovum, Kadaster, Ministerie van BZK en VNG Realisatie. Bij de totstandkoming zijn diverse belanghebbenden betrokken. Afstemming met een bredere groep belanghebbende organisaties is nodig, met name om de samenhang met het gehele stelsel van basisregistraties te borgen. 

Deze Architectuurbeschrijving Voorzieningen van de Samenhangende Objectenregistratie vormt samen met andere documenten een volledige beschrijving van de samenhangende objectenregistratie, zoals hieronder weergegeven. Op het moment van schrijven zijn niet voor alle blokken al uitwerkingen openbaar.

<figure id="documentenstructuur">
    <img src="media/documentenstructuur.png" alt="documenten van de samenhangende objectenregistratie">
    <figcaption>Documenten van de samenhangende objectenregistratie</figcaption>
</figure>

Globale uitgangspunten voor het programma DiS-Geo worden vastgelegd in een nog te verschijnen beleidsvisie DiS Geo.

De architectuurvisie van het programma DiS-Geo is beschreven in een [houtskoolschets](https://www.geobasisregistraties.nl/documenten/publicatie/2020/07/16/houtskoolschets-architectuurvisie-dis-geo) getiteld "Geodata als stroom uit het stopcontact".

Globale uitgangspunten voor het gegevensmodel, de voorziene processen voor inwinning, registratie en ontsluiting van gegevens, en eerste beelden over de organisatie en governance en financiering zijn vastgelegd in een [beleidsvisie samenhangende objectenregistratie](https://www.geobasisregistraties.nl/documenten/beleidsnota/2019/11/29/beleidsvisie-samenhangende-objectenregistratie) die eind 2019 door het BAG BAO en de Regieraad BGT is vastgesteld.

Sindsdien wordt er gewerkt aan een verdere invulling van een drietal onderwerpen, die samenvallen met drie van de vijf lagen uit het [NORA-vijflaagsmodel](#nora5laagsmodel):

Een uitwerking van de governance, organisatie en financiering van een samenhangende objectenregistratie, bestaande uit onder meer een beschrijving van taken en verantwoordelijkheden, de inrichting van de besluitvormingsstructuur, financieringsafspraken en een eerste opzet van ketenprocessen (organisatorische laag / laag 2 uit het NORA-vijflaagsmodel). Hiervan zijn op dit moment nog geen documenten beschikbaar.

Een uitwerking van de inhoud van een samenhangende objectenregistratie, bestaande uit onder meer inhoudelijke uitgangspunten, de invulling van een aantal generieke onderwerpen die van belang zijn voor de informatiemodellering en een conceptuele beschrijving van de begrippen (soorten objecten), de eigenschappen die daarvan worden vastgelegd en de waarden die deze eigenschappen kunnen aannemen (informatielaag / laag 3 uit het NORA-vijflaagsmodel). Er is een [hoofdlijnenrapport](https://docs.geostandaarden.nl/disgeo/hiso/) verschenen en er zijn [eisen aan het model](https://docs.geostandaarden.nl/disgeo/emso/). 

Een uitwerking van de architectuurbeschrijving van de ICT-voorzieningen voor een samenhangende objectenregistratie, bestaande uit een afbakening van de systeembegrenzing, ICT-inrichtingsprincipes en een uitwerking van de functionele onderdelen van de ICT-voorzieningen en hun onderlinge samenhang (applicatielaag / laag 4 uit het NORA-vijflaagsmodel). Het document dat u nu leest is hiervan een versie.

