## ICT-inrichtingsprincipes

Dit hoofdstuk beschrijft de principes die richtinggevend zijn voor de functionele inrichting van de ICT-voorzieningen voor de Objectenregistratie en de bijbehorende ICT-organisatie. 

### Beleid Samenhangende Objectenregistratie

De beleidsvisie Samenhangende Objectenregistratie (SOR), als onderdeel van DiS-Geo, beschrijft de doelstellingen en beleidscontouren van de SOR (zie: https://www.geobasisregistraties.nl/documenten/beleidsnota/2019/11/29/beleidsvisie-samenhangende-objectenregistratie). Naast de beleidsvisie is gewerkt aan een houtskoolschets voor DiS-Geo (zie: https://www.geobasisregistraties.nl/basisregistraties/documenten/publicatie/2020/06/15/dis-online-als-stroom-uit-het-stopcontact).

De volgende beleidsuitgangspunten voor de architectuur van de SOR zijn afgeleid uit de 2 bovenstaande beleidsdocumenten.

> 1. We laten ons bij het ontwerp en de verdere uitwerking niet beperken door de nu bestaande juridische kaders (deze kunnen in principe worden aangepast, via een traject aanpassing wet- en regelgeving).
> 2. In het ontwerp van een samenhangende objectenregistratie is sprake van een nadrukkelijke scheiding tussen de vastlegging van gegevens en de functionaliteit voor het bewerken, opvragen en presenteren daarvan.
> 3. Er wordt gebruik gemaakt van standaard infrastructurele voorzieningen die beschikbaar zijn bij de bronhouders en de gebruikers (denk hierbij aan standaardnetwerken, netwerkprotocollen en beveiligingsmechanismen).
> 4. Er wordt in de eindsituatie zoveel mogelijk uitgegaan van ‘bevragen bij de bron’. Hierbij is van belang dat de gebruiker voor verstrekkingen zoveel mogelijk uit kan gaan van één loket. Een belangrijk aandachtspunt hierbij is het gebeurtenis georiënteerd werken (nader uit te werken). Of de bronhouders gedistribueerd en decentraal werken of direct inwinning en bijhouding in een (of meerdere) voorziening(en) uitvoeren via gestandaardiseerde services moet nader bepaald worden (nadere uitwerking in kader van DiS GEO/beleidsvisie: leveranciers, bronhouders, Kadaster, VNG-R, BZK).
> 5. Er wordt ingewonnen op het niveau van de huidige schaalniveaus van BAG en BGT. De gegevens kunnen gepresenteerd worden op verschillende schaalniveaus (meest gedetailleerde weergave: 1:1.000). Autogeneralisatie voor informatie op hogere schaalniveaus moet mogelijk zijn (op basis van logica en functies). Bijvoorbeeld het (deels) afleiden van de informatie voor de BRT uit de BGT, maar ook voor het definiëren van een wegennetwerk met alle rijkswegen op basis van het gehele wegennetwerk.
> 6. Keuzen voor een technische inrichting van de registratie worden pas later in het traject gemaakt, zodat oplossingen gebaseerd zijn op recente inzichten in oplossingsmogelijkheden.
-Vanuit andere (basis)registraties, zoals de subjectenregistraties BRP of HR, moeten eenvoudig relaties gelegd kunnen worden naar de samenhangende objectenregistratie.
-De registratie gedraagt zich voor gebruikers zoveel mogelijk als één registratie, of het daadwerkelijk één registratie wordt, is nog niet bepaald (nader uit te werken). Daarnaast kunnen er uit de registratie (informatie)producten afgeleid worden en beschikbaar gesteld worden.
-De kerngegevens en aanvullende gegevens worden in principe ontsloten als open data (waar nodig ontsloten op basis van autorisaties), dus het “open data, tenzij” regime geldt.
-In principe kan de informatie via meerdere kanalen, afgestemd op gebruikersbehoefte, uitgeleverd worden (nadere uitwerking in kader van DiS GEO). |  | Ja  | 
-WELKE INRICHTINGSPRNCIPES WILLEN WE OVERNEMEN UIT DE HOUTSKOOLSCHETS (ALLEEN DIEGENE dIE GAAN OVER ICT (en dus niet over de gegevens).


### Inrichtingsprincipes vergelijkbare domeinen

De SOR staat niet op zichzelf en binnen andere domeinen is veel kennis en kunde opgebouwd over inrichtingsprincipes van dit soort ICT-voorzieningen. We hebben hier met name gebruik gemaakt van:
- De [Overall Globale Architectuur Schets (OGAS)](https://aandeslagmetdeomgevingswet.nl/publish/library/219/dso_-_gas_-_overall_gas_1.pdf) van het Digitaal Stelsel Omgevingswet.
- [NORA](#basisprincipes-nora)
- [GEMMA](#inrichtingsprincipes-gemma)
- [Common Ground](#inrichtingsprincipes-common-ground)


### ICT-inrichtingsprincipes Samenhangende Objectenregistratie

Voor de ICT-inrichting van de Samenhangende Objectenregistratie hanteren we de onderstaande principes. Met 'de oplossing' bedoelen we steeds de ICT-voorzieningen die de Samenhangende Objectenregistratie realiseren.

 **Inrichtingsprincipe 1: Gegevens worden gescheiden van applicaties bewaard**, *zodat* het beheren en afnemen van gegevens onafhankelijk is van de gebruikte applicaties en gegevens te (her)gebruiken zijn in verschillende applicaties voor verschillende doeleinden.

Grondslag: Verwijzingen opnemen naar de hieroor gebruikte andere principes

**Inrichtingsprincipe 2: Ieder gegeven wordt op precies &eacute&eacuten plek bijgehouden**, *zodat* altijd duidelijk is wat het actuele brongegevens is en waar dat wordt beheerd.

Grondslag: 

**Inrichtingsprincipe 3: Gegevens zijn alleen te benaderen via dataservices**, *zodat* deze services kunnen garanderen dat de gegevens, metagegevens en de toegang ertoe altijd voldoen aan de eisen en dat logging altijd plaatsvindt. Dit was: "een bron - een waarheid".
 
Grondslag:  
 
**Inrichtingsprincipe 4: Datasservices controleren het beheer en de afname van gegevens**, *zodat* de services kunnen garanderen dat de gegevens, metagegevens en de toegang ertoe altijd voldoen aan de eisen en dat logging altijd plaatsvindt. N.B. als dit de correcte '*zodat*' is, dan is dit principe hetzelfde als het vorige principe en moeten we ze samenvoegen tot 1. Dit principe heeft de volgende onderliggende principes in zich:
    - **Dataservices regelen de toegang tot gegevens**, *zodat* deze services ervoor kunne zorgen dat altijd is voldaan aan de toegangseisen.
    - **Dataservices houden metadata actueel**, *zodat* data en meta-data altijd onderling consistent zijn.
    - **Dataservices borgen de gegevensregels**, *zodat* gegarandeerd is dat de gegevens altijd voldoen aan de gegevensregels. **N.B.** niet 'borgen de kwaliteit' want kwaliteit is veel breder dan alleen volgoen aan de gegevensregels.

Grondslag

**Inrichtingsprincipe 5: We bewaren en ontsluiten informatie op betrouwbare en veilige wijze**, *zodat* om op data te kunnen vertrouwen is het nodig om aan te tonen dat data niet bedoeld of onbedoeld gemanipuleerd is. Daarom zorgen we ervoor dat data bij alle handelingen vanaf het moment van ontstaan tot het moment van gebruik veilig is. We wijzigen data daarom op basis van een brondocument of mutatieverwijzing. We bewaken integriteit en consistentie van data. We bewaren data conform de eisen van de wet (w.o. archiefwet, etc.).

Grondslag

**Inrichtingsprincipe 6: We maken de samenhang van data inzichtelijk**, zodat om data uit verschillende gegevensverzamelingen te kunnen combineren is het nodig om de samenhang te kennen. Zo maken we mogelijk dat er samengestelde producten over het geheel van het gegevenslandschap kunnen worden gerealiseerd.

Grondslag





**Gegevens en functionaliteit zijn gescheiden**

Gegevens kunnen alleen worden benaderd via dataservices. Onder 'benaderen' verstaan we het maken, lezen en aanpassen van gegevens.
Gegevens worden nooit verwijderd, maar *gemarkeerd* als 'verwijderd'. Applicaties kunnen alleen via de dataservices gegevens maken, lezen en aanpassen. Onderstaande afbeelding uit de API-strategie geeft dit weer.

<p class='note'>
    WB: Bij Common Ground betekent dit principe dat gegevens los van applicaties worden opgeslagen. Het betekent bij Common Ground niet dat gegevens alleen via services te benaderen zijn. Dat is bovendien een op zichzelf staand principe dat we verderop formuleren. Beide principes zijn wel relevant, maar hebben allebei een andere rationale. Zie mijn lijstje hierboven.
</p>

<figure id="apitoegang">
    <img src="https://docs.geostandaarden.nl/api/API-Strategie/media/clip02.png" alt="apitoegang">    
    <figcaption>Gegevens kunnen alleen worden benaderd via dataservices.</figcaption>
</figure>

De ontkoppeling en interoperabiliteit van de gegevens maken verandering mogelijk (middels API strategie en URI strategie)

**De oplossing zorgt dat af te nemen gegevens altijd actueel zijn**

Alle mutaties vinden plaats op de samenhangende gegevensset. Een wijziging aan een gegeven wordt genotificeerd. Daardoor kunnen afnemers zorgen dat ze actuele gegevens blijven afnemen.

**E&eacuten bron - &eacute&eacuten waarheid**
De oplossing zorgt ervoor dat ieder gegeven in &eacute&eacuten bron wordt bijgehouden. Dit voorkomt dat er meerdere bronnen voor hetzelfde gegeven bestaan. 

**Dubbele opslag betekent synchroniseren**
Partijen die, om wat voor reden dan ook, een kopie dataset willen beheren, kunnen en mogen dat doen, maar zijn dan zelf verantwoordelijk voor het up-to-date houden van die gegevensset.  

Dit geldt zowel binnen als buiten de oplossing, dus ook voor eventuele afgeleide opslag die geoptimaliseerd is ten behoeven van verstrekking.

<p class='note'>
    WB: Dat een afnemer die een eigen kopie heeft zelf verantwoordelijk is voor het synchroniseren, is een organisatorische afspraak, geen ICT-inrichtingsprincipe.
</p>

**Gegevens kunnen alleen via Dataservices worden benaderd**
Om te garanderen dat de gegevens blijven voldoen aan de gestelde kwalteit en actualiteit kunnen ze alleen benaderd 
worden via *Dataservices*. Directe toegang tot de gegevens vanuit applicaties is ten strengste verboden. 

Dit principe zorgt ervoor dat gegevens blijven voldoen aan de (integriteits-)eisen, doordat de dataservices dit waarborgen. Ook zorgt dit principe ervoor dat er een ontkoppeling is tussen de gegevens en de ontsluiting ervan. Dat maakt het mogelijk om veranderingen aan te brengen in de gegevensopslag of in de dataservices zonder dat deze elkaar beïnvloeden.

**Dataservices controleren**
Alle controles, of het nou gaat om toegangscontrole tot de gegevens, of kwaliteitscontroles worden gedaan door
de dataservices, en niet door applicaties. Zoals al eerder gezegd: aplicaties benaderen de gegevens via de dataservices en niet direct.
Applicaties zorgen wel voor een nette foutafhandeling: als een service een foutcode retourneet, zorgt de applicatie
voor de afhandeling van die fout door het geven van een melding, of door een nieuwe aanroep van de dataservice.

- *Dataservices loggen de transacties op de gegevens*
Alle (!) transacties op de gegevens worden gelogd. Dit is nodig om een audit-trail te kunnen opbouwen.

- *Dataservices houden metadata up-to-date*
Waar mogelijk wordt de metadata door de dataservices up-to-date gehouden. Denk hierbij aan datum laatste mutatie, door wie gemuteerd, enz.

- *Dataservices controleren*
Alle controles, of het nou gaat om toegangscontrole tot de gegevens, of kwaliteitscontroles worden gedaan door
de dataservices, en niet door applicaties. Zoals al eerder gezegd: aplicaties benaderen de gegevens via de dataservices en niet direct.
Applicaties zorgen wel voor een nette foutafhandeling: als een service een foutcode retourneet, zorgt de applicatie
voor de afhandeling van die fout door het geven van een melding, of door een nieuwe aanroep van de dataservice.

- *Dataservices regelen de toegang tot de gegevens*
Bij het aanroepen van de dataservices wordt gecontroleerd of de gebruiker de gegevens wel mag benaderen.
Benaderen kan weer zijn: maken, lezen en aanpassen. De dataservice controleert of de gebruiker wel de rechten
heeft om de gegevens te maken, te lezen of aan te passen. Wat een gebruiker mag wijzigen hangt ook van de *klassificatie*
van de gegevens af. 

- *Dataservices loggen de transacties op de gegevens*
Alle (!) transacties op de gegevens worden gelogd. Dit is nodig om een *audit-trail* te kunnen opbouwen.

- *Dataservices borgen de kwaliteit van de gegevens*
Alle (!) controles die moeten plaatsvinden voordat een gegeven wordt gewijzigd worden in de dataservice gedaan.  

Enkele voorbeelden van een kwailiteitscheck: 
- domeinwaarde check: komt de nieuwe waarde voor in een lijst met geldige waarden, of ligt de nieuwe waarde tussen twee grenswaarden.
- datum check: is de waarde volgens een bepaald datum formaat.
- type check: is de nieuwe waarde wel van een bepaald datatype.
- referentie check: mag een gegeven worden gemarkeerd als verwijderd, terwijl het gegeven nog ergens anders bestaat? 

**Het Gegevensmodel is flexibel en aanpasbaar**  

<p class='note'>
     JvG: Dit principe is toegevoegd, maar nog niet besproken in de groep architectuur 
</p>

Een uitgangspunt voor het gegevensmodel van de SOR is dat het informatiemodel flexibel moet zijn. Eenvoudig aan te passen, en het onderscheid tussen verplichte en vrijwillige objecten in de registratie moet niet diepgaand in het uitgewerkte gegevensmodel worden verankerd.  
De oplossing moet met deze flexibiliteit in het gegevensmodel om kunnen gaan zodat het weinig impact heeft op de dataservices, en daarmee de applicaties die van die services gebruik maken, als er iets wijzigt. 

