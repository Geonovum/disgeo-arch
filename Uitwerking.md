## Uitwerking onderdelen inrichting Objectenregistratie

### Inleiding

Dit hoofdstuk beschrijft de nadere uitwerking van de functionele onderdelen van de Objectenregistratie en hun interne en externe verbindingen. 

<p class='note'>
     Deze nadere uitwerking volgt. Beschrijving vindt plaats parallel aan de review op de afbakening en inrichting.
</p>
 
 <!-- Als commentaar even alle componenten opgenomen tbv volgende stap (door Marcel):
 
De laag **Metabeheer** bestaat uit de delen **Metagegevensbeheer** en **Inzicht in kwaliteit**. 

Het deel Metagegevensbeheer bevat de volgende clusters aan functionaliteiten:
- *Toegang*: voor het bewaken en loggen van de toegang van meta-beheerders tot de beheerdiensten.
- *Informatiemodel*: voor het beheren van het informatiemodel, de gegevensregels en de bijbehorende gegevens- en dienstencatalogi.

Het deel 'Inzicht in kwaliteit' bevat de volgende clusters aan functionaliteiten:
 - *Toegang*: voor het bewaken en loggen van de toegang van meta-beheerders tot de diensten.
 - *kwaliteitsindicatoren*: voor het beheren van de door bronhouders en afnemers en andere betrokkenen (zoals toezichthouder en  beleidsverantwoordelijke) overeengekomen kwaliteitsindicatoren en bijbehorende diensten
 - *Kwaliteitsmetingen:* Voor het bepalen van de waarden van de kwaliteitsindicatoren ten behoeve van monitoring van de algehele kwaliteit, bijvoorbeeld door middel van analyses

De laag **Uitvoering** bevat de functies voor het beheren van objectgegevens en voor het afnemen van objectgegevens

Op de Uitvoeringslaag onderkennen we de volgende clusters voor *beheer van objectgegevens*:
- *Toegang*: voor het bewaken en loggen van de toegang van bronhouders en hun gemachtigden tot de beheerdiensten.
- *Registratie*: voor het creëren en wijzigen van objectgegevens door bronhouders en hun gemachtigden.
- *Opslag*: voor het duurzaam beschikbaar houden van gegevens over objecten en objecteigenschappen.

Op de Uitvoeringslaag onderkennen we daarnaast de volgende clusters voor het *afnemen van objectgegevens* :
- *Afgeleide opslag*: voor het beschikbaar maken van gegevens afgestemd op de specifieke behoeften van het afnemen van objectgegevens door grote aantallen afnemers.
- *Afname gegevens*: voor het afnemen van objectgegevens op verschillende manieren, variërend van het raadplegen van enkelvoudige gegevens tot afnamen in 'bulk' voor bijvoorbeeld analysedoeleinden.
- *Notificatie*: voor het notificeren van afnemers van voor hen relevante gebeurtenissen (we gebruiken gebeurtenissen hier in brede zin, breder dan alleen gebeurtenissen die de objectgegevens betreffen)
- *Afname informatie*: voor het afnemen van generieke informatieproducten op verschillende manieren. Het visueel raadplegen van basisgegevens in context (viewer) is zo'n informatieproduct. Ook gecombineerde afname die een afgesproken generieke behoefte van afnemers invult kan zo'n informatieproduct zijn.
- *Terugmelding*: voor het in staat stellen van afnemers om bij gerede twijfel aan de juistheid van gegevens dit te melden.
- *Toegang*: voor het bewaken en loggen van de toegang van afnemers tot de afnamediensten. 


Op de laag **Ondersteuning** onderkennen we de volgende clusters voor de ondersteuning van bronhouders en afnemers en hun gemachtigden en leveranciers:
- *Toegang*: voor het bewaken en loggen van de toegang van bronhouders en afnemers tot de ondersteuningsdiensten.
- *Beheer toegang*: voor het beheren van autorisaties op gegevens en diensten door bronhouders en afnemers zelf en eventueel ook door de beheerder van de ICT-voorziening(en).
- *Beheer abonnementen*: voor het beheren van abonnementen op notificaties van gebeurtenissen door bronhouders en afnemers
- *Beheer betalingen*: voor het beheren van de betalingen van betaalde diensten door de gebruikers van die diensten, indien sprake is van betaalde diensten. Betalen kan op verschillende manieren worden ingericht, zoals vooraf, bij afname van de dienst of achteraf.
- *Beheer kwaliteitsdashboard*: voor het inzien van de waarden van kwaliteitsindicatoren per bronhouder of groep van bronhouders (algehele kwaliteit wordt gemeten in de laag Metabeheer, zie onderdeel Inzicht in Kwaliteit)
- *Beheer gegevenscatalogus*: voor het inzien van de beschikbare soorten objectgegevens, eigenschappen en relaties en de betekenis daarvan, evenals het uitvoeren van versiemanagement op de catalogus als er sprake is van nieuwe objectgegevens of gegevensregels (vanuit metagegegevensbeheer)
- *Dienstencatalogus:* voor het inzien van de beschikbare gegevensproducten en diensten voor het beheren en afnemen ervan, evenals voor het uitvoeren van versiemanagement op de dienstencatalogus als er sprake is van nieuwe diensten zoals gegevensdiensten (dataservices), informatiediensten (afname informatie) of abonnementsdiensten op notificaties 

