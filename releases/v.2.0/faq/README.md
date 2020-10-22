
# FAQ om beskrivelse af datasæt og datakataloger med DCAT 

I denne FAQ (som udvikles løbende) finder du svar på spørgsmål vedrørende beskrivelse af datasæt og datakataloger i henhold til DCAT-vokabularet og den europæiske og danske anvendelsesprofil. I første omgang guider svarene primært videre til uddybende indhold om disse modeller og relaterede eksterne dokumenter, men denne faq kan udbygges efter behov.

<!-- 
## Hvordan finder nye anvendere frem til et udgivet datasæt
Anvendelse af DCAT og bagvedliggende metamodel -->

## TITEL, BESKRIVELSE og IDENTIFIKATION

### Hvordan giver man datasæt gode titler og beskrivelser?
- https://diggsweden.github.io/DCAT-AP-SE/docs/recommendations.html#1-bra-namn-ska-vara-korta-och-beskrivande
- https://diggsweden.github.io/DCAT-AP-SE/docs/recommendations.html#2-%C3%B6vers%C3%A4tt-fritextf%C3%A4lt-till-andra-spr%C3%A5k

### Hvorfor skal man oprette en identifikator og hvordan oprettes de?
Læs mere her: 
- https://arkitektur.digst.dk/rammearkitektur/datastandarder/retningslinjer-stabile-http-urier ; 
- https://joinup.ec.europa.eu/collection/semantic-interoperability-community-semic/document/10-rules-persistent-uris
- https://joinup.ec.europa.eu/release/dcat-ap-how-use-identifiers-datasets-and-distributions
- https://www.go-fair.org/fair-principles/f1-meta-data-assigned-globally-unique-persistent-identifiers/


## KRAV OM OVERHOLDELSE

### Hvilke egenskaber er obligatoriske til beskrivelse af datasæt? 
Alle egenskaber er i specifikationen opmærket med deres kravniveau (obligatorisk, anbefalet eller valgfri), 

Følgende egenskaber er obligatoriske: 

- titel (title), 
- beskrivelse (description) -
- udgiver (publisher) ELLER datasætansvarlig organisation DK

Se også denne oversigt:
https://github.com/digst/DCAT-AP-DK/tree/master/releases/v.2.0/views/mandatory
og https://digst.github.io/DCAT-AP-DK/releases/v.2.0/docs/#forskellige-visninger-af-dcat-ap-dk

### Hvilke egenskaber anbefales til beskrivelse af datasæt?
Alle egenskaber er opmærket med deres kravniveau (obligatorisk, anbefalet eller valgfri).

Følgende egenskaber anbefales: 

- identifikator (identifier), 
- titel (title), 
- beskrivelse (description), 
- udgiver (publisher),
- datasætansvarlig organisation DK (dataset responsible organisation), 
- skaber (creator), 
- kontaktpunkt (contact point), 
- har distribution (dataset distribution), 
- destinationsside (landing page), 
- overholder (conforms to), 
- dokumentation (documentation), 
- emne (theme/ category), 
- sprog (language),
- dækningsperiode (temporal coverage), 
- opdateringsfrekvens (frequency), 
- udgivelsesdato (release date), 
- seneste ændringsdato (update/ modification date)

Se også denne oversigt: https://github.com/digst/DCAT-AP-DK/tree/master/releases/v.2.0/views/mandatory%2Brecommended
og https://digst.github.io/DCAT-AP-DK/releases/v.2.0/docs/#forskellige-visninger-af-dcat-ap-dk

## ADGANG TIL DATA

### Hvordan angiver man hvordan brugeren får adgang til datasættet?
- Destinationsside (på dcat:Resource): Se https://www.w3.org/TR/vocab-dcat-2/#Property:resource_landing_page 
En destinationsside er en webside som der kan navigeres til i en webbrowser for at få adgang til kataloget, et datasæt, dets distributioner og/eller yderligere information.

