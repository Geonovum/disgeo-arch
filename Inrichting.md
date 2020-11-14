## Inrichting

### Inleiding

Dit hoofdstuk beschrijft de functionele inrichting van de Samenhangende Objectenregistratie op de applicatielaag van het NORA-vijflaagsmodel. Het doel ervan is om sturing te kunnen geven aan de transitie naar de Objectenregistratie en te dienen als kader voor technische inrichting van de Objectenregistratie. Ook biedt het een deel van de basis voor de organisatorische inrichting van de Objectenregistratie. 

Dit hoofdstuk beschrijft de onderdelen van de Objectenregistratie en de verbindingen daartussen en het wijst de functies van de Objectenregistratie toe aan deze onderdelen. 

### Functionele lagen in de inrichting

We onderscheiden drie lagen in de functionele indeling van de Objectenregistratie, zoals de afbeelding hieronder toont. Daarmee duiden we alleen het doel van de functies en doen we geen uitspraak over de de technische inrichting of de verdeling ervan over verschillende ICT-voorzieningen.

<figure id="inrichtinglagen">
    <img src="media/functionele-lagen-objectenregistratie.png" alt="functionele lagen">
    <figcaption>Functionele lagen in de inrichting van de Objectenregistratie</figcaption>
</figure>

De laag **Metabeheer** bevat de functies die nodig zijn voor het beheren en gebruiken van gegevens over de gegevens, te weten Gegevenscatalogus en Gegevenskwaliteit. Gegevenscatalogus bevat de functies die nodig zijn om informatiemodellen en gegevensregels te beheren in catalogi waarmee die informatiemodellen en gegevensregels kunnen worden toegepast in voorzieningen. Gegevenskwaliteit bevat de functies om kwaliteitsindicatoren te beheren en kwaliteitsmetingen te doen teneinde inzicht in de gegevenskwaliteit te verkrijgen.

De **Uitvoeringslaag** bevat de functies die nodig zijn voor het beheren en afnemen van objectgegevens, zoals voor het registreren en wijzigen van gegevens en voor het raadplegen ervan. Op deze laag maken we onderscheid tussen de functies ten behoeve van het beheren van objectgegevens door gebruikers in de rol van bronhouder en het afnemen van objectgegevens door gebruikers in de rol van afnemer. 

De **Ondersteuningslaag** bevat de functies die nodig zijn om bronhouders en afnemers te ondersteunen bij het beheren en afnemen van gegevens, zoals het beheren van machtigingen en het raadplegen van dienstencatalogi.

De functies in de drie lagen voor Metabeheer, Uitvoering en Ondersteuning maken we zichtbaar in een **totaaloverzicht**.

<figure id="metabeheer-inrichting-uitvoering">
    <img src="media/inrichting-metabeheer-uitvoering-ondersteuning-objectenregistratie.png" alt="inrichting metabeheer uitvoering ondersteuning">
    <figcaption>De capabilities op de lagen Metabeheer en Uitvoering en Ondersteuning</figcaption>
</figure>


### Functies in de laag Metabeheer

Op de laag **Metabeheer** onderkennen we de volgende clusters voor inzien van de gegevensstructuur en inzicht in de gegevenskwaliteit: 

- *Toegang*: voor het bewaken van de toegang van meta-beheerders tot de diensten.
- *Gegevenscatalogus*: voor het kunnen beschrijven van de in de objectenregistratie beschikbare gegevens en informatieproducten en deze beschrijving te ontsluiten, zodat bronhouders, afnemers en andere betrokkenen hier kennis van kunnen nemen.
 - *Gegevenskwaliteit*: voor het vastleggen van de afgesproken kwaliteitsindicatoren en het meten en monitoren wat de waarde van deze indicatoren is en zowel de indicatoren als de gemeten waarden beschikbaar te stellen voor bronhouders, afnemers en andere betrokkenen, zoals toezichthouders en beleidsverantwoordelijken.

### Functies in de laag Uitvoering

Op de Uitvoeringslaag onderkennen we de volgende clusters voor *beheer en afname van objectgegevens*:
- *Toegang*: voor het bewaken van de toegang van bronhouders en hun gemachtigden tot de beheerdiensten en van afnemers tot de afnamediensten. 
- *Registratie*: voor het creëren en wijzigen van objectgegevens door bronhouders en hun gemachtigden.
- *Opslag*: voor het duurzaam beschikbaar houden van objectgegevens.
- *Afname*: voor het afnemen van objectgegevens en daarvan afgeleide informatieproducten.
- *Notificatie*: voor het notificeren van afnemers van voor hen relevante gebeurtenissen die betrekking hebben op objectgegevens, zodat zij kunnen handelen naar die gebeurtenissen.
- *Terugmelding*: voor het in staat stellen van afnemers om meldingen over de juistheid van gegevens te kunnen registreren en deze beschikbaar te laten zijn voor bronhouders, zodat zij ze kunnen behandelen.

De component Terugmelding heeft als doel dat meldingen van afnemers over de juistheid van gegevens geregistreerd kunnen worden en beschikbaar zijn voor bronhouders, zodat zij ze kunnen behandelen

### Functies in de laag Ondersteuning

Op de **Ondersteuningslaag** onderkennen we de volgende clusters voor de ondersteuning van bronhouders en hun gemachtigden en afnemers:
- *Toegang*: voor het bewaken van de toegang van bronhouders en hun gemachtigden en afnemers tot de ondersteuningsdiensten.
- *Machtigingen*: voor het beheren van machtigingen voor diensten door bronhouders en afnemers. 
- *Abonnementen*: voor het kunnen registreren en beheren van abonnementen door bronhouders en afnemers op notificaties over gebeurtenissen die betrekking hebben op objectgegevens waarin ze geïnteresseerd zijn, en voor het kunnen registreren en beheren van abonnementen op Afname.
- *Betalingen*: voor het beheren van betalingen van betaalde diensten door de gebruikers van die diensten, indien sprake is van betaalde diensten. Betalen kan op verschillende manieren worden ingericht, zoals vooraf, bij afname van de dienst of achteraf, en is gekoppeld aan abonnementen.
- *Dienstencatalogus:* voor het beschrijven van de diensten van de objectenregistratie en om deze beschrijvingen (interactief) te ontsluiten, zodat betrokkenen hier makkelijk en goed kennis van kunnen nemen.



### Algemene functies

In alle drie lagen onderkennen we *Toegang* voor het bewaken van toegang tot diensten. Deze functie wordt op een plek uitgewerkt onder Algemeen. 

Verder onderkennen we de behoefte aan *Interactie* om de diensten en de gegevens en producten van de objectenregistratie aan eindgebruikers (personen in de rol van bronhouder of afnemer) te presenteren en de mogelijkheden te bieden om er mee te interacteren.

De objectenregistratie zal naar verwachting verschillende generieke interactiecomponenten bieden, bijvoorbeeld een viewer voor het zoeken en raadplegen van objectgegevens (inzage), portalen voor het beheren van machtigingen en loketten voor het indienen van terugmeldingen en het beheren van abonnementen.

Uitwerking van eisen aan Interactie staan onder Algemeen.

### Niet-functionele eisen

Aan de componenten in de drie lagen voor Metabeheer, Uitvoering en Ondersteuning, bestaan ook **niet-functionele eisen**. Deze benoemen we in algemene zin overkoepelend over de lagen en componenten.

<p class='note'>
Open vraag aan de reviewers: Welke niet-functionele eisen moeten opgenomen worden in deze Architectuurbeschrijving?
</p>


