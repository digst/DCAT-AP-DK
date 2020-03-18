<style>
@media print {
  html { margin: 0cm 2cm 2cm 0cm; font-size: 80%; }
  /* DIGST fonts */
  body { font-family: "Helvetica Neue", Helvetica, Arial, sans-serif;}
  h2,h3,h4, h4 dfn { font-family: "Garamond", serif; color: black; margin-bottom: 0; font-style: normal; font-weight: normal;}
  h2:not(#subtitle) { page-break-before: always; font-size: 250%; border-bottom: solid 0.5px black; padding-top: 20px; margin-bottom: 6px;}
  h3 { font-size: 145%;}
  h4 { font-size: 125%;}
  #toc {page-break-before: always;}
  /* DIGST-like frontpage */
  .head { width: 50%; margin-left: 24px; padding: 0px; background-color: #031D5C;}
  .head div { background-color: white; padding: 24px; }
  .head hr { display: none;}
  .head h1 { background-color: #031D5C; color: white; margin: 0px; padding: 50px 0px 50px 24px; font-weight: normal; }
  #subtitle { padding-left: 24px; background-color: #031D5C; color: #031D5C; }
  .head time { display: block; font-family: "Helvetica Neue", Helvetica, Arial; margin: 0px; background-color: #031D5C; font-size: 80%; color: white;}
  .toc li { line-height: 70%; font-family: "Helvetica Neue", Helvetica, Arial;
    font-weight: 600; font-size: 90%; }
  h2.heading.settled > a.self-link, h3.heading.settled > a.self-link, h4.heading.settled > a.self-link, h4.heading.settled > a.self-link, h5.heading.settled > a.self-link, h6.heading.settled > a.self-link { display: none; }
  blockquote { font-size: 80%; font-style: italic; margin-left: 5%; width: 70%; border-left-width: 2px;}
	h2#abstract {display: none;}
	.p-summary {width: 50%; margin-left: 24px; padding: 0px;}
}
.new {
    border: solid 3px green;
    padding: 6px;
    margin: 18px 0px 18px 0px;
}

h2.heading.settled > a.self-link, h3.heading.settled > a.self-link, h4.heading.settled > a.self-link, h4.heading.settled > a.self-link, h5.heading.settled > a.self-link, h6.heading.settled > a.self-link { display: none; }

.term-table{
  font-size: 80%;
}

.term-table tr td:nth-of-type(3), .term-table tr td:nth-of-type(4), .term-table tr td:nth-of-type(5){
  word-wrap: anywhere;
  overflow-wrap: anywhere;
  hyphens: auto;
  word-break: break-all;
}

.term-table td{
  border-bottom: 1px solid #ccc;
  padding: 12px 8px;
}

.term-table tr td:first-child{
  font-weight: 600;
  word-wrap: break-word;
}

.term-table tr th:first-child{
  width: 20%;
}

.term-table tr th:nth-of-type(2){
  width: 22%;
}

.term-table tr th:nth-of-type(3){
  width: 15%;
}

.term-table tr th:nth-of-type(4){
  width: 15%;
}

.term-table tr th:nth-of-type(5){
  width: 15%;
}

.term-table tr th:nth-of-type(6){
  width: 13%;
}

.term-table tr td:nth-of-type(2){
  font-style: italic;
}

.term-table th{
  color: #fff;
  border: none;
  background-color: #940027;
  text-transform: capitalize;
  font-weight: 600;
  padding: 6px 8px;
}

.body{
  max-width: 100% !important;
}

.body.h-entry{
  max-width: 100%;
}

	@media screen and (min-width: 78em) {

		body.h-entry:not(.toc-inline) {
			padding-left: 25em;
		}
}
	
	
/* style til egne og andres definitioner rød/blå*/
</style>

<pre class="metadata">
Title: UDKAST: Standard for beskrivelse af datasæt (DCAT-AP-DK)
Status: LD
URL: https://github.com/digst/DCAT-AP-DK/releases/v.2.0/
Editor Term: Bidragsyder, Bidragsydere 
Editor: Digitaliseringsstyrelsen,, arkitektur@digst.dk
Editor: [Styrelsen for data og effektivisering]
Editor: [Styrelsen for arbejdsmarked og rekruttering]
Editor: [Geodatastyrelsen]
Editor: [Erhvervstyrelsen]
Editor: [Danmarks Miljøportal]
Editor: [Danmarks Statistik]
Editor: [Kommunernes Landsforening]
Editor: [KOMBIT]
Group: Udvalget for Arkitektur og Standarder (UAS) 


Abstract: Dette dokument 'Standard for beskrivelse af datasæt (DCAT-AP-DK)' udgør en fællesoffentlig standard for beskrivelse af offentlige myndigheders datasæt.
Boilerplate: copyright no, conformance no, abstract no
Shortname: DCAT-AP-DK
Revision: 2.0.0
Date: 2019-03-11
Max ToC Depth: 3
Markup Shorthands: markdown yes
Repository: digst/DCAT-AP-DK/DCAT-AP-DK/releases/v.2.0
Inline Github Issues: full
Logo: digst...
</pre>


<h1>UDKAST: Standard for beskrivelse af datasæt (DCAT-AP-DK 2.0)</h1>

UDKAST til DCAT-AP-DK 2.0
Marts 2020
   



# Introduktion

DCAT-AP-DK 2.0 er en specifikation til beskrivelse af datasæt til anvendelse i dansk fællesoffentlig regi. Standarden omfatter basisoplysninger om datasæt, som fx titel, beskrivelse, udgiver, udgivelsesdato mv., samt en ensartet struktur for disse oplysninger i et fælles udvekslingsformat, som gør det muligt at dele oplysninger om datasæt på en effektiv måde. Specifikationen resulterer i en såkaldt anvendelsesprofil baseret på internationale og nationale specifikationer.

## Formål
Specifikationen skal være med til sørge for at begreber til beskrivelse af datasæt anvendes mere ens, og dermed skal den understøtte højere grad af interoperablitet og kvalitet i oplysningerne. 


## Baggrund

De grundlæggende strukturer og elementer hentes fra EU-Kommissionens specifikation DCAT-AP 2.0 der har til formål at standardisere og etablere sammen-hæng mellem dataportaler i medlemslandene. EU-Kommissionens specifikation tager ligeledes afsæt i W3C specifikationen DCAT (Data Catalog Vocabulary). EU-Kommissionens specifikation angiver ikke blot hvilke felter der er *obligatoriske*, men angiver også *anbefalede* og *valgfrie* egenskaber og giver mulighed for en meget omfangsrig metadatabeskrivelse. DCAT-AP-DK 2.0 vil anvende elementer fra og vil være i overensstemmelse med DCAT-AP 2.0, men vil også tilføje enkelte nye elementer for at opfylde behov i en dansk administrativ og fællesoffentlig kontekst.

Standarden er udarbejdet med feedback fra og sparring med en følgegruppe med medlemmer som repræsenterer både kommuner, regioner og statslige myndigheder.

For at sikre at behov imødekommes vil den danske specifikation således tage udgangspunkt i følgegruppens vurdering af obligatoriske, anbefalede og valgfrie egenskaber i DCAT-AP 2.0. 



## Metode

Denne standard udgøres af en dansk basisprofil for datsæt (DCAT-AP-DK), som indeholder de basisoplysninger om datsæt, der indgår i typiske datasætoverblik.  Basisoplysningerne udgør en fælles kerne, der kan udvides med yderligere kontekstafhængige oplysninger, i nye og mere specifikke anvendelsesprofiler. Informationer dannet på baggrund af to eller flere specifikke anvendelsesprofiler kan potentielt bringes til at hænge sammen via denne fælles kerne.

Selve udviklingsarbejdet er foretaget i henhold de [Fællesoffentlige regler for begrebs- og datamodellering](https://arkitektur.digst.dk/metoder/regler-begrebs-og-datamodellering), og standarden udgøres af en basisprofil, der sammensætter flere eksisterende nationale og internationale modeller.



## Standardens anvendelse og afgrænsning



## Konformans og afvigelser fra DCAT-AP

### Tilføjelser

### Udeladelser

### Ændringer af kravniveau



# Oversigt over anvendelsesprofilen

## Diagram



## Namespaces

* adms: http://www.w3.org/ns/adms#
* dcat: http://www.w3.org/ns/dcat#
* dcatap: http://data.europa.eu/r5r/
* dct: http://purl.org/dc/terms/
* foaf: http://xmlns.com/foaf/0.1/
* locn: http://www.w3.org/ns/locn#
* owl: http://www.w3.org/2002/07/owl#
* odrl: http://www.w3.org/ns/odrl/2/
* rdfs: http://www.w3.org/2000/01/rdf-schema#
* schema: http://schema.org/
* skos: http://www.w3.org/2004/02/skos/core#
* spdx: http://spdx.org/rdf/terms#
* xsd: http://www.w3.org/2001/XMLSchema#
* vann: http://purl.org/vocab/vann/
* voaf: http://purl.org/vocommons/voaf#
* vcard: http://www.w3.org/2006/vcard/ns#
* dcat-ap-dk: https://data.gov.dk/model/profile/dcat-ap-dk/


# Modellens grundlæggende struktur
DCAT beskriver en ramme metadata om datasæt i tre forskellige lag, et kataloglag, på datasætlag og på repræsentationslag. Hvert element i et givet lag kan beskrives med metadata, såsom titel, beskrivelse osv. 

## Kataloglaget
Kataloglaget er det øverste lag i DCAT-standarden. Det indeholder metadata om selve kataloget samt reference til de datasæt som indgår i det pågældende datakatalog. 

## Datasætlaget
Dette lag udgøres af de individuelle datassæt. Et datasæt er et logisk element der repræsenterer den udgivne information. Det kan referere til mange forskellige repræsentatationer at netop dette datasæt. 

## Repræsentationslaget
Repræsentationslaget er det nederste lag i DCAT-standarden. Her defineres adgangsURL, formatet, størrelse, downloadURL adgangsservice etc..


# Elementer i DCAT-AP-DK 
I det følgende præsenteres alle egenskaberne i DCAT-AP-DK per klasse.





## Klasse: Katalog (Obligatorisk)    STIL1!

Denne klasse anvendes til at beskrive et katalog hvori der indgår datasætbeskrivelser. Det er obligatorisk at anvende klassen

(dcat:Catalog)


## Klasse: Katalog (dcat:Catalog)  STIL2!
Denne klasse anvendes til at beskrive et katalog hvori der indgår datasætbeskrivelser. Det er obligatorisk at anvende klassen.


## Klasse: Katalog  STIL3!
Denne klasse anvendes til at beskrive et katalog hvori der indgår datasætbeskrivelser.
<dl class="def"> 
<dt>RDF-egenskab</dt><dd></dd>dcat:Catalog<dt>
<dt>Definition</dt><dd></dd>En organiseret samling af metadata om ressourcer (fx. datasæt og dataservices i kontekst af et datakatalog)<dt>
<dt>Anvendelsesnote</dt><dd></dd>En organiseret samling af metadata om ressourcer (fx. datasæt og dataservices i kontekst af et datakatalog)<dt>
<dt>Kravniveau</dt><dd></dd>Obligatorisk<dt>
</dl>




### Egenskab: beskrivelse (Obligatorisk)   STIL1!
Denne egenskab giver en tekstbaseret beskrivelse af kataloget.  Denne egenskab kan gentages for hver sprog. Multipliciteten skal være 1 - *.

(dct:description)

### Egenskab: beskrivelse (dct:description)    STIL2!
Denne egenskab giver en tekstbaseret beskrivelse af kataloget.  Denne egenskab kan gentages for hver sprog. Multipliciteten skal være 1 - * (Obligatorisk)

### Egenskab: beskrivelse     STIL3!
Denne egenskab giver en tekstbaseret beskrivelse af kataloget.  Denne egenskab kan gentages for hver sprog. 
<dl class="def"> 
<dt>RDF-egenskab</dt><dd></dd>dct:description<dt>
<dt>Definition</dt><dd></dd>En tekstbaseret beskrivelse af ressourcen.<dt>
<dt>Rækkevidde</dt><dd></dd>rdfs:Literal<dt>
<dt>Kravniveau</dt><dd></dd>Obligatorisk (Multiplicitet:1 - *)<dt>
</dl>



### Egenskab: titel (Obligatorisk)
Det eller de ord, der navngiver datasættet
(dct:title)


### Egenskab: udgiver (Obligatorisk)  
dct:publisher

### Egenskab: datasæt (Obligatorisk) 
dcat:dataset

### Egenskab: hjemmeside (Anbefalet) 
foaf:homepage

### Egenskab: sprog  (Anbefalet) 
dct:language

### Egenskab: licens (Anbefalet) 
dct:license

### Egenskab: udgivelsesdato  (Anbefalet) 
dct:issued

### Egenskab: seneste opdateringsdato  (Anbefalet)  
dct:modified

### Egenskab: geografisk afgrænsning  (Anbefalet)   
dct:spatial

### Egenskab: anvendt klassifikation (Anbefalet)  
dcat:themeTaxonomy

### Egenskab: har del (Valgfri)
dct:hasPart

### Egenskab: er del af (Valgfri)
dct:isPartOf

### Egenskab: optegnelse (Valgfri)
dcat:record

### Egenskab: adgangsrettigheder (Valgfri)
dct:rights

### Egenskab: service (Valgfri)
dcat:service

### Egenskab: katalog (Valgfri)
dcat:catalog

### Egenskab: skaber (Valgfri)
dct:creator


<p class="example">
'
ex:catalog
  a dcat:Catalog ;
  dct:publisher ex:Organization-001 ;
  dct:title "Imaginary Catalog"@en ;
  rdfs:label "Imaginary Catalog"@en ;
  dcat:dataset ex:dataset-001 ;
  dcat:dataset ex:dataset-002 ;
  dcat:dataset ex:dataset-003 ;
  foaf:homepage <http://example.org/catalog> ;
.
'
</p>


## Klassen Katalogoptegnelse
En optegnelse i et datakatalog der beskriver registreringen af et enkelt datasæt eller en dataservice

### Egenskab: optegnelsens genstand (Obligatorisk)
Den ressource (datasæt, dataservice eller katalog) optegnelsen i kataloget handler om
foaf:primaryTopic 

### Egenskab: seneste opdateringsdato (Obligatorisk)
dct:modified

### Egenskab: i overenstemmelse med (Anbefalet)
dct:conformsTo

### Egenskab: status (Anbefalet)
adms:status

### Egenskab: udgivelsesdato (Anbefalet)
dct:issued

### Egenskab: bskrivelse (Valgfri)
dct:description

### Egenskab: sprog (Valgfri)
dct:language

### Egenskab: kilde(Valgfri)
dct:source

### Egenskab: titel (Valgfri)
dct:title




## Klassen Datasæt
A conceptual entity that represents the information published.


### Egenskab: titel (Obligatorisk)
dct:title

### Egenskab: beskrivelse (Obligatorisk)
dct:description

### Egenskab: udgiver (?)
dct:publisher

### Egenskab: dataansvarlig organisation (?)
dcat-dk:dataResponsibleOrganisation

### Egenskab: Kontaktpunkt (Anbefalet)
dcat:contactPoint

### Egenskab: identifikator (Anbefalet)
dct:identifier

### Egenskab: anden identifikator (Valgfri)
adms:identifier

### Egenskab: datatema ()
EUs datatemaer
Forvaltningsopgaver (FORM/KLE) - versionsnummer
dct:theme

### Egenskab: nøgleord (Valgfri)
dcat:keyword

### Egenskab: hjemmel (Anbefalet)
cv:hasLegalResource

### Egenskab: personoplysningskategori (Anbefalet)

### Egenskab: betalingspålagt (Anbefalet)
dcat-dk: payment ImposedContents|

### Egenskab: datasærepræsentation (Anbefalet)
dcat:distribution



### Egenskab:  (Valgfri)
dct:spatial
dct:temporal
dct:accessRights
dct:creator
schema:maintainer
dct:conformsTo
foaf:page
dct:accrualPeriodicity
dct:hasVersion
dct:isReferencedBy
dct:isVersionOf
dcat:landingPage
dct:language
dqv:hasQualityMetadata 
duv:hasUsage

## Klassen Datasætrepræsentation
physical embodiment of the Dataset in a particular format


## Klassen Dataservice

A collection of operations that provides access to one or more datasets or data processing functions.


## Klassen Aktør

An entity that is associated with Catalogues and/or Datasets. 














# Emner

* Basisinformation
* Emneinddeling
* Aktører
* Dataindhold
* Afgrænsning
* Datakvalitet
* Jura og regulering
* Proveniens og historik



# Referencer

* DCAT 2.0: https://www.w3.org/TR/vocab-dcat-2/
* DCAT-AP 2.0: https://joinup.ec.europa.eu/solution/dcat-application-profile-data-portals-europe/release/200
* DCAT-AP validator: https://www.itb.ec.europa.eu/shacl/dcat-ap/upload
* DCAT-AP-OP (1.1): http://data.europa.eu/euodp/en/developerscorner
* Overblik over nationale DCAT-APer: https://datos.gob.es/sites/default/files/doc/file/report_dcat-ap_and_its_extensions.pdf
* EDP Goldbook: https://www.europeandataportal.eu/sites/default/files/european_data_portal_-_open_data_goldbook.pdf
* W3C Data Quality Vocabulary: https://www.w3.org/TR/vocab-dqv/
* Fælles sprog for datakvalitet: https://arkitektur.digst.dk/sites/default/files/faelles_sprog_for_datakvalitet_-_vejledning_til_deklaration_af_datasaet_med_kernedimensioner_vers_1.0.0.docx
* W3C Data on the Web Best practices: https://www.w3.org/TR/dwbp/


# Bilag

## UML-diagrammer

## Eksempler 

## Begrebsliste



================

arkitektur.digst.dk




# Short hands

   
# h1

## h2

### h3 

#### h4

##### h5

<p align="center"><a href="img/test.jpg"><img src="img/test.jpg" alt="test" width="800"/></a></p>

Links: [Test](https://www.example.om)


<p class="note">Note 1</p>

<p class="example">Example 2</p>

<p class="assertion">assertion 3</p>

<p class="advisement">advisement</p>

<p class="issue">Issue</p>

definition list:
<dl class="def"> 
<dt>1</dt><dd></dd>a<dt>
<dt>2</dt><dd></dd>b<dt>
</dl>
	
* bullit 1	
* bullit 2
* bullit 3

*kursiv*

**fed**


