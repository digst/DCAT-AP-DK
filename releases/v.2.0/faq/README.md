
# FAQ om beskrivelse af datasæt og datakataloger med DCAT (under udvikling)

I FAQ'en finder du svar på spørgsmål vedrørende beskrivelse af datasæt og datakataloger i henhold til DCAT-vokabularet og den europæiske og danske anvendelsesprofil. I første omgang guider svarene primært videre til uddybende indhold om disse modeller og relaterede eksterne dokumenter, men denne faq kan udbygges efter behov.



<!-- 
## Hvordan finder nye anvendere frem til et udgivet datasæt
Anvendelse af DCAT og bagvedliggende metamodel -->

## Hvordan giver man datasæt gode titler og beskrivelser?
https://diggsweden.github.io/DCAT-AP-SE/docs/recommendations.html#1-bra-namn-ska-vara-korta-och-beskrivande
https://diggsweden.github.io/DCAT-AP-SE/docs/recommendations.html#2-%C3%B6vers%C3%A4tt-fritextf%C3%A4lt-till-andra-spr%C3%A5k

## Hvorfor skal man oprette en identifikator og hvordan oprettes de?
Læs mere her: https://arkitektur.digst.dk/rammearkitektur/datastandarder/retningslinjer-stabile-http-urier (Revision på vej) ; 
https://joinup.ec.europa.eu/collection/semantic-interoperability-community-semic/document/10-rules-persistent-uris
https://joinup.ec.europa.eu/release/dcat-ap-how-use-identifiers-datasets-and-distributions

## Hvordan skelner man mellem mulighederne for angivelse af hvordan man får adgang til datasættet?
- Destinationsside (på dcat:Resource): Se https://www.w3.org/TR/vocab-dcat-2/#Property:resource_landing_page 
En destinationsside er en webside som der kan navigeres til i en webbrowser for at få adgang til kataloget, et datasæt, dets distributioner og/eller yderligere information.

- Adgangs-URL (på dcat:Distribution): Se https://www.w3.org/TR/vocab-dcat-2/#Property:distribution_access_url
En adgangs-URL er en URL for en ressource som giver adgang til en distribution af datasættet. Fx, destinationsside, feed, SPARQL-endpoint. Anvendes i alle sammenhænge undtagen til angivelse af et simpelt download link hvor anvendelse af egenskaben download-URL foretrækkes.

- Dataadgangstjeneste (på dcat:Distribution): se https://www.w3.org/TR/vocab-dcat-2/#Property:distribution_access_service
Et websted eller endpoint der giver adgang til distributionen af datasættet. dcat:accessService BØR anvendes til at angive et link til en beskrivelse af en dcat:DataService som kan give adgang til distributionen.

- Download-Url (på dcat:Distribution): se https://www.w3.org/TR/vocab-dcat-2/#Property:distribution_download_url
Download-Url er en URL til fil der kan downloades i et bestemt format. Fx en CSV-fil eller en RDF-fil. Formatet for distributionen angives ved hjælp af egenskaberne dct:format og/eller dcat:mediaType. dcat:download-URL BØR anvendes til angivelse af den adresse hvor distributionen er tilgængelig direkte, typisk gennem et HTTP Get request

OBS: Hvis en eller flere distributioner kun er tilgængelige via en destinationsside (dvs. en URL til direkte download er ikke kendt), så bør destinationssidelinket gentages som adgangsadresse for en distribution 

Se eksempler her: https://www.w3.org/TR/vocab-dcat-2/#example-landing-page


## Hvordan sikrer man god datakvalitet i de udgivne datasæt
Til at beskrive kvalitetsrelaterede informationer af DCAT-datasæt og -distributioner anvendes [Data on the Web Best Practices: Data Quality Vocabulary](https://www.w3.org/TR/vocab-dqv/). [Fælles sprog for datakvalitet](https://arkitektur.digst.dk/metoder/faelles-sprog-datakvalitet) (Vejledning til deklaration af datasæt med kernedimensioner vers. 1.0.0) anvender også DQV.

Læs mere her: https://www.w3.org/TR/vocab-dcat-2/#quality-information; https://www.w3.org/TR/vocab-dqv/; https://arkitektur.digst.dk/metoder/faelles-sprog-datakvalitet;  https://github.com/w3c/dxwg/wiki/Quality-documentation

## Hvordan kan man understøtte god datakvalitet i DCAT-metadatabeskrivelser?
Ved hjælp af SHACL-implementeringen af den danske anvendelsesprofil er det muligt at validere indholdet af en given DCAT-metadatabeskrivelse iht. DCAT-AP-DK og adressere flere kernekvalitetsdimensioner. Hvis den obligatoriske information mangler eller hvis obligatoriske, anbefalede eller valgfrie elementer er ikke er angivet korrekt, kan en validator baseret på SHACL-indholdet give relevante valideringsresultater og beskeder.   

Læs mere her: https://github.com/digst/DCAT-AP-DK/tree/master/releases/v.2.0/validation



## MODELLERING AF VERSIONER OG TIDSSERIER

### Hvordan skal versioner beskrives?
Læs mere her: https://github.com/w3c/dxwg/wiki/Dataset-(and-other-DCAT)-versioning
Note: info om arkiverede data.

### Hvordan beskriver man tidsserier?
Læs mere her: https://joinup.ec.europa.eu/release/dcat-ap-how-model-dataset-series og
https://github.com/w3c/dxwg/issues/868



## ANVENDELSE AF DCAT 

### Hvordan anvender man DCAT til beskrivelse af forskningsdata?
Læs mere her: https://ec.europa.eu/jrc/en/publication/using-dcat-ap-research-data; https://ec-jrc.github.io/dcat-ap-jrc/; https://www.go-fair.org/fair-principles/

### Hvis der andre generelle specifikationer til beskrivelse af datasæt?
Ja, udover W3Cs DCAT specificerer Schema.org også [datasæt](https://schema.org/Dataset)

Schema.org er et samarbejde imellem de største søgemaskiner i et forsøg på at levere rigere og bedre søgeresultater på nettet. Opmærker man derfor med Schema.org vil datasættet derfor typisk opnås en bedre formidling og placering søgemaskinernes resultatliste. 
Der er et pågående arbejde i regi af W3C vedrørende mapping mellem DCAT-AP og Schema.org.

Læs mere her: https://schema.org/Dataset; https://schema.org/docs/data-and-datasets.html; https://ec-jrc.github.io/dcat-ap-to-schema-org/

### Kan jeg opmærke min eksisterende html-side med DCAT?
Ja, DCAT-metadata kan indlejres i eksisterende opmærkning vha. JSON-LD eller RFDa.
RDFa er en W3C-anbefaling der tilføjer et sæt attributniveauudvidelser til HTML, XHTML og forskellige XML-baserede dokumenttyper til indlejring af metadata i webdokumenter, https://en.wikipedia.org/wiki/RDFa

Se fx vejledninger her: 
- https://theodi.org/article/marking-up-your-dataset-with-dcat/
- https://developers.google.com/search/docs/data-types/dataset

### Hvilke applikationer understøtter DCAT?

