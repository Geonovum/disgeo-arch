## ICT-inrichtingsprincipes

Dit hoofdstuk beschrijft de principes die richtinggevend zijn voor de functionele inrichting van de ICT-voorzieningen voor de Objectenregistratie en de bijbehorende ICT-organisatie. 

### Beleid Samenhangende Objectenregistratie

De beleidsvisie Samenhangende Objectenregistratie (SOR), als onderdeel van DiS-Geo, beschrijft de doelstellingen en beleidscontouren van de SOR (zie: https://www.geobasisregistraties.nl/documenten/beleidsnota/2019/11/29/beleidsvisie-samenhangende-objectenregistratie). Naast de beleidsvisie is gewerkt aan een houtskoolschets voor DiS-Geo (zie: https://www.geobasisregistraties.nl/basisregistraties/documenten/publicatie/2020/06/15/dis-online-als-stroom-uit-het-stopcontact).

De volgende beleidsuitgangspunten voor de architectuur van de SOR zijn afgeleid uit de 2 bovenstaande beleidsdocumenten.

> **vanuit Beleidsvisie Samenhangende Objectenregistratie**
> 1. We laten ons bij het ontwerp en de verdere uitwerking niet beperken door de nu bestaande juridische kaders (deze kunnen in principe worden aangepast, via een traject aanpassing wet- en regelgeving).
> 2. In het ontwerp van een samenhangende objectenregistratie is sprake van een nadrukkelijke scheiding tussen de vastlegging van gegevens en de functionaliteit voor het bewerken, opvragen en presenteren daarvan.
> 3. Er wordt gebruik gemaakt van standaard infrastructurele voorzieningen die beschikbaar zijn bij de bronhouders en de gebruikers (denk hierbij aan standaardnetwerken, netwerkprotocollen en beveiligingsmechanismen).
> 4. Er wordt in de eindsituatie zoveel mogelijk uitgegaan van ‘bevragen bij de bron’. Hierbij is van belang dat de gebruiker voor verstrekkingen zoveel mogelijk uit kan gaan van één loket. Een belangrijk aandachtspunt hierbij is het gebeurtenis georiënteerd werken (nader uit te werken). Of de bronhouders gedistribueerd en decentraal werken of direct inwinning en bijhouding in een (of meerdere) voorziening(en) uitvoeren via gestandaardiseerde services moet nader bepaald worden (nadere uitwerking in kader van DiS GEO/beleidsvisie: leveranciers, bronhouders, Kadaster, VNG-R, BZK).
> 5. Er wordt ingewonnen op het niveau van de huidige schaalniveaus van BAG en BGT. De gegevens kunnen gepresenteerd worden op verschillende schaalniveaus (meest gedetailleerde weergave: 1:1.000). Autogeneralisatie voor informatie op hogere schaalniveaus moet mogelijk zijn (op basis van logica en functies). Bijvoorbeeld het (deels) afleiden van de informatie voor de BRT uit de BGT, maar ook voor het definiëren van een wegennetwerk met alle rijkswegen op basis van het gehele wegennetwerk.
> 6. Keuzen voor een technische inrichting van de registratie worden pas later in het traject gemaakt, zodat oplossingen gebaseerd zijn op recente inzichten in oplossingsmogelijkheden.
> 7. Vanuit andere (basis)registraties, zoals de subjectenregistraties BRP of HR, moeten eenvoudig relaties gelegd kunnen worden naar de samenhangende objectenregistratie.
> 8. De registratie gedraagt zich voor gebruikers zoveel mogelijk als één registratie, of het daadwerkelijk één registratie wordt, is nog niet bepaald (nader uit te werken). Daarnaast kunnen er uit de registratie (informatie)producten afgeleid worden en beschikbaar gesteld worden.
> 9. De kerngegevens en aanvullende gegevens worden in principe ontsloten als open data (waar nodig ontsloten op basis van autorisaties), dus het “open data, tenzij” regime geldt.
> 10. In principe kan de informatie via meerdere kanalen, afgestemd op gebruikersbehoefte, uitgeleverd worden (nadere uitwerking in kader van DiS GEO).

> **vanuit Architectuurvisie (Houtskoolschets) DiS-Geo**
> 11. Bronhouders zijn verantwoordelijk voor basisgegevens
> 12. Bronhouders kunnen leveranciers machtigen
> 13. Gegevens aanpassen kan makkelijk en goed
> 14. Gegevens passen bij elkaar: relaties tussen gegevens zijn voor gebruikers duidelijk, en gegevens zijn in samenhang bruikbaar
> 15. De gegevensstructuur kan snel genoeg meegroeien met de gebruiksbehoefte

### Inrichtingsprincipes vergelijkbare domeinen

De SOR staat niet op zichzelf en binnen andere domeinen is veel kennis en kunde opgebouwd over inrichtingsprincipes van dit soort ICT-voorzieningen. We hebben hier met name gebruik gemaakt van:
- De [Overall Globale Architectuur Schets (OGAS)](https://aandeslagmetdeomgevingswet.nl/publish/library/219/dso_-_gas_-_overall_gas_1.pdf) van het Digitaal Stelsel Omgevingswet.
- [NORA](#basisprincipes-nora)
- [GEMMA](#inrichtingsprincipes-gemma)
- [Common Ground](#inrichtingsprincipes-common-ground)
- 10 golden rules data, deze 10 golden rules zijn tot stand gekomen vanuit de best-practices rondom data management.


### ICT-inrichtingsprincipes Samenhangende Objectenregistratie

Voor de ICT-inrichting van de Samenhangende Objectenregistratie hanteren we de onderstaande principes. Met 'de oplossing' bedoelen we steeds de ICT-voorzieningen die de Samenhangende Objectenregistratie realiseren.

 **Inrichtingsprincipe 1: Gegevens worden gescheiden van applicaties bewaard**, *zodat* het beheren en afnemen van gegevens onafhankelijk is van de gebruikte applicaties en gegevens te (her)gebruiken zijn in verschillende applicaties voor verschillende doeleinden.
 
Grondslag: Beleidsuitgangspunten (2, 4), Common Ground 

**Inrichtingsprincipe 2: Ieder gegeven wordt op precies &eacute&eacuten plek bijgehouden**, *zodat* altijd duidelijk is wat het actuele brongegeven is en waar dat wordt beheerd. Dit principe heeft de volgende onderliggende principes in zich:
     - **Dubbele opslag betekent synchroniseren**, zodat partijen altijd naar dezelfde gegevens kijken. Dit geldt zowel binnen als buiten de oplossing, dus ook voor eventuele afgeleide opslag die geoptimaliseerd is ten behoeve van verstrekking.

Grondslag: Beleidsuitgangspunten (4, 6, 10), Common Ground (04)

**Inrichtingsprincipe 3: Gegevens zijn alleen te benaderen via dataservices**, *zodat* deze services kunnen garanderen dat de gegevens, metagegevens en de toegang ertoe altijd voldoen aan de eisen en dat logging altijd plaatsvindt. Dit principe heeft de volgende onderliggende principes in zich:
    - **Dataservices regelen de toegang tot gegevens**, *zodat* deze services ervoor kunnen zorgen dat altijd is voldaan aan de eisen betreffende toegang.
    - **Dataservices leggen elke toegang tot gegevens vast in logging**, *zodat* deze services ervoor kunnen zorgen dat aantoonbaar is wat door gemachtigde leveranciers onder verantwoordelijkheid van bronhouders plaatsvindt.
    - **Dataservices houden metadata actueel**, *zodat* data en meta-data altijd onderling consistent zijn.
    - **Dataservices borgen de gegevensregels**, *zodat* gegarandeerd is dat de gegevens altijd voldoen aan de gegevensregels. **N.B.** niet 'borgen de kwaliteit' want kwaliteit is veel breder dan alleen voldoen aan de gegevensregels.

Om te garanderen dat de gegevens blijven voldoen aan de gestelde kwaliteit en actualiteit kunnen ze alleen benaderd worden via (data)services. Dit principe zorgt ervoor dat gegevens blijven voldoen aan de (integriteits-)eisen, doordat de dataservices dit waarborgen. Ook zorgt dit principe ervoor dat er een ontkoppeling is tussen de gegevens en de ontsluiting ervan. Applicaties benaderen de gegevens via de dataservices en niet direct. Dat maakt het mogelijk om veranderingen aan te brengen in de gegevensopslag of in de dataservices zonder dat deze elkaar beïnvloeden. Hierdoor kunnen we flexibel omgaan met aanpassingen in het gegevensmodel.
De service controleert of de gebruiker wel de toegangsrechten heeft om de gegevens te maken, te lezen of aan te passen.
Alle transacties op de gegevens worden gelogd. Dit is nodig om een audit-trail te kunnen opbouwen.

Grondslag: Beleidsuitgangspunten (2, 3, 4, 11, 12, 13, 15), DSO (05)
 
**Inrichtingsprincipe 4: We bewaren en ontsluiten informatie op betrouwbare en veilige wijze**, *zodat* we kunnen aantonen dat data niet bedoeld of onbedoeld gemanipuleerd is. Om op data te kunnen vertrouwen zorgen we ervoor dat data bij alle handelingen vanaf het moment van ontstaan tot het moment van gebruik veilig is. We wijzigen de actuele versie van data daarom alleen op basis van een brondocument of mutatieverwijzing en leggen die vast. We bewaken integriteit en consistentie van data. We bewaren data conform de eisen van de wet (w.o. archiefwet, etc.).

Grondslag: Beleidsuitgangspunten (2, 4, 13), DSO (09), Common Ground (03)

**Inrichtingsprincipe 5: We maken samenhangend gebruik van data makkelijk mogelijk**, zodat data uit verschillende gegevensverzamelingen te combineren is. Zo maken we mogelijk dat er samengestelde producten over het geheel van het gegevenslandschap kunnen worden gerealiseerd. Dit principe heeft de volgende onderliggende principes in zich:
    - **alles is een service**, *zodat* zowel computers als mensen de beschikbare functies kunnen begrijpen en benutten.
    - **intern is extern**, *zodat* alle services herkenbaar en bruikbaar zijn voor externe leveranciers van bronhouders en afnemers en deze op innovatieve manieren de waarde van gegevens kunnen vergroten.

Grondslag: Beleidsuitgangspunten (7, 8, 10, 14), DSO (05)