De onderliggende laag **Voorzieningenbeheer** bevat de volgende clusters aan functionaliteiten:
 - *Toegang*: voor het bewaken en loggen van de toegang van voorzieningingenbeheerders.
 - *Autorisatievormen*: voor het beheren van de beschikbare autorisatievormen.
 - *Abonnementsvormen*: voor het beheren van de beschikbare abonnementsvormen.
 - *Betalingsvormen*: voor het beheren van de beschikbare betalingsvormen.
 - *Dienstvormen*: voor het beheren van de beschikbaren dienstvormen.
 - *Metingen*: voor het uitvoeren van metingen en raadplegen van uitgevoerde metingen en beschikbaar meetgegevens, zoals aantallen gebruiker.
 
 Als we alle clusters met functionaliteiten in één overzicht plaatsen, wordt het geheel minder overzichtelijk. Het kan mogelijk wel nuttig zijn zo'n overzicht als praatplaat-aan-de-wand te gaan gebruiken bij de beheerorganisatie(s) bijvoorbeeld in workshops die bij de gezamenlijke inrichting worden gehouden. 
 
 <figure id="alles in een plaat">
    <img src="media/alles-in-een-plaat.png" alt="alles in een plaat">
    <figcaption>Alle capability-clusters in een plaat</figcaption>
</figure>

-->

###Uitwerking Metabeheer

###Uitwerking Uitvoering

###Uitwerking Ondersteuning

###Uitwerking Beheer van voorzieningen (algemeen)

API-strategie
URI-strategie
Technische standaarden
-	Aanwijzingen/kaders voor technology stack
Standaarden
-	Verwijzing naar inhoudelijke?? Standaarden zoals NTA8035 etcetera NEN3610/2610
-	Relatie met Forum Standaardisatie Logius, NORA, GEMMA, PETRA, WILMA etcetera.


 - *Toegang*: hier maken we gebruik van generieke componenten uit de Generieke Digitale Infrastructuur (GDI) conform de Wet digitale overheid (Wdo) zoals eHerkenning en digikoppeling en opvolgende authenticatiemiddelen (iDIN, DigiD, eIDAS etc.) 
 
 De Wet digitale overheid heeft als doel het regelen van het veilig en betrouwbaar kunnen inloggen voor Nederlandse burgers en bedrijven bij de (semi-)overheid. De wet stelt daarnaast open standaarden verplicht. Hiermee implementeert Nederland de EU richtlijn over toegankelijkheid van overheidswebsites en apps.
Wet Digitale Overheid
De wet verankert taken, verantwoordelijkheden en bevoegdheden mbt de voorzieningen voor de generieke digitale infrastructuur (GDI), verplichtingen voor bestuursorganen en aanspraken van burgers en bedrijven. Gewerkt wordt in tranches; de eerste tranche regelt onder meer de toegang tot digitale dienstverlening van de overheid middels elektronische identificatie/authenticatie, informatieveiligheid en standaarden.
 
 - *Autorisatievormen*: voor het beheren van de beschikbare autorisatievormen.
 - *Abonnementsvormen*: voor het beheren van de beschikbare abonnementsvormen.
 - *Betalingsvormen*: voor het beheren van de beschikbare betalingsvormen.
 - *Dienstvormen*: voor het beheren van de beschikbaren dienstvormen.
 - *Metingen*: voor het uitvoeren van metingen en raadplegen van uitgevoerde metingen en beschikbaar meetgegevens, zoals aantallen gebruiker.



###Cross-check:

Wanneer er duidelijkheid komt over de rollen en bijbehorende taken, bevoegdheden en verantwoordelijkheden, kunnen we controleren dat alle activiteiten van alle rollen zijn benoemd en beschreven door de activiteiten per rol op te sommen, en aan te geven in welk cluster van functionaliteiten de bijbehorende functie/capability staat om die activiteit mogelijk te maken.
 
Uitwerking van functies die nodig zijn voor activiteiten

De huidige en nieuwe ondersteunende activiteiten behoren (geheel of gedeeltelijk) bij één of meer van de volgende formele (stelsel) rollen:

• Bronhouder : gegevensleverancier, ondersteuning bronhouders, kwaliteitsmanagement (dashboard ter ondersteuning van de bijhouding), beheer voorziening (mutatievoorzieningen en opslag voor bronhouders) en leveren software (registratiesoftware)

bronhouden
gegevens ontvangen
bronhouders ondersteunen
bijhouding ondersteunen met inzicht in kwaliteit via een dashboard per bronhouder
voorzieningbeheer van registratiefunctionaliteit (inname service)
softwarelevering aan voorzieningenbeheer



• Verstrekker: beheer voorziening (verstrekkingsvoorzieningen en opslag voor verstrekking)

verstrekken
gegevens leveren
generieke informatieproducten leveren
afnemers ondersteunen
afname ondersteunen met inzicht in kwaliteit via een dashboard voor gebruikers

voorzieningbeheer van verstrekkingsfunctionaliteit (uitgifte service)
softwarelevering aan voorzieningenbeheer



• Afnemer: beheer informatiedienst, kwaliteitsmanagement (dashboard ten behoeve van inzicht in gegevenskwaliteit voor gebruikers) en leveren software (software voor gebruik in afnemende processen)

• Toezichthouder: kwaliteitsmanagement (dashboard met indicatoren ter ondersteuning van de oordeelvorming door toezicht en handhaving)

• Beleidsverantwoordelijke : beheer standaarden (in afstemming met bronhouders en afnemers)
 