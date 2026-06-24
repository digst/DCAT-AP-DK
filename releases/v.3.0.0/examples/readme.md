<img width="263" height="21" alt="billede" src="https://github.com/user-attachments/assets/0bbd685e-b18f-4b7b-b59a-05f587e52631" /># Eksempler på anvendelse af DCAT

Henvend jer gerne til arkitektur@digst.dk hvis I som dansk organisation udstiller metadata om datasæt iht. DCAT allerede, så vil vil tilføje jeres eksempler til listen herunder.

## Eksempler på anvendelse af DCAT-AP-DK 3.0.0
Se ovenstående rdf/ttl-filer.

## Eksempler på anvendelse af DCAT-AP - i Danmark
I forbindelse med arbejdet med Datavejviser og implementeringen af en række EU-retsakter er mange danske myndigheder begyndt at beskrive deres data med DCAT-AP. Disse beskrivelser er tilgængelige gennem Datavejviser i både menneske- og maskinlæsbart format. Datasætbeskrivelser kan eksporteres i forskellige RDF-serialiseringer, enten enkeltvis på siden for det givne datasæt, eller samlet ved at tilgå https://datavejviser.dk/katalog.xml. Her kan "xml" til sidst i URL'en erstattes med "jsonld", "ttl" eller "n3" efter behov.

Derudover kan det også være relevant at inspicere nogle af de endpoints, som Datavejviser henter metadata fra, fx:

* Open Data DK: https://admin.opendata.dk/catalog.xml. DCAT-feed er tilgængelige i 4 formater (xml, jsonld, ttl, n3): Erstat "xml" til sidst i URL'en med "jsonld", "ttl" eller "n3" efter behov. 

* Danmarks Miljøportal: https://datakatalog.miljoeportal.dk/api/dcat/catalogue (RDF/XML)

* Rigsarkivets digitalt skabte data: https://digidata.rigsarkivet.dk/api/dcat/v1 (RDF/XML)

* Styrelsen for Arbejdsmarked og Rekrutterings Jobindsats: https://api.jobindsats.dk/v2/digst (JSON-LD)


## Eksempler på anvendelse af DCAT - generelt
* DCAT-eksempler fra W3C: https://github.com/w3c/dxwg/tree/gh-pages/dcat/examples