- Adgangs-URL (på dcat:Distribution): Se https://www.w3.org/TR/vocab-dcat-2/#Property:distribution_access_url
En adgangs-URL er en URL for en ressource som giver adgang til en distribution af datasættet. Fx, destinationsside, feed, SPARQL-endpoint. Anvendes i alle sammenhænge undtagen til angivelse af et simpelt download link hvor anvendelse af egenskaben download-URL foretrækkes.

- Dataadgangstjeneste (på dcat:Distribution): se https://www.w3.org/TR/vocab-dcat-2/#Property:distribution_access_service
Et websted eller endpoint der giver adgang til distributionen af datasættet. dcat:accessService BØR anvendes til at angive et link til en beskrivelse af en dcat:DataService som kan give adgang til distributionen.

- Download-Url (på dcat:Distribution): se https://www.w3.org/TR/vocab-dcat-2/#Property:distribution_download_url
Download-Url er en URL til fil der kan downloades i et bestemt format. Fx en CSV-fil eller en RDF-fil. Formatet for distributionen angives ved hjælp af egenskaberne dct:format og/eller dcat:mediaType. dcat:download-URL BØR anvendes til angivelse af den adresse hvor distributionen er tilgængelig direkte, typisk gennem et HTTP Get request

![DCAT-Datasæt-distribution](https://www.w3.org/2011/gld/wiki/images/2/26/Dcat-distribution-proposal.png "DCAT-AP 2.0.1 UML Diagram")

OBS: Hvis en eller flere distributioner kun er tilgængelige via en destinationsside (dvs. en URL til direkte download er ikke kendt), så bør destinationssidelinket gentages som adgangsadresse for en distribution 

Se eksempler her: https://www.w3.org/TR/vocab-dcat-2/#example-landing-page

## RETTIGHEDER OG LICENSER

### Hvordan udtrykkes licenser og rettighedsudsagn?

På kataloget (dcat:Catalog) anvendes følgende:
- dct:license - https://digst.github.io/DCAT-AP-DK/releases/v.2.0/docs/#egenskab-licens-license
- dcc:rights -  https://digst.github.io/DCAT-AP-DK/releases/v.2.0/docs/#egenskab-rettigheder-rights

På datasættet (dcat:Dataset)  anvendes følgende:
- dct:accessRights -  https://digst.github.io/DCAT-AP-DK/releases/v.2.0/docs/#egenskab-adgangsrettigheder-access-rights

På distributionen (dcat:Distributionen) anvendes følgende:
- dct:rights -  https://digst.github.io/DCAT-AP-DK/releases/v.2.0/docs/#egenskab-rettigheder-rights%E2%91%A0
- dct:license - https://digst.github.io/DCAT-AP-DK/releases/v.2.0/docs/#egenskab-licens-license%E2%91%A0
- odrl:hasPolicy - https://digst.github.io/DCAT-AP-DK/releases/v.2.0/docs/#egenskab-har-politik-has-policy

Rettighedsudsagnet beskrives med klassen dct:RightsStatement: https://digst.github.io/DCAT-AP-DK/releases/v.2.0/docs/#klasse-rettighedsudsagn-rights-statement
 
Ift. adgangsrettigheder kan klassifikationen Adgangsrettigheder anvendes: https://digst.github.io/DCAT-AP-DK/releases/v.2.0/docs/#adgangsrettigheder

Læs mere om anvendelse af ovenstående egenskaber i DCAT-AP-DK og her: https://www.w3.org/TR/vocab-dcat-2/#license-rights 

## DATAKVALITET

### Hvordan sikrer man god datakvalitet i de udgivne datasæt
Til at beskrive kvalitetsrelaterede informationer af DCAT-datasæt og -distributioner anvendes [Data on the Web Best Practices: Data Quality Vocabulary](https://www.w3.org/TR/vocab-dqv/). [Fælles sprog for datakvalitet](https://arkitektur.digst.dk/metoder/faelles-sprog-datakvalitet) (Vejledning til deklaration af datasæt med kernedimensioner vers. 1.0.0) anvender også DQV.

Læs mere her: https://www.w3.org/TR/vocab-dcat-2/#quality-information; https://www.w3.org/TR/vocab-dqv/; https://arkitektur.digst.dk/metoder/faelles-sprog-datakvalitet;  https://github.com/w3c/dxwg/wiki/Quality-documentation

### Hvordan kan man understøtte god datakvalitet i DCAT-metadatabeskrivelser?
Ved hjælp af SHACL-implementeringen af den danske anvendelsesprofil er det muligt at validere indholdet af en given DCAT-metadatabeskrivelse iht. DCAT-AP-DK og adressere flere kernekvalitetsdimensioner. Hvis den obligatoriske information mangler eller hvis obligatoriske, anbefalede eller valgfrie elementer er ikke er angivet korrekt, kan en validator baseret på SHACL-indholdet give relevante valideringsresultater og beskeder.   

Læs mere her: https://github.com/digst/DCAT-AP-DK/tree/master/releases/v.2.0/validation

## BESKRIVELSE AF PERIODER

### Hvad er forskellen mellem 'startdato og 'har begyndelse', samt 'slutdato' og 'har slutning' ift. en periode?
Klassen Periode har følgende fire egenskaber: Se også: https://digst.github.io/DCAT-AP-DK/releases/v.2.0/docs/#klasse-periode-periodoftime
- Egenskab: startdato (start date)
- Egenskab: slutdato (end date)
- Egenskab: har begyndelse (beginning)
- Egenskab: har slutning (end)

DCAT angiver to måder hvorpå man kan angive henholdsvis start og af-slutning af en periode. Det ene sæt benytter to egenskaber fra Time Ontology – en specifikation udformet i et samarbejde mellem OGC og W3C. Det andet sæt benytter to egenskaber der er defineret af DCAT-arbejdsgruppen. DCATs to egenskaber kan benytte følgende typer af tidsenheder til angivelse af helholdsvis startdato og slutdato: xsd:date, xsd:dateTime. xsd:gYear og xsd:gYearMonth. Time Ontologys to egenskaber for henholdsvis begyndelse og slutning har følgende: xsd:date, xsd:dateTimeStamp. xsd:gYear og xsd:gYearMonth. Noter at Time Ontology benytter xsd.dateTimeStamp i stedet for xsd:dateTime. Desuden kan Time Ontology benytte tidsenheder der ikke er relateret til den gregorianske kalender. 

I den danske profilering af DCAT er det valgt i videst muligt omfang at videreføre EU's DCAT-AP der tillader brug af begge egenskabssæt. Derfor er det også valgt at præsentere begge de to mulige sæt af start/slut-angivelse. DCATs egenskaber anbefales da de er de mest enkle at benytte, mens Time Ontology-egenskaberne er valgfri.


## TIDSSERIER og VERSIONER

### Hvordan beskriver man tidsserier?
Læs mere her: https://joinup.ec.europa.eu/release/dcat-ap-how-model-dataset-series og
https://github.com/w3c/dxwg/issues/868

### Hvordan skal versioner beskrives?
Læs mere her: https://github.com/w3c/dxwg/wiki/Dataset-(and-other-DCAT)-versioning


## ANVENDELSE AF DCAT 

### Hvordan anvender man DCAT til beskrivelse af forskningsdata?
Læs mere her: https://ec.europa.eu/jrc/en/publication/using-dcat-ap-research-data; https://ec-jrc.github.io/dcat-ap-jrc/; https://www.go-fair.org/fair-principles/

### Hvor finder jeg eksempler på anvendelse af DCAT, DCAT-AP og DCAT-AP-dk?
Se https://github.com/digst/DCAT-AP-DK/tree/master/releases/v.2.0/examples

### Findes der andre generelle specifikationer til beskrivelse af datasæt?
Ja, se fx.

[Schema.org](https://schema.org/Dataset).
Schema.org er et samarbejde imellem de største søgemaskiner i et forsøg på at levere rigere og bedre søgeresultater på nettet. Opmærker man derfor med Schema.org vil datasættet derfor typisk opnås en bedre formidling og placering søgemaskinernes resultatliste. Der er et pågående arbejde i regi af W3C vedrørende mapping mellem DCAT-AP og Schema.org.
Læs mere her: https://schema.org/Dataset; https://schema.org/docs/data-and-datasets.html; https://ec-jrc.github.io/dcat-ap-to-schema-org/

[ISO/IEC 11179-7:2019(en)](https://webshop.ds.dk/da-dk/standarder/standard/sprog-og-operativsystemer/iso-iec-11179-72019)
Med del 7 - ISO/IEC 11179-7:2019(en) Information technology — Metadata registries (MDR) — Part 7: Metamodel for data set registration), udvides ISO 11179 Metadata Registry (MDR) til datasætbeskrivelse, og det står anført at standarden "was prepared taking into account concepts described in the following documents: — Data Catalog Vocabulary (DCAT)[1] (published by the World Wide Web Consortium (W3C)) (..);"

### Hvilke mapninger mellem DCAT-AP og øvrige specifikationer findes der?
- [GeoDCAT-AP](https://joinup.ec.europa.eu/solution/geodcat-application-profile-data-portals-europe) (EU ISA Programme) - Defines mappings from INSPIRE/ISO 19115 metadata to DCAT-AP
  - [Alignment of INSPIRE metadata with DCAT-AP](https://ies-svn.jrc.ec.europa.eu/projects/metadata/wiki/Alignment_of_INSPIRE_metadata_with_DCAT-AP)
  - [Mappings defined in GeoDCAT-AP](https://github.com/GeoCat/iso-19139-to-dcat-ap/blob/master/documentation/Mappings.md)
- [ISO 19115 - DCAT - Schema.org mapping](https://www.w3.org/2015/spatial/wiki/ISO_19115_-_DCAT_-_Schema.org_mapping) (W3C SDW WG)
- [StatDCAT-AP](https://joinup.ec.europa.eu/solution/statdcat-application-profile-data-portals-europe) (EU ISA Programme) - Defines mappings from SDMX metadata to DCAT-AP
- [DDI v2 to Dublin Core](http://www.ddialliance.org/resources/ddi-profiles/dc) (DDI Alliance)
- [DCAT to Schema.org mapping](https://project-open-data.cio.gov/metadata-resources/) (Project Open Data)
- [DCAT-AP to Schema.org mapping](https://ec-jrc.github.io/dcat-ap-to-schema-org/) (JRC)
- [DataCite to DCAT-AP mapping](https://ec-jrc.github.io/datacite-to-dcat-ap/) (JRC)

Ref: https://www.w3.org/2017/dxwg/wiki/Main_Page#Mappings_to.2Ffrom_DCAT_.28and_DCAT_application_profiles.29

### Kan jeg opmærke min eksisterende html-side med DCAT?
Ja, DCAT-metadata kan indlejres i eksisterende opmærkning vha. JSON-LD eller RFDa.
RDFa er en W3C-anbefaling der tilføjer et sæt attributniveauudvidelser til HTML, XHTML og forskellige XML-baserede dokumenttyper til indlejring af metadata i webdokumenter, https://en.wikipedia.org/wiki/RDFa

Se fx vejledninger og eksempler her: 
- https://theodi.org/article/marking-up-your-dataset-with-dcat/
- https://developers.google.com/search/docs/data-types/dataset
- https://github.com/digst/DCAT-AP-DK/tree/master/releases/v.2.0/examples/RDFa

### Hvilke applikationer understøtter DCAT?

