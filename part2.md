# Deel 2: Technische voorzieningen

Dit deel is bedoeld voor linked data specialisten en developers die willen werken met het RDA applicatieprofiel, termenlijsten en centrale toegang van Podiumkunst.net.

## Voorzieningen dataplatform

### RDA applicatieprofiel

Het Podiumkunst.net RDA-applicatieprofiel is bedoeld om collecties van podiumkunsteninstellingen met elkaar te verbinden. Dit gebeurt volgens de principes van linked data, zoals beschreven in de Digitaal Erfgoed Referentie Architectuur van het Netwerk Digitaal Erfgoed. 

Vrijwel alle andere voorzieningen maken gebruik van of zijn gebaseerd op het RDA applicatieprofiel van Podiumkunst.net. RDA biedt verschillende implementatiescenario's. Voor dit profiel is gekozen voor het Linked Open Data-scenario (implementatiescenario A), waarbij de gegevens als Linked Open Data worden gepubliceerd.

In het Podiumkunst.net RDA-applicatieprofiel staat bijvoorbeeld:

- welke soorten informatie (entiteiten) wel of niet gebruikt worden,
- welke gegevens verplicht, optioneel of juist weggelaten worden,
- hoe de gegevens worden ingevoerd,
- en welke termenbronnen bij bepaalde velden gebruikt mogen of moeten worden.

[Hier vind je het applicatieprofiel en bijbehorende documentatie](https://github.com/PodiumkunstNet/ApplicationProfileRDA) 


## Voorzieningen dienstplatform

### Centrale toegang tot verbonden collecties
Wanneer collecties gepubliceerd zijn als Linked Data, en geregistreerd zijn bij het Datasetregister en de Podiumkunst.net Knowledge Graph, zijn deze collecties centraal doorzoekbaar.

Met behulp van SPARQL-queries kunnen de aangesloten collecties bevraagd worden. De centrale toegang is een door Podiumkunst.net ontwikkelde API-laag die deze SPARQL-queries 'verbergt' en de resultaten teruggeeft in formaten die bruikbaar zijn voor web- en applicatieontwikkelaars, zoals JSON of GraphQL.

De centrale toegang is gebouwd met het oog op performance. Caching speelt hierbij een belangrijke rol.

Aangesloten datasets:
- (conceptversie) [Muziekopnamen Zendgemachtigden](https://data.beeldengeluid.nl/id/dataset/0028)
- (conceptversie) Theater Oostpool en Muziektheater De Plaats (via [PodiumArchief]())
- [Muziekschatten](https://data.muziekschatten.nl/) - Nederlandstalig klassiek

#### Wil je de centrale toegang gebruiken?
Je kunt de centrale toegang gebruiken om een nieuwe publiekstoepassing, zoals een website, mobiele app, of interactieve installatie te ontwikkelen.
Dat werkt als volgt: 

-

### Caching
Om snel te kunnen zoeken in verschillende triples stores, heeft Podiumkunst.net een cachingmechanisme gebouwd. 

## Overige voorzieningen

### Termenlijsten
Termen beschrijven waar erfgoed over gaat (zoals begrippen, personen of plaatsen) en zijn meer dan woorden, omdat ze een unieke identifier (URI) hebben die precies de betekenis vastlegt en extra informatie kan bevatten, zoals definities en synoniemen. Ze maken erfgoed beter vindbaar en worden beheerd in betrouwbare termenlijsten, die zorgen voor kwaliteit, actualiteit en duurzame beschikbaarheid.

Door Podiumkunst.net ontwikkelde termenlijsten: 
- Uitvoeringsmedium (oa instrumenten en bezettingen)

Daarnaast zijn er een aantal, al bestaande, lijsten die relevant zijn voor de podiumkunsten (via het [Termennetwerk](https://termennetwerk.netwerkdigitaalerfgoed.nl/)): 
- GTAA van Beeld & Geluid (oa geografische namen, persoonsnamen, onderwerpen)       
- Muziekschatten van SOM  (oa persoonsnamen, klassieke muziekwerken, onderwerpen)     
- Muziek van Muziekweb (oa genres, personen, groepen)       
- Nederlandse Thesaurus van Auteursnamen van de Koninklijke Bibliotheek (auteurs, ook theater)
- Regiotermen Fryslân van Tresoar (personen)
- RKDartists van de RKD (kunstenaars, ook theater)
- Thesaurus Nationaal Museum voor Wereldculturen van Stichting Nationaal Museum van Wereldculturen (begrippen, onderwerpen)
- Brinkman trefwoordenthesaurus van Brinkman (begrippen, onderwerpen)
- Wikidata (persoonsnamen, straten en plaatsnamen)


### Datasetregister
Het Datasetregister geeft inzicht in welke erfgoedcollecties er al beschikbaar zijn in Linked Data en moedigt zo aan om de datasets te gebruiken en met elkaar te verbinden.
Een dataset is een verzameling van gegevens (data of metadata).

Om een dataset toe te voegen aan het Datasetregister is een datasetbeschrijving nodig. Dit is een beschrijving (metadata) van de dataset. Een datasetbeschrijving bevat informatie die de dataset beschrijft, zoals een identificatie (URI), een naam, een inhoudsbeschrijving, een licentie, een taal en een data-eigenaar (de maker). Aanvullend op de verplichte informatie elementen kan er informatie worden gegeven over de creatiedatum, publicatiedatum, versie, contact informatie, dekking qua plaats/gebied en tijd/periode, steekwoorden en genre. Lees hier verder over de [datasetbeschrijvingen](https://datasetregister.netwerkdigitaalerfgoed.nl/faq-beheerders.php). 

#### Toevoegen van een dataset aan het Datasetregister
Voordat je een dataset toevoegt, kun je de datasetbeschrijving eerst controleren met behulp van [deze tool](https://datasetregister.netwerkdigitaalerfgoed.nl/validate.php).
Wanneer de datasetbeschrijving klopt, dan kun je de dataset aanmelden via [dit formulier](https://datasetregister.netwerkdigitaalerfgoed.nl/viaurl.php).


