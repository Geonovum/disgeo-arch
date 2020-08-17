## Inrichting van de Objectenregistratie

<p class='note'>
     WB: Dit hoofdstuk heb ik deels aangepast en moet nog verder worden uitgewerkt. 
</p>

### Inleiding

Dit hoofdstuk beschrijft de functionele (of conceptuele) inrichting van de Samenhangende Objectenregistratie op de applicatielaag van het NORA-vijflaagsmodel. Het doel ervan is om sturing te kunnen geven aan de transitie naar de Objectenregistratie en te dienen als kader voor technische inrichting van de Objectenregistratie. Ook biedt het eenn basis voor de organisatorische inrichting van de Objectenregistratie. 

Dit hoofdstuk beschrijft de onderdelen of componenten van de Objectenregistratie en de verbindingen daartussen en het wijst de functies van de Objectenregistratie toe aan deze onderdelen. Het beschrijft ook de benodigde standaarden voor de Objectenregistratie en de relatie met de inhoud van de Objectenregistratie (op de gegevenslaag van het NORA vijflaagsmodel).

### Functionele lagen in de inrichting

We onderscheiden vier lagen in de functionele inrichting van de Objectenregistratie, zoals de afbeelding hieronder toont.

<figure id="inrichtinglagen">
    <img src="media/inrichting-lagen-sor.png" alt="inrichtinglagen">
    <figcaption>Lagen in de inrichting van de Objectenregistratie</figcaption>
</figure>

De **uitvoeringslaag** bevat de functies die nodig zijn voor het voor het beheren en afnemen van objectgegevens, zoals voor het registreren en wijzigen van gegevens en voor het raadplegen ervan. Op deze laag maken we onderschied tussen de functies ten behoeve van het beheren van objectgegevens door bronhouders en het afnemen ervan door afnemers van de Objectenregistratie.

De **ondersteuningslaag** bevat de functies die nodig zijn om bronhouders en afnemers te ondersteunen bij het beheren en afnemen vna gegevens, zoals het beheren van autorisaties en het raadplegen van gegevens- en dienstencatalogi.

De volgende laag bevat de functies die betrekking hebben op het beheren van meta-data en bestaat uit twee delen: **Meta-gegevensbeheer** en **'Inzicht in kwaliteit'**. Meta-gegevensbeheer bevat de functies die nodig zijn om informatiemodellen, gegevensregels en gegevens- en dienstencatalogi te beheren. 'Inzicht in kwaliteit' bevat de functies om kwaliteitsindicatoren te beheren en kwaliteitsanalyses te doen.

De laag **Platformbeheer** bevat de functies voor het beheren van het platform, of de platformen, die het beheren en afnemen van objectgegevens en meta-gegevens mogelijk maken.

### Functies in de lagen Uitvoering en Ondersteuning

De lagen Uitvoering en Ondersteuning bevatten de functies voor: 1) het beheren en afnemen van objectgegevens en 2) ondersteuning van bronhouders en afnemers. Onderstaande afbeelding toont de clusters van functionaliteiten op deze lagen.

<figure id="inrichtinguitvoeringondersteuning">
    <img src="media/inrichting-uitvoering-ondersteuning-sor.png" alt="inrichtinguitvoeringondersteuning">
    <figcaption>De capability-clusters op de lagen Uitvoering en Ondersteuning</figcaption>
</figure>

Op de **uitvoeringslaag** onderkennen we de volgende clusters voor beheer van objectgegevens:
- Toegang: voor het bewaken en loggen van de toegang van bronhouders en gemachtigden tot de beheerdiensten.
- Registratie: voor het creëren en wijzigen van objectgegevens door bronhouders en gemachtigden.
- Opslag: voor het duurzaam beschikbaar houden van gegevens over objecten en objecteigenschappen.

Voor het afnemen van objectgegevens onderkennen we de volgende clusters:
- Afgeleide opslag: voor het beschikbaar maken van gegevens afgestemd op de specifieke behoeften van het afnemen van objectgegevens door grote aantallen afnemers.
- Afname: voor het afnemen van objectgegevens op verschillende manieren, variërend van het raadplegen van enkelvoudige gegevens tot 'bulk' afnamen, bijvoorbeeld voor analysedoeleinden.
- Notificatie: voor het notificeren van afnemers van voor hen relevante gebeurtenissen (we gebruiken gebeurtenissen hier in brede zin, breder dan alleen gebeurtenissen die de objectgegevens betreffen)
- Terugmelding: voor het in staat stellen van afnemers om bij gerede twijfel aan de juistheid van gegevens dit te melden.
- Toegang: voor het bewaken en loggen van de toegang van afnemers tot de afnamediensten. 

<p class='note'>
     WB: In afbeelding Notificeren veranderen in Notificatie. De clusters hebben zelfstandige naamwoorden als naam. 
</p>

Op de **ondersteuningslaag** onderkennen we de volgende clusters voor de ondersteuning van bronhouders en afnemers en hun gemachtigden en leveranciers:

<p class='note'>
     WB: TOT HIER GEKOMEN 17-8-2020 
</p>

Onderstaande afbeelding toont de functionaliteiten per cluster op deze twee lagen.

<figure id="functiesuitvoeringondersteuning">
    <img src="media/functies-uitvoering-ondersteuning-sor.png" alt="functiesuitvoeringondersteuning">
    <figcaption>De capabilities op de lagen Uitvoering en Ondersteuning</figcaption>
</figure>



### Functies in de laag Meta-gegevensbeheer en Inzicht in kwaliteit

### Functies in de laag Platformbeheer

### Componenten en samenhang

(waaronder de landelijke en bronhouderonderdelen)

### Benodigde standaarden

### Relatie met de inhoud van de Objectenregistratie

Op de gegevenslaag van het NORA vijflaagsmodel