## ICT-inrichtingsprincipes

<p class='note'>
     WB: Ik heb dit hoofdstuk beperkt tot de inrichtingsprincipses voor de SOR en de context en achtergrond grotendeels verplaatst naar de bijlagen. De lezer hoeft alleen het resultaat te zien. Als de lezer geinteresseerd is in de achtergronden en afwegingen dan zijn deze in de bijlage te vinden.
</p>

### Inleiding

Dit hoofdstuk bevat de principes die richtinggevend zijn voor de functionele (en deels ook de technische) inrichting van de ICT-voorzieningen voor de Objectenregistratie. 

Bij het opstellen van de principes zijn de volgende bronnen gehanteerd:
- De beleidsvisie DiS Geo, (of "de [houtskoolschets](https://www.geobasisregistraties.nl/basisregistraties/documenten/publicatie/2020/06/15/dis-online-als-stroom-uit-het-stopcontact)").
- De [Overall Globale Architectuur Schets (OGAS)](https://aandeslagmetdeomgevingswet.nl/publish/library/219/dso_-_gas_-_overall_gas_1.pdf) van het Digitaal Stelsel Omgevingswet. Bij het opstellen van de architectuurschets voor het DSO is recent gekeken naar diverse andere relevante richtinggevende principes zoals [NORA](#basisprincipes-nora), [GEMMA](#inrichtingsprincipes-gemma) en [Common Ground](#inrichtingsprincipes-common-ground) en is een hanteerbare set principes afgeleid.
- Internationale architectuurprincipes van W3C, en met name  de principes uit [Spatial Data on the Web Best Practices](https://www.w3.org/TR/sdw-bp/#bp-summary) die zijn opgetekend op basis van vele internationale ervaringen met het omgaan met geo-gegevens. 

<p class='note'>
     WB: Is bovenstaande opsomming volledig? We moeten nog toetsen in hoeverre de 'web best practices' nog relevant zijn, omdat we geconstareerd hebben dat deze vooral over de inhoud gaan en minder over de functionele ICT-inrichting. Ook moeten we nog toetsen in hoeverre we nog voortbouwen op de principes van het DSO.
</p>

<p class='note'>
     WB: Ik heb de paragraaf mbt het doel van de SOR verplaatst naar het hoofdstuk Afbakening.
</p>

<p class='note'>
     WB: Ik heb Inrichtingsprincipes van DSO, Spatial Data en Common Ground verplaatst naar de bijlagen.
</p>

<p class='note'>
    WB: Ik heb ook de verantwoording aan de DiS Geo / Houtskoolschets principes verplaatst naar de bijlage. 
</p>


### Inrichtingsprincipes Samenhangende Objectenregistratie

De inrichtinsprincipes voor de Samenhangende Objecten Registratie zijn, gebaseerd op DSO, best practices, en Common Ground, samengevat de volgende:

**Gegevens en functionaliteit zijn gescheiden**
Gegevens kunnen alleen worden benaderd via dataservices. Benaderen is maken, lezen en aanpassen van gegevens.
Gegevens worden nooit verwijderd, maar *gemarkeerd* als verwijderd.
Applicaties kunnen alleen via de dataservices gegevens maken, lezen en aanpassen.  

De Ontkoppeling en interoperabiliteit van de gegevens maken verandering mogelijk (middels API strategie en URI strategie)

**De oplossing zorgt dat af te nemen gegevens altijd actueel zijn**
Alle mutaties vinden plaats op de samenhangende gegevensset. Een wijziging aan een gegeven wordt genotificeerd. Daardoor kunnen afnemers zorgen dat ze actuele gegevens blijven afnemen.

**E�n bron - ��n waarheid**
De oplossing zorgt ervoor dat ieder gegeven in ��n bron wordt bijgehouden. We voorkomen dat er meerdere bronnen voor hetzelfde gegeven bestaan. 

**Dubbele opslag betekent synchroniseren**
Partijen die, om wat voor reden dan ook, een kopie dataset willen beheren, kunnen en mogen dat doen, maar dan zijn zij zelf verantwoordelijk voor het up-to-date houden van die gegevensset.  

Dit geldt zowel binnen als buiten de oplossing, dus ook voor de voorziening voor verstrekking.

**Gegevens kunnen alleen via Dataservices worden benaderd**
Om te garanderen dat de gegevens blijven voldoen aan de gestelde kwalteit en actualiteit kunnen ze alleen benaderd 
worden via *Dataservices*. Directe toegang tot de gegevens vanuit applicaties is ten strengste verboden.  

**Dataservices loggen de transacties op de gegevens**
Alle (!) transacties op de gegevens worden gelogd. Dit is nodig om een audit-trail te kunnen opbouwen.

**Dataservices houden metadata up-to-date**
Waar mogelijk wordt de metadata door de dataservices up-to-date gehouden. Denk hierbij aan datum laatste mutatie, door wie gemuteerd, enz.

*Dataservices controleren*
Alle controles, of het nou gaat om toegangscontrole tot de gegevens, of kwaliteitscontroles worden gedaan door
de dataservices, en niet door applicaties. Zoals al eerder gezegd: aplicaties benaderen de gegevens via de dataservices en niet direct.
Applicaties zorgen wel voor een nette foutafhandeling: als een service een foutcode retourneet, zorgt de applicatie
voor de afhandeling van die fout door het geven van een melding, of door een nieuwe aanroep van de dataservice.

*Dataservices regelen de toegang tot de gegevens*
Bij het aanroepen van de dataservices wordt gecontroleerd of de gebruiker de gegevens wel mag benaderen.
Benaderen kan weer zijn: maken, lezen en aanpassen. De dataservice controleert of de gebruiker wel de rechten
heeft om de gegevens te maken, te lezen of aan te passen. Wat een gebruiker mag wijzigen hangt ook van de *klassificatie*
van de gegevens af. 

*Dataservices loggen de transacties op de gegevens*
Alle (!) transacties op de gegevens worden gelogd. Dit is nodig om een *audit-trail* te kunnen opbouwen.

*Dataservices borgen de kwaliteit van de gegevens*
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



