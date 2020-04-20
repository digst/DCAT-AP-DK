
# FAQ om beskrivelse af datasæt og datakataloger med DCAT (under udvikling)

I FAQ'en finder du svar på spørgsmål vedrørende beskrivelse af datasæt og datakataloger i henhold til DCAT-vokabularet og den europæiske og danske anvendelsesprofil. I første omgang guider svarene primært videre til uddybende indhold om disse modeller og relaterede eksterne dokumenter, men denne faq kan udbygges efter behov.


## Hvordan finder nye anvendere frem til et udgivet datasæt
Anvendelse af DCAT og bagvedliggende metamodel 

## Hvordan giver man datasæt gode titler?
https://diggsweden.github.io/DCAT-AP-SE/docs/recommendations.html#1-bra-namn-ska-vara-korta-och-beskrivande

## Hvordan skriver man en god tekstbaseret beskrivelse af et datasæt?

## Hvornår skelner man mellem mulighederne for angivelse af hvordan man får adgang til datasættet?
Destinationsside, adgangs-URL, download-URL etc.

## Hvordan skelner man mellem de forskellige aktørroller?
Dataansvarlig organisation, udgiver, skaber, bidragsyder, vedligeholder

## Hvordan skal versioner beskrives?
Læs mere her: https://github.com/w3c/dxwg/wiki/Dataset-(and-other-DCAT)-versioning
Note: info om arkiverede data.

## Hvordan beskriver man tidsserier?
Læs mere her: https://joinup.ec.europa.eu/release/dcat-ap-how-model-dataset-series

## Hvorfor skal man operette en identifikator og hvordan man det?
Læs mere her: https://arkitektur.digst.dk/rammearkitektur/datastandarder/retningslinjer-stabile-http-urier (Revsion på vej)

## Hvordan angiver sikrer man god datakvalitet i de udgivne datasæt
Til at beskrive kvalitetsrelaterede informationer af DCAT-datasæt og -distributioner anvendes [Data on the Web Best Practices: Data Quality Vocabulary](https://www.w3.org/TR/vocab-dqv/). [Fælles sprog for datakvalitet](https://arkitektur.digst.dk/metoder/faelles-sprog-datakvalitet) (Vejledning til deklaration af datasæt med kernedimensioner vers. 1.0.0) anvender også DQV.

Læs mere her: https://www.w3.org/TR/vocab-dcat-2/#quality-information; https://www.w3.org/TR/vocab-dqv/; https://arkitektur.digst.dk/metoder/faelles-sprog-datakvalitet;  https://github.com/w3c/dxwg/wiki/Quality-documentation

## Hvordan kan man understøtte god datakvalitet i DCAT-metadatabeskrivelser?
Ved hjælp af SHACL-implementeringen af den danske anvendelsesprofil er det muligt at validere indholdet af en given DCAT-metadatabeskrivelse iht. DCAT-AP-DK og adressere flere kernekvalitetsdimensioner. Hvis den obligatoriske information mangler eller hvis obligatoriske, anbefalede eller valgfrie elementer er ikke er angivet korrekt, kan en validator baseret på SHACL-indholdet give relevante valideringsresultater og beskeder.   

Læs mere her: https://github.com/digst/DCAT-AP-DK/tree/master/releases/v.2.0/validation

## Hvordan anvender man DCAT til beskrivelse af forskningsdata?
Læs mere her: https://ec.europa.eu/jrc/en/publication/using-dcat-ap-research-data; https://ec-jrc.github.io/dcat-ap-jrc/; https://www.go-fair.org/fair-principles/

## Hvis der andre generelle specfifikationer til beskrivelse af datasæt?
Ja, udover W3Cs DCAT specificerer Schema.org også [datasæt](https://schema.org/Dataset)

Schema.org er et samarbejde imellem de største søgemaskiner i et forsøg på at levere rigere og bedre søgeresultater på nettet. Opmærker man derfor med Schema.org vil datasættet derfor typisk opnås en bedre formidling og placering søgemaskinernes resultatliste. 
Der er et pågående arbejde i regi af W3C vedrørende mapping mellem DCAT-AP og Schema.org.

Læs mere her: https://schema.org/Dataset; https://schema.org/docs/data-and-datasets.html; https://ec-jrc.github.io/dcat-ap-to-schema-org/



