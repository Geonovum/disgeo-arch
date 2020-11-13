## ICT-inrichtingsprincipes

Dit hoofdstuk beschrijft de principes die richtinggevend zijn voor de functionele inrichting van de ICT-voorzieningen voor de Objectenregistratie en de bijbehorende ICT-Beheerorganisatie. 

### Beleid Samenhangende Objectenregistratie

De overkoepelende [Architectuurvisie DiS-Geo](https://www.geobasisregistraties.nl/documenten/publicatie/2020/07/16/houtskoolschets-architectuurvisie-dis-geo) geeft de richtinggevende kaders waarbinnen de bestaande geo basisregistraties worden doorontwikkeld tot een samenhangende objectenregistratie.

De [Beleidsvisie Samenhangende Objectenregistratie](https://www.geobasisregistraties.nl/documenten/beleidsnota/2019/11/29/beleidsvisie-samenhangende-objectenregistratie) beschrijft de doelstellingen en beleidscontouren voor de objectenregistratie.  

De volgende uitgangspunten voor de architectuur van de objectenregistratie zijn afgeleid uit beide bovenstaande documenten.

**Vanuit Architectuurvisie DiS-Geo**
 1. Bronhouders zijn verantwoordelijk voor basisgegevens
 2. Bronhouders kunnen leveranciers machtigen
 3. Gegevens aanpassen kan makkelijk en goed
 4. Gegevens passen bij elkaar: relaties tussen gegevens zijn voor gebruikers duidelijk, en gegevens zijn in samenhang bruikbaar
 5. De gegevensstructuur kan snel genoeg meegroeien met de gebruiksbehoefte

**Vanuit Beleidsvisie Samenhangende Objectenregistratie**
 6. We laten ons bij het ontwerp en de verdere uitwerking niet beperken door de nu bestaande juridische kaders (deze kunnen in principe worden aangepast, via een traject aanpassing wet- en regelgeving).
 7. In het ontwerp van een samenhangende objectenregistratie is sprake van een nadrukkelijke scheiding tussen de vastlegging van gegevens en de functionaliteit voor het bewerken, opvragen en presenteren daarvan.
 8. Er wordt gebruik gemaakt van standaard infrastructurele voorzieningen die beschikbaar zijn bij de bronhouders en de gebruikers (denk hierbij aan standaardnetwerken, netwerkprotocollen en beveiligingsmechanismen).
 9. Er wordt in de eindsituatie zoveel mogelijk uitgegaan van ‘bevragen bij de bron’. Hierbij is van belang dat de gebruiker voor verstrekkingen zoveel mogelijk uit kan gaan van één loket. Een belangrijk aandachtspunt hierbij is het gebeurtenis georiënteerd werken (nader uit te werken). Of de bronhouders gedistribueerd en decentraal werken of direct inwinning en bijhouding in een (of meerdere) voorziening(en) uitvoeren via gestandaardiseerde services moet nader bepaald worden (nadere uitwerking in kader van DiS GEO/beleidsvisie: leveranciers, bronhouders, Kadaster, VNG-R, Ministerie van BZK).
 10. Er wordt ingewonnen op het niveau van de huidige schaalniveaus van BAG en BGT. De gegevens kunnen gepresenteerd worden op verschillende schaalniveaus (meest gedetailleerde weergave: 1:1.000). Autogeneralisatie voor informatie op hogere schaalniveaus moet mogelijk zijn (op basis van logica en functies). Bijvoorbeeld het (deels) afleiden van de informatie voor de BRT uit de BGT, maar ook voor het definiëren van een wegennetwerk met alle rijkswegen op basis van het gehele wegennetwerk.
 11. Keuzen voor een technische inrichting van de registratie worden pas later in het traject gemaakt, zodat oplossingen gebaseerd zijn op recente inzichten in oplossingsmogelijkheden.
 12. Vanuit andere (basis)registraties, zoals de subjectenregistraties BRP of HR, moeten eenvoudig relaties gelegd kunnen worden naar de samenhangende objectenregistratie.
 13. De registratie gedraagt zich voor gebruikers zoveel mogelijk als één registratie, of het daadwerkelijk één registratie wordt, is nog niet bepaald (nader uit te werken). Daarnaast kunnen er uit de registratie (informatie)producten afgeleid worden en beschikbaar gesteld worden.
 14. De kerngegevens en aanvullende gegevens worden in principe ontsloten als open data (waar nodig ontsloten op basis van autorisaties), dus het “open data, tenzij” regime geldt.
 15. In principe kan de informatie via meerdere kanalen, afgestemd op gebruikersbehoefte, uitgeleverd worden (nadere uitwerking in kader van DiS GEO).


### Inrichtingsprincipes vergelijkbare domeinen

Binnen andere domeinen is veel kennis en kunde opgebouwd over inrichtingsprincipes van dit soort ICT-voorzieningen. We hebben hier met name gebruik gemaakt van de volgende groepen met ervaring en vastgelegde kennis:
- De [Overall Globale Architectuur Schets (OGAS)](https://aandeslagmetdeomgevingswet.nl/publish/library/219/dso_-_gas_-_overall_gas_1.pdf) van het Digitaal Stelsel Omgevingswet. Zie ook de [bijlage](#inrichtingsprincipes-digitaal-stelsel-omgevingwet).
- De referentie architectuur [NORA](#basisprincipes-nora) van de architecten van samenwerkende Nederlandse overheden  
- Het [GEMMA Gegevenslandschap en Common Ground](#architectuurprincipes-gemma-gegevenslandschap-en-common-ground) van samenwerkende gemeenten en de Vereniging van Nederlandse Gemeenten.
- De [10 golden rules data](#10-golden-rules-data) die tot stand zijn gekomen vanuit de best-practices rondom data management.


### ICT-inrichtingsprincipes Samenhangende Objectenregistratie

Voor de ICT-inrichting van de Samenhangende Objectenregistratie hanteren we de onderstaande principes. Met 'de oplossing' bedoelen we steeds de ICT-voorzieningen die de Samenhangende Objectenregistratie realiseren.

 **Inrichtingsprincipe 1: Gegevens worden gescheiden van applicaties bewaard**, *zodat* het beheren en afnemen van gegevens onafhankelijk is van de gebruikte applicaties en gegevens te (her)gebruiken zijn in verschillende applicaties voor verschillende doeleinden.
 
Grondslag: Uitgangspunten (7, 9), GGL / Common Ground (04)

**Inrichtingsprincipe 2: Ieder gegeven wordt op precies &eacute&eacuten plek bijgehouden**, *zodat* altijd duidelijk is wat het actuele brongegeven is en waar dat wordt beheerd. Dit principe heeft de volgende onderliggende principes in zich:

    - **Dubbele opslag betekent synchroniseren**, zodat partijen altijd naar dezelfde gegevens kijken. Dit geldt zowel binnen als buiten de oplossing, dus ook voor eventuele afgeleide opslag die geoptimaliseerd is ten behoeve van verstrekking.

Grondslag: Uitgangspunten (9, 11, 15), GGL / Common Ground (04)

**Inrichtingsprincipe 3: Gegevens zijn alleen te benaderen via dataservices**, *zodat* deze services kunnen garanderen dat de gegevens, metagegevens en de toegang ertoe altijd voldoen aan de eisen en dat logging altijd plaatsvindt. Om te garanderen dat de gegevens blijven voldoen aan de gestelde kwaliteit en actualiteit kunnen ze alleen benaderd worden via (data)services. Dit principe zorgt ervoor dat gegevens blijven voldoen aan de (integriteits-)eisen, doordat de dataservices dit waarborgen. Ook zorgt dit principe ervoor dat er een ontkoppeling is tussen de gegevens en de ontsluiting ervan. Applicaties benaderen de gegevens via de dataservices en niet direct. Dat maakt het mogelijk om veranderingen aan te brengen in de gegevensopslag of in de dataservices zonder dat deze elkaar beïnvloeden. Hierdoor kan flexibel omgegaan worden met aanpassingen in het gegevensmodel. Dit principe heeft de volgende onderliggende principes in zich:
    - **Dataservices regelen de toegang tot gegevens**, *zodat* deze services ervoor kunnen zorgen dat altijd is voldaan aan de eisen betreffende toegang. De services controleren of de gebruiker wel de toegangsrechten heeft om de gegevens te maken, te lezen of aan te passen.
    - **Dataservices leggen elke toegang tot gegevens vast in logging**, *zodat* deze services ervoor kunnen zorgen dat aantoonbaar is wat door gemachtigde leveranciers onder verantwoordelijkheid van bronhouders plaatsvindt. Alle transacties op de gegevens worden gelogd. Dit is nodig om een audit-trail te kunnen opbouwen.
    - **Dataservices houden metadata actueel**, *zodat* data en meta-data altijd onderling consistent zijn.
    - **Dataservices borgen de gegevensregels**, *zodat* gegarandeerd is dat de gegevens altijd voldoen aan de gegevensregels.

Grondslag: Uitgangspunten (1, 2, 3, 5, 7, 8, 9), DSO (05)
 
**Inrichtingsprincipe 4: Informatie wordt op betrouwbare en veilige wijze ontsloten**, *zodat* aangetoond kan worden dat data niet bedoeld of onbedoeld gemanipuleerd is. Om op data te kunnen vertrouwen zorgen functies ervoor dat data bij alle handelingen vanaf het moment van ontstaan tot het moment van gebruik veilig is. Data wijzigt daarom alleen op basis van een brondocument of mutatieverwijzing en de wijziging wordt vastgelegd. Integriteit en consistentie van data wordt bewaakt. Data wordt bewaard conform de eisen van de wet (w.o. archiefwet, etc.).

Grondslag: Uitgangspunten (3, 7, 9), DSO (09), GGL / GGL / Common Ground (03)

**Inrichtingsprincipe 5: Samenhangend gebruik van data is makkelijk mogelijk**, zodat data uit verschillende gegevensverzamelingen te combineren is. Het is mogelijk dat er samengestelde producten over het geheel van het gegevenslandschap kunnen worden gerealiseerd. Dit principe heeft de volgende onderliggende principes in zich:
    - **Alles is een service**, *zodat* alle functionaliteit zonder handmatige/menselijke tussenstappen kan worden gecombineerd om samenhangend gebruik makkelijk te maken.
    - **Intern is extern**, *zodat* alle services herkenbaar en begrijpbaar zijn voor zowel interne als externe leveranciers van fucntionaliteit aan bronhouders en afnemers. Dit is essentieel om mogelijk te maken om op innovatieve manieren de waarde van gegevens in samenhangend gebruik te vergroten.

Grondslag: Uitgangspunten (4, 12, 13, 15), DSO (05)



Overigens wordt van dienstenaanbieders verwacht dat ze invulling geven aan basisprincipes die staan genomend in de NORA, zie https://www.noraonline.nl/wiki/Basisprincipes_totaaloverzicht. 
Vanuit basisprincipes BP01 tot en met BP05: diensten zijn proactief vindbaar en toegankelijk, uniform en gebundeld voor afnemers. 
Vanuit basisprincipes BP09 en BP10: dienstenaanbieder is betrouwbaar en ontvankelijk voor input. 

