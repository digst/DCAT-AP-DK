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
URL: https://github.com/digst/DCAT-AP-DK/tree/master/releases/v.2.0/
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
Date: 2019-03-27
Max ToC Depth: 3
Markup Shorthands: markdown yes
Repository: digst/DCAT-AP-DK/tree/master/releases/v.2.0
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

## Emner

* Basisinformation
* Emneinddeling
* Aktører
* Dataindhold
* Afgrænsning
* Datakvalitet
* Jura og regulering
* Proveniens og historik


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
DCAT bevæger sig i tre sammenhængende niveauer, et katalogniveau, på datasætniveau og på et distributionsniveau. Hvert element på et givet niveau kan beskrives med metadata, såsom titel, beskrivelse osv. 

## Katalogniveauet
Kataloglaget er det øverste niveau i DCAT-standarden. Det indeholder metadata om selve kataloget samt reference til de datasæt som indgår i det pågældende datakatalog. 

## Datasætnvieauet
Dette niveau udgøres af de individuelle datassæt. Et datasæt er et logisk element der repræsenterer den udgivne information. Det kan referere til mange forskellige repræsentatationer at netop dette datasæt. 

## Distributionsniveauet
Distributionsniveauet er det nederste lag i DCAT-standarden. Her beskrives hvordan man opnår adgang den fysiske distribution af datasættet med oplysninger såsom adgangsURL, format, størrelse, downloadURL adgangsservice etc..

<p class="issue">Hvordan fungerer denne fortælling om strukturen? </p>

# Elementer i DCAT-AP-DK 
I det følgende præsenteres alle egenskaberne i DCAT-AP-DK per klasse.

<p class="issue">Herunder er indsat elementerne fra DCAP-AP samt enkelte yderligere egenskaber. Elementbetegnelserne er oversat til dansk (forslag), men anvendelsesnoterne er endnu ikke oversat. Det er også hensigten at de oprindelige definitioner fra kernemodellerne skal hentes ind. Derudover mangler flere egenskaber angivelse af kravniveau</p>


## Katalog

<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/dcat#Catalog</dd>
<dt>Anvendelsesnote (da) </dt>
<dd>En organiseret samling af metadata om datasæt og dataservices i et katalog.</dd>
<dt>Anvendelsesnote (en)</dt>
<dd>A catalogue or repository that hosts the Datasets being described.</dd>
<dt>Definition (en)</dt>
<dd>A curated collection of metadata about resources (e.g., datasets and data services in the context of a data catalog).</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>

### titel

<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/title</dd>
<dt>Anvendelsesnote (da)</dt>
<dd>Denne egenskab giver det eller de ord der navngiver kataloget </dd>
<dt>Anvendelsesnote (en)</dt>
<dd>This property contains a name given to the Catalogue. This property can be repeated for parallel language versions of the name.</dd>
<dt>Definition (en)</dt>
<dd>A name given to the resource.</dd>
<dt>Multiplicitet</dt>
<dd>1..*</dd>
<dt>Kravniveau</dt>
<dd>Obligatorisk</dd>
</dl>

### beskrivelse

<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/description</dd>
<dt>Anvendelsesnote (da)</dt>
<dd>Denne egenskab giver en tekstbaseret beskrivelse af datakatalogets formål og indhold. Egenskaben kan gentages for hvert sprogvariant af beskrivelsen</dd>
<dt>Anvendelsesnote (en)</dt>
<dd>This property contains a free-text account of the Catalogue. This property can be repeated for parallel language versions of the description.</dd>
<dt>Definition (en)</dt>
<dd>An account of the resource.</dd>
<dt>Multiplicitet</dt>
<dd>1..*</dd>
<dt>Kravniveau</dt>
<dd>Obligatorisk</dd>
</dl>

### udgiver

<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/publisher</dd>
<dt>Anvendelsesnote (da)</dt>
<dd>Denne egenskab angiver den aktør (organisation) der er ansvarlig for at gøre kataloget tilgængligt.</dd>
<dt>Anvendelsesnote (en)</dt>
<dd>This property refers to an entity (organisation) responsible for making the Catalogue available. </dd>
<dt>Definition (en)</dt>
<dd>An entity responsible for making the resource available.</dd>
<dt>Multiplicitet</dt>
<dd>1..1</dd>
<dt>Kravniveau</dt>
<dd>Obligatorisk</dd>
</dl>

### skaber

<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/creator</dd>
<dt>Anvendelsesnote (da)</dt>
<dd>Denne egenskab angiver den aktør der primært er ansvarlig for katalogets skabelse.</dd>
<dt>Anvendelsesnote (en)</dt>
<dd>This property refers to the entity primarily responsible for producing the catalogue.</dd>
<dt>Definition (en)</dt>
<dd>An entity responsible for making the resource.</dd>
<dt>Multiplicitet</dt>
<dd>0..1</dd>
<dt>Kravniveau</dt>
<dd>Obligatorisk</dd>
</dl>

### udgivelsesdato

<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/issued</dd>
<dt>Anvendelsesnote (da)</dt>
<dd>Denne egenskab angiver den dato hvor kataloget først blev formelt udgivet</dd>
<dt>Anvendelsesnote (en)</dt>
<dd>This property contains the date of formal issuance (e.g., publication) of the Catalogue.</dd>
<dt>Definition (en)</dt>
<dd>Date of formal issuance of the resource.</dd>
<dt>Multiplicitet</dt>
<dd>0..1</dd>
<dt>Kravniveau</dt>
<dd>Obligatorisk</dd>
</dl>

### seneste opdateringsdato

<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/modified</dd>
<dt>Anvendelsesnote (da)</dt>
<dd>Denne egenskab angiver den dato hvor kataloget senest er blevet ændret.</dd>
<dt>Anvendelsesnote (en)</dt>
<dd>This property contains the most recent date on which the Catalogue was changed or modified.</dd>
<dt>Definition (en)</dt>
<dd>Date on which the resource was changed.</dd>
<dt>Multiplicitet</dt>
<dd>0..1</dd>
<dt>Kravniveau</dt>
<dd>Obligatorisk</dd>
</dl>

### geografisk område

<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/spatial</dd>
<dt>Anvendelsesnote (da)</dt>
<dd>Denne egenskab angiver et geografisk område som kataloget dækker.</dd>
<dt>Anvendelsesnote (en)</dt>
<dd>This property refers to a geographical area covered by the Catalogue. </dd>
<dt>Definition (en)</dt>
<dd>Spatial characteristics of the resource.</dd>
<dt>Multiplicitet</dt>
<dd>0..*</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>

### sprog

<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/language</dd>
<dt>Anvendelsesnote (da)</dt>
<dd>Denne egenskab angiver et sprog som er anvendt til tekstbaserede metadata om dataset og dataservices i kataloget. Egenskaben kan gentages for hver sprogvariant metadata forefindes på. </dd>
<dt>Anvendelsesnote (en)</dt>
<dd>This property refers to a language used in the textual metadata describing titles, descriptions, etc. of the Datasets in the Catalogue. This property can be repeated if the metadata is provided in multiple languages.</dd>
<dt>Definition (en)</dt>
<dd>A language of the resource.</dd>
<dt>Multiplicitet</dt>
<dd>0..*</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>

### licens

<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/license</dd>
<dt>Anvendelsesnote (da)</dt>
<dd>Denne egenskab angiver den licens under hvilken kataloget kan anvendes eller genbruges</dd>
<dt>Anvendelsesnote (en)</dt>
<dd>This property refers to the licence under which the Catalogue can be used or reused.</dd>
<dt>Definition (en)</dt>
<dd>A legal document giving official permission to do something with a resource.</dd>
<dt>Multiplicitet</dt>
<dd>0..1</dd>
<dt>Kravniveau</dt>
<dd>Obligatorisk</dd>
</dl>

### adgangsrettigheder

<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/rights</dd>
<dt>Anvendelsesnote (da)</dt>
<dd>Denne egenskab angiver det dokument der beskriver adgangsrettighederne for kataloget</dd>
<dt>Anvendelsesnote (en)</dt>
<dd>This property refers to a statement that specifies rights associated with the Catalogue.</dd>
<dt>Definition (en)</dt>
<dd>Information about rights held in and over the resource.</dd>
<dt>Multiplicitet</dt>
<dd>0..1</dd>
<dt>Kravniveau</dt>
<dd>Obligatorisk</dd>
</dl>

### katalogpost

<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/dcat#record</dd>
<dt>Anvendelsesnote (da)</dt>
<dd>Denne egenskab angiver en registrering af et enkelt datasæt eller en enkelt dataservice som er en del af kataloget</dd>
<dt>Anvendelsesnote (en)</dt>
<dd>This property refers to a Catalogue Record that is part of the Catalogue</dd>
<dt>Definition (en)</dt>
<dd>A record describing the registration of a single dataset or data service that is part of the catalog.</dd>
<dt>Multiplicitet</dt>
<dd>0..*</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>

### emneklassifikation

<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/dcat#themeTaxonomy</dd>
<dt>Anvendelsesnote (da)</dt>
<dd>Denne egenskab angiver en emneklassifikation der anvendes til kategorisering af datasæt og dataservices i kataloget</dd>
<dt>Anvendelsesnote (en)</dt>
<dd>This property refers to a knowledge organization system used to classify the Catalogue's Datasets.</dd>
<dt>Definition (en)</dt>
<dd>A knowledge organization system (KOS) used to classify catalog's datasets and services.</dd>
<dt>Multiplicitet</dt>
<dd>0..*</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>

### dataservice

<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/dcat#service</dd>
<dt>Anvendelsesnote (da)</dt>
<dd>Denne egenskab angiver et websted eller endpoint som er opført i kataloget.</dd>
<dt>Anvendelsesnote (en)</dt>
<dd>This property refers to a site or end-point that is listed in the catalog.</dd>
<dt>Definition (en)</dt>
<dd>A site or endpoint that is listed in the catalog.</dd>
<dt>Multiplicitet</dt>
<dd>0..*</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>

### katalog

<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/dcat#catalog</dd>
<dt>Anvendelsesnote (da)</dt>
<dd>Denne egenskab angiver et katalog hvis indhold er relevant i forhold til det aktuelle katalog.</dd>
<dt>Anvendelsesnote (en)</dt>
<dd>This property refers to a catalog whose contents are of interest in the context of this catalog.</dd>
<dt>Definition (en)</dt>
<dd>A catalog whose contents are of interest in the context of this catalog.</dd>
<dt>Multiplicitet</dt>
<dd>0..*</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>

### datasæt

<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/dcat#dataset</dd>
<dt>Anvendelsesnote (da)</dt>
<dd>Denne egenskab angiver et datasæt som er opført i kataloget</dd>
<dt>Anvendelsesnote (en)</dt>
<dd>This property links the Catalogue with a Dataset that is part of the Catalogue.</dd>
<dt>Definition (en)</dt>
<dd>A collection of data that is listed in the catalog.</dd>
<dt>Multiplicitet</dt>
<dd>1..*</dd>
<dt>Kravniveau</dt>
<dd>Obligatorisk</dd>
</dl>

### websted

<dl class="def">
<dt>URI</dt>
<dd>http://xmlns.com/foaf/0.1/homepage</dd>
<dt>Anvendelsesnote (da)</dt>
<dd>Denne egenskab angiver en webside som fungerer som katalogets hjemmeside.</dd>
<dt>Anvendelsesnote (en)</dt>
<dd>This property refers to a web page that acts as the main page for the Catalogue.</dd>
<dt>Definition (en)</dt>
<dd>A homepage for some thing.</dd>
<dt>Multiplicitet</dt>
<dd>0..1</dd>
<dt>Kravniveau</dt>
<dd>Obligatorisk</dd>
</dl>

### delkatalog

<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/hasPart</dd>
<dt>Anvendelsesnote (da)</dt>
<dd>Denne egenskab angiver et relateret katalog som er en del af det aktuelle katalog.</dd>
<dt>Anvendelsesnote (en)</dt>
<dd>This property refers to a related Catalogue that is part of the described Catalogue.</dd>
<dt>Definition (en)</dt>
<dd>A related resource that is included either physically or logically in the described resource.</dd>
<dt>Multiplicitet</dt>
<dd>0..*</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>

### del af katalog

<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/isPartOf</dd>
<dt>Anvendelsesnote (da)</dt>
<dd>Denne egenskab angiver et relateret katalog som det aktuelle katalog fysisk eller logisk er en del af.</dd>
<dt>Anvendelsesnote (en)</dt>
<dd>This property refers to a related Catalogue in which the described Catalogue is physically or logically included.</dd>
<dt>Definition (en)</dt>
<dd>A related resource in which the described resource is physically or logically included.</dd>
<dt>Multiplicitet</dt>
<dd>0..1</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>

## Katalogpost

<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/dcat#CatalogRecord</dd>
<dt>Anvendelsesnote (da) </dt>
<dd>Post i et datakatalog der beskriver registreringen af et enkelt datasæt eller en enkelt dataservice.</dd>
<dt>Anvendelsesnote (en)</dt>
<dd>A description of a Dataset’s entry in the Catalogue. </dd>
<dt>Definition (en)</dt>
<dd>A record in a data catalog, describing the registration of a single dataset or data service.</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>

### genstand for registrering

<dl class="def">
<dt>URI</dt>
<dd>http://xmlns.com/foaf/0.1/primaryTopic</dd>
<dt>Anvendelsesnote (da)</dt>
<dd>Denne egenskab angiver det datasæt, den dataservice eller det katalog som er genstand for registreringen.</dd>
<dt>Anvendelsesnote (en)</dt>
<dd>This property links the Catalogue Record to the Dataset, Data service or Catalog described in the record.</dd>
<dt>Definition (en)</dt>
<dd>A document that this thing is the primary topic of.</dd>
<dt>Multiplicitet</dt>
<dd>1..1</dd>
<dt>Kravniveau</dt>
<dd>Obligatorisk</dd>
</dl>

### seneste ændringsdato

<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/modified</dd>
<dt>Anvendelsesnote (da)</dt>
<dd>Denne egenskab angiver den dato hvor katalogposten senest er blevet ændret.</dd>
<dt>Anvendelsesnote (en)</dt>
<dd>This property contains the most recent date on which the Catalogue entry was changed or modified.</dd>
<dt>Definition (en)</dt>
<dd>Date on which the resource was changed.</dd>
<dt>Multiplicitet</dt>
<dd>1..1</dd>
<dt>Kravniveau</dt>
<dd>Obligatorisk</dd>
</dl>

### udgivelsesdato

<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/issued</dd>
<dt>Anvendelsesnote (da)</dt>
<dd>Denne egenskab angiver den dato hvor beskrivelsen af datasættet eller dataservicen blev registreret i kataloget.</dd>
<dt>Anvendelsesnote (en)</dt>
<dd>This property contains the date on which the description of the Dataset was included in the Catalogue.</dd>
<dt>Definition (en)</dt>
<dd>Date of formal issuance of the resource.</dd>
<dt>Multiplicitet</dt>
<dd>0..1</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>

### titel

<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/title</dd>
<dt>Anvendelsesnote (da)</dt>
<dd>Denne egenskab angiver det eller de ord som navngiver katalogposten. Egenskaben kan gentages for hver sprogvariant.</dd>
<dt>Anvendelsesnote (en)</dt>
<dd>This property contains a name given to the Catalogue Record. This property can be repeated for parallel language versions of the name.</dd>
<dt>Definition (en)</dt>
<dd>A name given to the resource.</dd>
<dt>Multiplicitet</dt>
<dd>0..*</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>

### beskrivelse

<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/description</dd>
<dt>Anvendelsesnote (da)</dt>
<dd>Denne egenskab giver en tekstbaseret beskrivelse af katalogposten. Egenskaben kan gentages for hvert sprogvariant af beskrivelsen</dd>
<dt>Anvendelsesnote (en)</dt>
<dd>This property contains a free-text account of the record. This property can be repeated for parallel language versions of the description.</dd>
<dt>Definition (en)</dt>
<dd>An account of the resource.</dd>
<dt>Multiplicitet</dt>
<dd>0..*</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>

### status

<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/adms#status</dd>
<dt>Anvendelsesnote (da)</dt>
<dd>Denne egenskab angiver hvilken tilstand katalogposten befinder sig ift. udvikling og ibrugtagning. (Udfaldsrum: Completed, Deprecated, Under Development, Withdrawn)   </dd>
<dt>Anvendelsesnote (en)</dt>
<dd>This property refers to the type of the latest revision of a Dataset's entry in the Catalogue. </dd>
<dt>Definition (en)</dt>
<dd>Links to the status of the Asset or Asset Distribution in the context of a particular workflow process. 
									Since Status is defined using a skos:Concept, that is the defined range for this property.</dd>
<dt>Multiplicitet</dt>
<dd>0..1</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>

### sprog

<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/language</dd>
<dt>Anvendelsesnote (da)</dt>
<dd>Denne egenskab angiver et sprog som er anvendt til tekstbaserede metadata om dataset og dataservices i kataloget. Egenskaben kan gentages for hver sprogvariant metadata forefindes på. </dd>
<dt>Anvendelsesnote (en)</dt>
<dd>This property refers to a language used in the textual metadata describing titles, descriptions, etc. of the Dataset. This property can be repeated if the metadata is provided in multiple languages.</dd>
<dt>Definition (en)</dt>
<dd>A language of the resource.</dd>
<dt>Multiplicitet</dt>
<dd>0..*</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>

### kilde

<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/source</dd>
<dt>Anvendelsesnote (da)</dt>
<dd>Denne egenskab angiver de oprindelige metadata som blev anvendt til oprettelse af metadata om det aktuelle datasæt eller den aktuelle dataservice.</dd>
<dt>Anvendelsesnote (en)</dt>
<dd>This property refers to the original metadata that was used in creating metadata for the Dataset.</dd>
<dt>Definition (en)</dt>
<dd>A related resource from which the described resource is derived.</dd>
<dt>Multiplicitet</dt>
<dd>0..1</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>

### overenstemmelse

<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/conformsTo</dd>
<dt>Anvendelsesnote (da)</dt>
<dd>Denne egenskab angiver en specifikation (anvendelsesprofil) som datasættets metadata er i overenstemmmelse med.</dd>
<dt>Anvendelsesnote (en)</dt>
<dd>This property refers to an Application Profile that the Dataset’s metadata conforms to</dd>
<dt>Definition (en)</dt>
<dd>An established standard to which the described resource conforms.</dd>
<dt>Multiplicitet</dt>
<dd>0..1</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>

## Datasæt

<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/dcat#Dataset</dd>
<dt>Anvendelsesnote (da) </dt>
<dd>En samling a data, udgivet eller organiseret af en enkelt kilde og som der er adgang til i en eller flere repræsentationer.</dd>
<dt>Anvendelsesnote (en)</dt>
<dd>A conceptual entity that represents the information published. </dd>
<dt>Definition (en)</dt>
<dd>A collection of data, published or curated by a single agent, and available for access or download in one or more representations.</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>

### identifikator

<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/identifier</dd>
<dt>Anvendelsesnote (da)</dt>
<dd>Denne egenskab angiver en global identifikator for datasættet, for eksempel en URI eller anden identifikator som er stabil og globalt unik</dd>
<dt>Anvendelsesnote (en)</dt>
<dd>This property contains the main identifier for the Dataset, e.g. the URI or other unique identifier in the context of the Catalogue.</dd>
<dt>Definition (en)</dt>
<dd>An unambiguous reference to the resource within a given context.</dd>
<dt>Multiplicitet</dt>
<dd>0..*</dd>
<dt>Kravniveau</dt>
<dd>Obligatorisk</dd>
</dl>

### anden identifikator

<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/adms#identifier</dd>
<dt>Anvendelsesnote (da)</dt>
<dd>Denne egenskab angiver lokal identifikator for datasættet.</dd>
<dt>Anvendelsesnote (en)</dt>
<dd>This property refers to a secondary identifier of the Dataset, such as MAST/ADS[1], DataCite[2], DOI[3], EZID[4] or W3ID[5].</dd>
<dt>Definition (en)</dt>
<dd>adms:identifier is used to link any resource to an instance of adms:Identifier which is its range</dd>
<dt>Multiplicitet</dt>
<dd>0..*</dd>
<dt>Kravniveau</dt>
<dd>Valgfri</dd>
</dl>

### titel

<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/title</dd>
<dt>Anvendelsesnote (da)</dt>
<dd>Denne egenskab angiver det eller de ord som navngiver datasættet. Egenskaben kan gentages for hver sprogvariant.</dd>
<dt>Anvendelsesnote (en)</dt>
<dd>This property contains a name given to the Dataset. This property can be repeated for parallel language versions of the name.</dd>
<dt>Definition (en)</dt>
<dd>A name given to the resource.</dd>
<dt>Multiplicitet</dt>
<dd>1..*</dd>
<dt>Kravniveau</dt>
<dd>Obligatorisk</dd>
</dl>

### beskrivelse

<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/description</dd>
<dt>Anvendelsesnote (da)</dt>
<dd>Denne egenskab giver en tekstbaseret beskrivelse af datasættets formål og indhold. Egenskaben kan gentages for hvert sprog.</dd>
<dt>Anvendelsesnote (en)</dt>
<dd>This property contains a free-text account of the Dataset. This property can be repeated for parallel language versions of the description.</dd>
<dt>Definition (en)</dt>
<dd>An account of the resource.</dd>
<dt>Multiplicitet</dt>
<dd>1..*</dd>
<dt>Kravniveau</dt>
<dd>Obligatorisk</dd>
</dl>

### udgiver

<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/publisher</dd>
<dt>Anvendelsesnote (da)</dt>
<dd>Denne egenskab angiver den aktør (organisation) som primært er ansvarlig for at gøre datasættet tilgængelig.</dd>
<dt>Anvendelsesnote (en)</dt>
<dd>This property refers to the entity (organisation) responsible for making the Dataset available.</dd>
<dt>Definition (en)</dt>
<dd>An entity responsible for making the resource available.</dd>
<dt>Multiplicitet</dt>
<dd>0..1</dd>
<dt>Kravniveau</dt>
<dd>Anbefalet</dd>
</dl>

### dataansvarlig organisation

<dl class="def">
<dt>URI</dt>
<dd>https://data.gov.dk/model/core/dcat-dk/dataresponsibleorganisation</dd>
<dt>Anvendelsesnote (da)</dt>
<dd>Denne egenskab angiver den aktør der er ansvarlig for den overordnede administration af alle forhold omkring et datasæt </dd>
<dt>Anvendelsesnote (en)</dt>
<dd>This property refers to the agent responsible for the general administration of all aspects concerning a dataset</dd>
<dt>Definition (en)</dt>
<dd>aktør der er ansvarlig for den overordnede administration af alle forhold omkring et datasætagent responsible for the general administration of all aspects concerning a dataset</dd>
<dt>Multiplicitet</dt>
<dd>0..1</dd>
<dt>Kravniveau</dt>
<dd>Anbefalet</dd>
</dl>

### skaber

<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/creator</dd>
<dt>Anvendelsesnote (da)</dt>
<dd>Denne egenskab angiver den aktør der er primært ansvarlig datasættets skabelse.</dd>
<dt>Anvendelsesnote (en)</dt>
<dd>This property refers to the entity primarily responsible for producing the dataset</dd>
<dt>Definition (en)</dt>
<dd>An entity responsible for making the resource.</dd>
<dt>Multiplicitet</dt>
<dd>0..1</dd>
<dt>Kravniveau</dt>
<dd>Valgfri</dd>
</dl>

### bidragsyder

<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/contributor</dd>
<dt>Anvendelsesnote (da)</dt>
<dd>Denne egenskab angiver en aktør der er har bidraget til datasættets skabelse.</dd>
<dt>Anvendelsesnote (en)</dt>
<dd>This property refers to the entity responsible for making contributions to the resource.</dd>
<dt>Definition (en)</dt>
<dd>n entity responsible for making contributions to the resource.</dd>
<dt>Multiplicitet</dt>
<dd>0..</dd>
<dt>Kravniveau</dt>
<dd>Valgfri</dd>
</dl>

### vedligeholder

<dl class="def">
<dt>URI</dt>
<dd>http://schema.org/maintainer</dd>
<dt>Anvendelsesnote (da)</dt>
<dd>Denne egenskab angiver en aktør der administrerer bidrag til eller udgivelsen af et datasæt.</dd>
<dt>Anvendelsesnote (en)</dt>
<dd>This property refers to the agent that manages contributions to, and/or publication of a dataset.</dd>
<dt>Definition (en)</dt>
<dd>A maintainer of a Dataset, software package (SoftwareApplication), or other Project.</dd>
<dt>Multiplicitet</dt>
<dd>0..</dd>
<dt>Kravniveau</dt>
<dd>Valgfri</dd>
</dl>

### kontaktpunkt

<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/dcat#contactPoint</dd>
<dt>Anvendelsesnote (da)</dt>
<dd>Denne egenskab angiver kontaktoplysninger som kan anvendes til at indsende spørgsmål eller kommentarer om datasættet.</dd>
<dt>Anvendelsesnote (en)</dt>
<dd>This property contains contact information that can be used for sending comments about the Dataset.</dd>
<dt>Definition (en)</dt>
<dd>Relevant contact information for the catalogued resource. Use of vCard is recommended.</dd>
<dt>Multiplicitet</dt>
<dd>0..*</dd>
<dt>Kravniveau</dt>
<dd>Anbefalet</dd>
</dl>

### distribution

<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/dcat#distribution</dd>
<dt>Anvendelsesnote (da)</dt>
<dd>Denne egenskab angiver en tilgænglig distribution af datasættet.</dd>
<dt>Anvendelsesnote (en)</dt>
<dd>This property links the Dataset to an available Distribution.</dd>
<dt>Definition (en)</dt>
<dd>An available distribution of the dataset.</dd>
<dt>Multiplicitet</dt>
<dd>0..*</dd>
<dt>Kravniveau</dt>
<dd>Anbefalet</dd>
</dl>

### uddrag

<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/adms#sample</dd>
<dt>Anvendelsesnote (da)</dt>
<dd>Denne egenskab angiver et uddrag af en distribution af datasættet</dd>
<dt>Anvendelsesnote (en)</dt>
<dd>This property refers to a sample distribution of the dataset.</dd>
<dt>Definition (en)</dt>
<dd>Links to a sample of an Asset (which is itself an Asset)</dd>
<dt>Multiplicitet</dt>
<dd>0..*</dd>
<dt>Kravniveau</dt>
<dd>Valgfri</dd>
</dl>

### destinationsside

<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/dcat#landingPage</dd>
<dt>Anvendelsesnote (da)</dt>
<dd>Denne egenskab angiver en webside som giver adgang til datasættet, dets distributioner og/eller yderliger information. 
		Egenskaben bør pege på en webside hos den oprindelige dataudstiller - ikke en side eller et websted hos tredjepart, såsom en aggregator.</dd>
<dt>Anvendelsesnote (en)</dt>
<dd>This property refers to a web page that provides access to the Dataset, its Distributions and/or additional information. 
		It is intended to point to a landing page at the original data provider, not to a page on a site of a third party, such as an aggregator.</dd>
<dt>Definition (en)</dt>
<dd>A Web page that can be navigated to in a Web browser to gain access to the catalog, a dataset, its distributions and/or additional information.</dd>
<dt>Multiplicitet</dt>
<dd>0..*</dd>
<dt>Kravniveau</dt>
<dd>Anbefalet</dd>
</dl>

### overenstemmelse

<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/conformsTo</dd>
<dt>Anvendelsesnote (da)</dt>
<dd>Denne egenskab angiver en specifikation som datasættet er i overenstemmmelse med.</dd>
<dt>Anvendelsesnote (en)</dt>
<dd>This property refers to an implementing rule or other specification.</dd>
<dt>Definition (en)</dt>
<dd>An established standard to which the described resource conforms.</dd>
<dt>Multiplicitet</dt>
<dd>0..*</dd>
<dt>Kravniveau</dt>
<dd>Anbefalet</dd>
</dl>

### dokumentation

<dl class="def">
<dt>URI</dt>
<dd>http://xmlns.com/foaf/0.1/page</dd>
<dt>Anvendelsesnote (da)</dt>
<dd>Denne egenskab angiver en webside eller et dokument som beskriver datasættet.</dd>
<dt>Anvendelsesnote (en)</dt>
<dd>This property refers to a page or document about this Dataset.</dd>
<dt>Definition (en)</dt>
<dd>A page or document about this thing.</dd>
<dt>Multiplicitet</dt>
<dd>0..*</dd>
<dt>Kravniveau</dt>
<dd>Anbefalet</dd>
</dl>

### emne

<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/dcat#theme</dd>
<dt>Anvendelsesnote (da)</dt>
<dd>Denne egenskab angiver et centralt emne for datasættet. Et datasæt kan have flere centrale emner.</dd>
<dt>Anvendelsesnote (en)</dt>
<dd>This property refers to a category of the Dataset. A Dataset may be associated with multiple themes.</dd>
<dt>Definition (en)</dt>
<dd>A main category of the resource. A resource can have multiple themes.</dd>
<dt>Multiplicitet</dt>
<dd>0..*</dd>
<dt>Kravniveau</dt>
<dd>Anbefalet</dd>
</dl>

### type

<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/type</dd>
<dt>Anvendelsesnote (da)</dt>
<dd>Denne egenskab angiver datasættets type i forhold til dets genre eller iboende karakter.</dd>
<dt>Anvendelsesnote (en)</dt>
<dd>This property refers to the type of the Dataset. A controlled vocabulary for the values has not been established.</dd>
<dt>Definition (en)</dt>
<dd>The nature or genre of the resource.</dd>
<dt>Multiplicitet</dt>
<dd>0..1</dd>
<dt>Kravniveau</dt>
<dd>Valgfri</dd>
</dl>

### søgeord

<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/dcat#keyword</dd>
<dt>Anvendelsesnote (da)</dt>
<dd>Denne egenskab angiver et ord eller tag der kan bruges som grundlag for en søgning</dd>
<dt>Anvendelsesnote (en)</dt>
<dd>This property contains a keyword or tag describing the Dataset.</dd>
<dt>Definition (en)</dt>
<dd>A keyword or tag describing the resource.</dd>
<dt>Multiplicitet</dt>
<dd>0..*</dd>
<dt>Kravniveau</dt>
<dd>Valgfri</dd>
</dl>

### sprog

<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/language</dd>
<dt>Anvendelsesnote (da)</dt>
<dd>Denne egenskab angiver det sprog der er anvendt i datasættet. Egenskaben kan gentages for hver sprogvariant.</dd>
<dt>Anvendelsesnote (en)</dt>
<dd>This property refers to a language of the Dataset. This property can be repeated if there are multiple languages in the Dataset.</dd>
<dt>Definition (en)</dt>
<dd>A language of the resource.</dd>
<dt>Multiplicitet</dt>
<dd>0..*</dd>
<dt>Kravniveau</dt>
<dd>Anbefalet</dd>
</dl>

### adgangsrettigheder

<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/accessRights</dd>
<dt>Anvendelsesnote (da)</dt>
<dd>Denne egenskab angiver oplysninger hvem der har rettighed til at tilgå datasættet. Via en klassifikation kan det angives hvorvidt datasættet er åbent, har adgangsbegrænsninger eller om det ikke er tilgængeligt. (Udfaldsrum: PUBLIC, RESTRICTED, NON_PUBLIC)</dd>
<dt>Anvendelsesnote (en)</dt>
<dd>This property refers to information that indicates whether the Dataset is open data, has access restrictions or is not public. A controlled vocabulary with three members (:public, :restricted, :non-public) will be created and maintained by the Publications Office of the EU. </dd>
<dt>Definition (en)</dt>
<dd>Information about who access the resource or an indication of its security status.</dd>
<dt>Multiplicitet</dt>
<dd>0..1</dd>
<dt>Kravniveau</dt>
<dd>Valgfri</dd>
</dl>

### geografisk område

<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/spatial</dd>
<dt>Anvendelsesnote (da)</dt>
<dd>Denne egenskab angiver et geografisk område som datasættet dækker.</dd>
<dt>Anvendelsesnote (en)</dt>
<dd>This property refers to a geographic region that is covered by the Dataset. </dd>
<dt>Definition (en)</dt>
<dd>Spatial characteristics of the resource.</dd>
<dt>Multiplicitet</dt>
<dd>0..*</dd>
<dt>Kravniveau</dt>
<dd>Valgfri</dd>
</dl>

### rumlig opløsning (i meter)

<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/dcat#spatialResolutionInMeters</dd>
<dt>Anvendelsesnote (da)</dt>
<dd>Denne egenskab angivermindste rumlige afstand som kan resolveres i et datasæt, målt i meter.</dd>
<dt>Anvendelsesnote (en)</dt>
<dd>This property refers to the minimum spatial separation resolvable in a dataset, measured in meters.</dd>
<dt>Definition (en)</dt>
<dd>minimum spatial separation resolvable in a dataset, measured in metres.</dd>
<dt>Multiplicitet</dt>
<dd>0..*</dd>
<dt>Kravniveau</dt>
<dd>Valgfri</dd>
</dl>

### dækningsperiode

<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/temporal</dd>
<dt>Anvendelsesnote (da)</dt>
<dd>Denne egenskab angiver den periode datasættet dækker</dd>
<dt>Anvendelsesnote (en)</dt>
<dd>This property refers to a temporal period that the Dataset covers.</dd>
<dt>Definition (en)</dt>
<dd>Temporal characteristics of the resource.</dd>
<dt>Multiplicitet</dt>
<dd>0..*</dd>
<dt>Kravniveau</dt>
<dd>Valgfri</dd>
</dl>

### tidslig opløsning

<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/dcat#temporalResolution</dd>
<dt>Anvendelsesnote (da)</dt>
<dd>Denne egenskab angiver mindste tidsperiode der kan resolveres i datasættet.</dd>
<dt>Anvendelsesnote (en)</dt>
<dd>This property refers to the minimum time period resolvable in the dataset.</dd>
<dt>Definition (en)</dt>
<dd>minimum time period resolvable in a dataset.</dd>
<dt>Multiplicitet</dt>
<dd>0..*</dd>
<dt>Kravniveau</dt>
<dd>Valgfri</dd>
</dl>

### opdateringsfrekvens

<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/accrualPeriodicity</dd>
<dt>Anvendelsesnote (da)</dt>
<dd>Denne egenskab angiver med hvilken frekvens datasættet opdateres.</dd>
<dt>Anvendelsesnote (en)</dt>
<dd>This property refers to the frequency at which the Dataset is updated.</dd>
<dt>Definition (en)</dt>
<dd>A rate at which something recurs.</dd>
<dt>Multiplicitet</dt>
<dd>0..1</dd>
<dt>Kravniveau</dt>
<dd>Anbefalet</dd>
</dl>

### udgivelsesdato

<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/issued</dd>
<dt>Anvendelsesnote (da)</dt>
<dd>Denne egenskab angiver den dato hvor datasættet først blev formelt udgivet</dd>
<dt>Anvendelsesnote (en)</dt>
<dd>This property contains the date of formal issuance (e.g., publication) of the Dataset.</dd>
<dt>Definition (en)</dt>
<dd>Date of formal issuance of the resource.</dd>
<dt>Multiplicitet</dt>
<dd>0..1</dd>
<dt>Kravniveau</dt>
<dd>Valgfri</dd>
</dl>

### opdateringsdato

<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/modified</dd>
<dt>Anvendelsesnote (da)</dt>
<dd>Denne egenskab angiver den dato hvor datasættet senest er blevet ændret.</dd>
<dt>Anvendelsesnote (en)</dt>
<dd>This property contains the most recent date on which the Dataset was changed or modified.</dd>
<dt>Definition (en)</dt>
<dd>Date on which the resource was changed.</dd>
<dt>Multiplicitet</dt>
<dd>0..1</dd>
<dt>Kravniveau</dt>
<dd>Valgfri</dd>
</dl>

### har kvalitetsmetadata

<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/dqv#hasQualityMetadata</dd>
<dt>Anvendelsesnote (da)</dt>
<dd>Denne egenskab angiver en gruppering af kvalitetsinformation så som certifikater, politikker, målinger og annotationer som en navngiven graf </dd>
<dt>Anvendelsesnote (en)</dt>
<dd>This property refers to a grouping of quality information such as certificates, policies, measurements and annotations as a named graph.</dd>
<dt>Definition (en)</dt>
<dd>Refers to a grouping of quality information such as certificates, policies, measurements and annotations as a named graph. Quality information represented in such a grouping can pertain to any kind of resource (e.g., a dataset, a linkset, a graph, a set of triples). However, in the DQV context, this property is generally expected to be used in statements in which subjects are instances of dcat:Dataset or dcat:Distribution.</dd>
<dt>Multiplicitet</dt>
<dd>0..1</dd>
<dt>Kravniveau</dt>
<dd>Valgfri</dd>
</dl>

### har anvendelse

<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/duv#usage</dd>
<dt>Anvendelsesnote (da)</dt>
<dd>Denne egenskab angiver instruktioner eller vejledning til anvendelse af datasættet.</dd>
<dt>Anvendelsesnote (en)</dt>
<dd>This property refers to dataset or distribution usage guidance/instructions.</dd>
<dt>Definition (en)</dt>
<dd>Dataset or distribution usage guidance/instructions.</dd>
<dt>Multiplicitet</dt>
<dd>0..1</dd>
<dt>Kravniveau</dt>
<dd>Valgfri</dd>
</dl>

### betalingspålagt

<dl class="def">
<dt>URI</dt>
<dd>https://data.gov.dk/model/core/dcat-dk/paymentImposedContents</dd>
<dt>Anvendelsesnote (da)</dt>
<dd>Denne egenskab angiver hvorvidt datasættet er betalingspålagt eller ej</dd>
<dt>Anvendelsesnote (en)</dt>
<dd>This property specifies whether payment is imposed on the dataset or not</dd>
<dt>Definition (en)</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd>0..1</dd>
<dt>Kravniveau</dt>
<dd>Valgfri</dd>
</dl>

### personoplysningskategori

<dl class="def">
<dt>URI</dt>
<dd>https://data.gov.dk/model/core/dcat-dk/paymentImposedContents</dd>
<dt>Anvendelsesnote (da)</dt>
<dd>Denne egenskab angiver en relation til en bestemt personoplysningskategori.</dd>
<dt>Anvendelsesnote (en)</dt>
<dd>This property specifies a relation to specific personal data category</dd>
<dt>Definition (en)</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd>0..*</dd>
<dt>Kravniveau</dt>
<dd>Valgfri</dd>
</dl>

### fortrolighedsgrad

<dl class="def">
<dt>URI</dt>
<dd>https://data.gov.dk/model/core/dcat-dk/paymentImposedContents</dd>
<dt>Anvendelsesnote (da)</dt>
<dd>Denne egenskab angiver i hvilket omfang information indeholdt i et datasæt kan videregives.</dd>
<dt>Anvendelsesnote (en)</dt>
<dd>This property specifies the extent by which information contained in a dataset can be disclosed.</dd>
<dt>Definition (en)</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd>0..1</dd>
<dt>Kravniveau</dt>
<dd>Valgfri</dd>
</dl>

### hjemmel

<dl class="def">
<dt>URI</dt>
<dd>http://data.europa.eu/m8g/hasLegalResource</dd>
<dt>Anvendelsesnote (da)</dt>
<dd>Denne egenskab angiver med hvilken hjemmel datasættet blev skabt.</dd>
<dt>Anvendelsesnote (en)</dt>
<dd>This property specifies the legal framework for the dataset.</dd>
<dt>Definition (en)</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd>0..*</dd>
<dt>Kravniveau</dt>
<dd>Valgfri</dd>
</dl>

### versionsnummer

<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/2002/07/owl#versionInfo</dd>
<dt>Anvendelsesnote (da)</dt>
<dd>Denne egenskab angiver en versionsnummer eller anden versionsangivelse af datasættet.</dd>
<dt>Anvendelsesnote (en)</dt>
<dd>This property contains a version number or other version designation of the Dataset.</dd>
<dt>Definition (en)</dt>
<dd>The annotation property that provides version information for an ontology or another OWL construct.</dd>
<dt>Multiplicitet</dt>
<dd>0..1</dd>
<dt>Kravniveau</dt>
<dd>Valgfri</dd>
</dl>

### versionsnoter

<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/adms#versionNotes</dd>
<dt>Anvendelsesnote (da)</dt>
<dd>Denne egenskab angiver en beskrivelse af forskellene mellem den aktuelle version og forrige version af datasættet. Denne egenskab kan genrages for hver sprogvariant af versionsnoterne.</dd>
<dt>Anvendelsesnote (en)</dt>
<dd>This property contains a description of the differences between this version and a previous version of the Dataset. This property can be repeated for parallel language versions of the version notes.</dd>
<dt>Definition (en)</dt>
<dd>A description of changes between this version and the previous version of the Asset</dd>
<dt>Multiplicitet</dt>
<dd>0..*</dd>
<dt>Kravniveau</dt>
<dd>Valgfri</dd>
</dl>

### har version

<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/hasVersion</dd>
<dt>Anvendelsesnote (da)</dt>
<dd>Denne egenskab angiver et relateret datasæt som er en version, udgave eller bearbejdelse af et aktuelle datasæt.</dd>
<dt>Anvendelsesnote (en)</dt>
<dd>This property refers to a related Dataset that is a version, edition, or adaptation of the described Dataset.</dd>
<dt>Definition (en)</dt>
<dd>A related resource that is a version, edition, or adaptation of the described resource.</dd>
<dt>Multiplicitet</dt>
<dd>0..*</dd>
<dt>Kravniveau</dt>
<dd>Valgfri</dd>
</dl>

### er version af

<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/isVersionOf</dd>
<dt>Anvendelsesnote (da)</dt>
<dd>Denne egenskab angiver et relateret datasæt som det aktuelle datasæt er en version, udgave eller bearbejdelse af.</dd>
<dt>Anvendelsesnote (en)</dt>
<dd>This property refers to a related Dataset of which the described Dataset is a version, edition, or adaptation.</dd>
<dt>Definition (en)</dt>
<dd>A related resource of which the described resource is a version, edition, or adaptation.</dd>
<dt>Multiplicitet</dt>
<dd>0..*</dd>
<dt>Kravniveau</dt>
<dd>Valgfri</dd>
</dl>

### proveniensudsagn

<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/provenance</dd>
<dt>Anvendelsesnote (da)</dt>
<dd>Denne egenskab angiver udsagn omkring datasættets proveniens i form af udsagn eventuelle aktørskift som er centrale for autenciteten, integriteten og fortolkningen af datasættet.</dd>
<dt>Anvendelsesnote (en)</dt>
<dd>This property contains a statement about the lineage of a Dataset.</dd>
<dt>Definition (en)</dt>
<dd>A statement of any changes in ownership and custody of the resource since its creation that are significant for its authenticity, integrity, and interpretation.</dd>
<dt>Multiplicitet</dt>
<dd>0..*</dd>
<dt>Kravniveau</dt>
<dd>Valgfri</dd>
</dl>

### relateret ressource

<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/relation</dd>
<dt>Anvendelsesnote (da)</dt>
<dd>Denne egenskab angiver en relateret ressource</dd>
<dt>Anvendelsesnote (en)</dt>
<dd>This property refers to a related resource.</dd>
<dt>Definition (en)</dt>
<dd>A related resource.</dd>
<dt>Multiplicitet</dt>
<dd>0..*</dd>
<dt>Kravniveau</dt>
<dd>Valgfri</dd>
</dl>

### kildedatasæt

<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/source</dd>
<dt>Anvendelsesnote (da)</dt>
<dd>Denne egenskab angiver et relateret datasæt hvoraf de aktuelle datasæt er afledt.</dd>
<dt>Anvendelsesnote (en)</dt>
<dd>This property refers to a related Dataset from which the described Dataset is derived.</dd>
<dt>Definition (en)</dt>
<dd>A related resource from which the described resource is derived.</dd>
<dt>Multiplicitet</dt>
<dd>0..*</dd>
<dt>Kravniveau</dt>
<dd>Valgfri</dd>
</dl>

### refereres af

<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/elements/1.1/isReferencedBy</dd>
<dt>Anvendelsesnote (da)</dt>
<dd>Denne egenskab angiver en reference til en beskrivelse af en relation til en anden ressource.</dd>
<dt>Anvendelsesnote (en)</dt>
<dd>This property provides a link to a description of a relationship with another resource.</dd>
<dt>Definition (en)</dt>
<dd>A related resource that references, cites, or otherwise points to the described resource.</dd>
<dt>Multiplicitet</dt>
<dd>0..*</dd>
<dt>Kravniveau</dt>
<dd>Valgfri</dd>
</dl>

### præciseret tilskrivning

<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/prov#qualifiedAttribution</dd>
<dt>Anvendelsesnote (da)</dt>
<dd>Denne egenskab tilskriver en aktør et bestemt ansvar i forbindelse med datasættet.</dd>
<dt>Anvendelsesnote (en)</dt>
<dd>This property refers to a link to an Agent having some form of responsibility for the resource</dd>
<dt>Definition (en)</dt>
<dd>Attribution is the ascribing of an entity to an agent. When an entity e is attributed to agent ag, entity e was generated by some unspecified activity that in turn was associated to agent ag. Thus, this relation is useful when the activity is not known, or irrelevant.</dd>
<dt>Multiplicitet</dt>
<dd>0..*</dd>
<dt>Kravniveau</dt>
<dd>Valgfri</dd>
</dl>

### præciseret relation

<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/dcat#qualifiedRelation</dd>
<dt>Anvendelsesnote (da)</dt>
<dd>Denne egenskab angiver en nærmere klassificeret relation til en anden ressource såsom en publikation der referer, citerer eller på anden på peger på datasættet. Anvendes til at referere til en anden ressource hvor relationens betydning er kendt men ikke matcher en af de standardiserede egenskaber fra Dublin Core.</dd>
<dt>Anvendelsesnote (en)</dt>
<dd>This property is about a related resource, such as a publication, that references, cites, or otherwise points to the dataset.</dd>
<dt>Definition (en)</dt>
<dd>Link to a description of a relationship with another resource.</dd>
<dt>Multiplicitet</dt>
<dd>0..*</dd>
<dt>Kravniveau</dt>
<dd>Valgfri</dd>
</dl>

### blev genereret ved

<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/prov#wasGeneratedBy</dd>
<dt>Anvendelsesnote (da)</dt>
<dd>Denne egenskab angiver den aktivitet der genererede eller leverede forretningskonteksten for datasættets skabelse.</dd>
<dt>Anvendelsesnote (en)</dt>
<dd>This property refers to an activity that generated, or provides the business context for, the creation of the dataset.</dd>
<dt>Definition (en)</dt>
<dd>Generation is the completion of production of a new entity by an activity. This entity did not exist before generation and becomes available for usage after this generation.</dd>
<dt>Multiplicitet</dt>
<dd>0..*</dd>
<dt>Kravniveau</dt>
<dd>Valgfri</dd>
</dl>

## Distribution

<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/dcat#Distribution</dd>
<dt>Anvendelsesnote (da) </dt>
<dd>En fysisk repræsentation af datasættet.  Et datasæt kan være tilgængelig i mange serialiseringer der kan variere på forskellige vis, herunder sprog, medietype eller format, systemorganisering, tidslig- og rumlig opløsning, detaljeringsniveau eller profiler (der kan specificere en eller flere af ovenstående)
	</dd>
<dt>Anvendelsesnote (en)</dt>
<dd>A physical embodiment of the Dataset in a particular format.</dd>
<dt>Definition (en)</dt>
<dd>A specific representation of a dataset. A dataset might be available in multiple serializations that may differ in various ways, including natural language, media-type or format, schematic organization, temporal and spatial resolution, level of detail or profiles (which might specify </dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>

### adgangsURL

<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/dcat#accessURL</dd>
<dt>Anvendelsesnote (da)</dt>
<dd>Denne egenskab angiver en URL som giver adgang til en distribution af datasættet. </dd>
<dt>Anvendelsesnote (en)</dt>
<dd>This property contains a URL that gives access to a Distribution of the Dataset. The resource at the access URL may contain information about how to get the Dataset. </dd>
<dt>Definition (en)</dt>
<dd>A URL of a resource that gives access to a distribution of the dataset. E.g. landing page, feed, SPARQL endpoint. Use for all cases except a simple download link, in which case downloadURL is preferred.</dd>
<dt>Multiplicitet</dt>
<dd>1..*</dd>
<dt>Kravniveau</dt>
<dd>Obligatorisk</dd>
</dl>

### download-URL

<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/dcat#downloadURL</dd>
<dt>Anvendelsesnote (da)</dt>
<dd></dd>
<dt>Anvendelsesnote (en)</dt>
<dd>This property contains a URL that is a direct link to a downloadable file in a given format. </dd>
<dt>Definition (en)</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd>0..*</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>

### adgangsservice

<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/dcat#accessService</dd>
<dt>Anvendelsesnote (da)</dt>
<dd></dd>
<dt>Anvendelsesnote (en)</dt>
<dd>This property refers to a data service that gives access to the distribution of the dataset</dd>
<dt>Definition (en)</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd>0..*</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>

### 

<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/title</dd>
<dt>Anvendelsesnote (da)</dt>
<dd>titelDenne egenskab angiver det eller de ord som navngiver distributionen. Egenskaben kan gentages for hver sprogvariant.</dd>
<dt>Anvendelsesnote (en)</dt>
<dd>titleThis property contains a name given to the Distribution. This property can be repeated for parallel language versions of the description.</dd>
<dt>Definition (en)</dt>
<dd>A name given to the resource.</dd>
<dt>Multiplicitet</dt>
<dd>0..*</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>

### beskrivelse

<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/description</dd>
<dt>Anvendelsesnote (da)</dt>
<dd>tekstbaseret beskrivelse af distributionen</dd>
<dt>Anvendelsesnote (en)</dt>
<dd>This property contains a free-text account of the Distribution. This property can be repeated for parallel language versions of the description.</dd>
<dt>Definition (en)</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd>0..*</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>

### overenstemmelse

<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/conformsTo</dd>
<dt>Anvendelsesnote (da)</dt>
<dd>Denne egenskab angiver en specifikation (schema) som distributionen er i overenstemmmelse med.</dd>
<dt>Anvendelsesnote (en)</dt>
<dd>This property refers to an established schema to which the described Distribution conforms.</dd>
<dt>Definition (en)</dt>
<dd>An established standard to which the described resource conforms.</dd>
<dt>Multiplicitet</dt>
<dd>0..*</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>

### udgivelsesdato

<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/issued</dd>
<dt>Anvendelsesnote (da)</dt>
<dd>Denne egenskab angiver den dato hvor distributionen først blev formelt udgivet</dd>
<dt>Anvendelsesnote (en)</dt>
<dd>This property contains the date of formal issuance (e.g., publication) of the Distribution.</dd>
<dt>Definition (en)</dt>
<dd>Date of formal issuance of the resource.</dd>
<dt>Multiplicitet</dt>
<dd>0..1</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>

### seneste ændringsdato

<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/modified</dd>
<dt>Anvendelsesnote (da)</dt>
<dd>Denne egenskab angiver den dato hvor distributionen senest er blevet ændret.</dd>
<dt>Anvendelsesnote (en)</dt>
<dd>This property contains the most recent date on which the Distribution was changed or modified.</dd>
<dt>Definition (en)</dt>
<dd>Date on which the resource was changed.</dd>
<dt>Multiplicitet</dt>
<dd>0..1</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>

### status

<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/adms#status</dd>
<dt>Anvendelsesnote (da)</dt>
<dd>Denne egenskab angiver hvilken tilstand distributionen befinder sig ift. udvikling og ibrugtagning. (Udfaldsrum: Completed, Deprecated, Under Development, Withdrawn)  </dd>
<dt>Anvendelsesnote (en)</dt>
<dd>This property refers to the maturity of the Distribution. It MUST take one of the values Completed, Deprecated, Under Development, Withdrawn. </dd>
<dt>Definition (en)</dt>
<dd>Links to the status of the Asset or Asset Distribution in the context of a particular workflow process. 
									Since Status is defined using a skos:Concept, that is the defined range for this property.</dd>
<dt>Multiplicitet</dt>
<dd>0..1</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>

### tilgængeligstype

<dl class="def">
<dt>URI</dt>
<dd>http://data.europa.eu/r5r/availability</dd>
<dt>Anvendelsesnote (da)</dt>
<dd></dd>
<dt>Anvendelsesnote (en)</dt>
<dd>This property indicates how long it is planned to keep the Distribution of the Dataset available. </dd>
<dt>Definition (en)</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd>0..1</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>

### sprog

<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/language</dd>
<dt>Anvendelsesnote (da)</dt>
<dd></dd>
<dt>Anvendelsesnote (en)</dt>
<dd>This property refers to a language used in the Distribution. This property can be repeated if the metadata is provided in multiple languages.</dd>
<dt>Definition (en)</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd>0..*</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>

### checksum

<dl class="def">
<dt>URI</dt>
<dd>http://spdx.org/rdf/terms#checksum</dd>
<dt>Anvendelsesnote (da)</dt>
<dd></dd>
<dt>Anvendelsesnote (en)</dt>
<dd>This property provides a mechanism that can be used to verify that the contents of a distribution have not changed. The checksum is related to the downloadURL</dd>
<dt>Definition (en)</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd>0..1</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>

### bytestørrelse

<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/dcat#byteSize</dd>
<dt>Anvendelsesnote (da)</dt>
<dd></dd>
<dt>Anvendelsesnote (en)</dt>
<dd>This property contains the size of a Distribution in bytes.</dd>
<dt>Definition (en)</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd>0..1</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>

### medietype

<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/dcat#mediaType</dd>
<dt>Anvendelsesnote (da)</dt>
<dd></dd>
<dt>Anvendelsesnote (en)</dt>
<dd>This property refers to the media type of the Distribution as defined in the official register of media types managed by IANA.</dd>
<dt>Definition (en)</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd>0..1</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>

### format

<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/format</dd>
<dt>Anvendelsesnote (da)</dt>
<dd></dd>
<dt>Anvendelsesnote (en)</dt>
<dd>This property refers to the file format of the Distribution</dd>
<dt>Definition (en)</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd>0..1</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>

### kompressionsformat

<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/dcat#compressFormat</dd>
<dt>Anvendelsesnote (da)</dt>
<dd></dd>
<dt>Anvendelsesnote (en)</dt>
<dd>This property refers to the format of the file in which the data is contained in a compressed form, e.g. to reduce the size of the downloadable file. It SHOULD be expressed using a media type as defined in the official register of media types managed by IANA.</dd>
<dt>Definition (en)</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd>0..1</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>

### pakkeformat

<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/dcat#packageFormat</dd>
<dt>Anvendelsesnote (da)</dt>
<dd></dd>
<dt>Anvendelsesnote (en)</dt>
<dd>This property refers to the format of the file in which one or more data files are grouped together, e.g. to enable a set of related files to be downloaded together. It SHOULD be expressed using a media type as defined in the official register of media types managed by IANA.</dd>
<dt>Definition (en)</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd>0..1</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>

### dokumentation

<dl class="def">
<dt>URI</dt>
<dd>http://xmlns.com/foaf/0.1/page</dd>
<dt>Anvendelsesnote (da)</dt>
<dd></dd>
<dt>Anvendelsesnote (en)</dt>
<dd>This property refers to a page or document about this Distribution.</dd>
<dt>Definition (en)</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd>0..*</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>

### har politik

<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/odrl/2/hasPolicy</dd>
<dt>Anvendelsesnote (da)</dt>
<dd></dd>
<dt>Anvendelsesnote (en)</dt>
<dd>This property refers to the policy expressing the rights associated with the distribution if using the ODRL vocabulary</dd>
<dt>Definition (en)</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd>0..1</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>

### adgangsrettigheder

<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/rights</dd>
<dt>Anvendelsesnote (da)</dt>
<dd></dd>
<dt>Anvendelsesnote (en)</dt>
<dd>This property refers to a statement that specifies rights associated with the Distribution.</dd>
<dt>Definition (en)</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd>0..1</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>

### licens

<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/license</dd>
<dt>Anvendelsesnote (da)</dt>
<dd></dd>
<dt>Anvendelsesnote (en)</dt>
<dd>This property refers to the licence under which the Distribution is made available.</dd>
<dt>Definition (en)</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd>0..1</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>

### tidslig opløsning

<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/dcat#temporalResolution</dd>
<dt>Anvendelsesnote (da)</dt>
<dd></dd>
<dt>Anvendelsesnote (en)</dt>
<dd>This property refers to the minimum time period resolvable in the dataset distribution.</dd>
<dt>Definition (en)</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd>0..*</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>

### rumlig opløsning (i meter)

<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/dcat#spatialResolutionInMeters</dd>
<dt>Anvendelsesnote (da)</dt>
<dd></dd>
<dt>Anvendelsesnote (en)</dt>
<dd>This property refers to the  minimum spatial separation resolvable in a dataset distribution, measured in meters.</dd>
<dt>Definition (en)</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd>0..*</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>

## 

<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/dcat#DataService</dd>
<dt>Anvendelsesnote (da) </dt>
<dd></dd>
<dt>Anvendelsesnote (en)</dt>
<dd>A collection of operations that provides access to one or more datasets or data processing functions.</dd>
<dt>Definition (en)</dt>
<dd></dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>

### endpoint-URL

<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/dcat#endpointURL</dd>
<dt>Anvendelsesnote (da)</dt>
<dd></dd>
<dt>Anvendelsesnote (en)</dt>
<dd>The root location or primary endpoint of the service (an IRI).</dd>
<dt>Definition (en)</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd>1..*</dd>
<dt>Kravniveau</dt>
<dd>Obligatorisk</dd>
</dl>

### titel

<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/title</dd>
<dt>Anvendelsesnote (da)</dt>
<dd>Denne egenskab angiver det eller de ord som navngiver dataservicen. Egenskaben kan gentages for hver sprogvariant.</dd>
<dt>Anvendelsesnote (en)</dt>
<dd>This property contains a name given to the Data Service. This property can be repeated for parallel language versions of the name.</dd>
<dt>Definition (en)</dt>
<dd>A name given to the resource.</dd>
<dt>Multiplicitet</dt>
<dd>1..*</dd>
<dt>Kravniveau</dt>
<dd>Obligatorisk</dd>
</dl>

### endpointbeskrivelse

<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/dcat#endpointDescription</dd>
<dt>Anvendelsesnote (da)</dt>
<dd></dd>
<dt>Anvendelsesnote (en)</dt>
<dd>This property contains a description of the services available via the end-points, including their operations, parameters etc.The property gives specific details of the actual endpoint instances, while dct:conformsTo is used to indicate the general standard or specification that the endpoints implement.</dd>
<dt>Definition (en)</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd>0..*</dd>
<dt>Kravniveau</dt>
<dd>Anbefalet</dd>
</dl>

### beskrivelse

<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/description</dd>
<dt>Anvendelsesnote (da)</dt>
<dd>tekstbaseret beskrivelse af dataservicen</dd>
<dt>Anvendelsesnote (en)</dt>
<dd>This property contains a free-text account of the Data Service. This property can be repeated for parallel language versions of the description.</dd>
<dt>Definition (en)</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd>0..*</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>

### leverer datasæt

<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/dcat#servesDataset</dd>
<dt>Anvendelsesnote (da)</dt>
<dd></dd>
<dt>Anvendelsesnote (en)</dt>
<dd>This property refers to a collection of data that this data service can distribute</dd>
<dt>Definition (en)</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd>0..*</dd>
<dt>Kravniveau</dt>
<dd>Anbefalet</dd>
</dl>

### licens

<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/licence</dd>
<dt>Anvendelsesnote (da)</dt>
<dd></dd>
<dt>Anvendelsesnote (en)</dt>
<dd>This property contains the licence under which the Data service is made available.</dd>
<dt>Definition (en)</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd>0..1</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>

### adgangsrettigheder

<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/accessRights</dd>
<dt>Anvendelsesnote (da)</dt>
<dd></dd>
<dt>Anvendelsesnote (en)</dt>
<dd>This property MAY include information regarding access or restrictions based on privacy, security, or other policies.</dd>
<dt>Definition (en)</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd>0..1</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>

## Aktør

<dl class="def">
<dt>URI</dt>
<dd>http://xmlns.com/foaf/0.1/Agent</dd>
<dt>Anvendelsesnote (da) </dt>
<dd></dd>
<dt>Anvendelsesnote (en)</dt>
<dd>An entity that is associated with Catalogues and/or Datasets. If the Agent is an organisation, the use of the Organization Ontology  is recommended. </dd>
<dt>Definition (en)</dt>
<dd></dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>

### navn

<dl class="def">
<dt>URI</dt>
<dd>http://xmlns.com/foaf/0.1/name</dd>
<dt>Anvendelsesnote (da)</dt>
<dd></dd>
<dt>Anvendelsesnote (en)</dt>
<dd>This property contains a name of the agent. This property can be repeated for different versions of the name (e.g. the name in different languages)</dd>
<dt>Definition (en)</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd>1..*</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>

### aktørtype

<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/type</dd>
<dt>Anvendelsesnote (da)</dt>
<dd></dd>
<dt>Anvendelsesnote (en)</dt>
<dd>This property refers to a type of the agent that makes the Catalogue or Dataset available</dd>
<dt>Definition (en)</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd>0..1</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>

## Emneklassifikation

<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/2004/02/skos/core#ConceptScheme</dd>
<dt>Anvendelsesnote (da) </dt>
<dd></dd>
<dt>Anvendelsesnote (en)</dt>
<dd>A concept collection (e.g. controlled vocabulary) in which the Category is defined.</dd>
<dt>Definition (en)</dt>
<dd></dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>

### titel

<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/title</dd>
<dt>Anvendelsesnote (da)</dt>
<dd>Denne egenskab angiver det eller de ord som navngiver emneklassifikationen. Egenskaben kan gentages for hver sprogvariant.</dd>
<dt>Anvendelsesnote (en)</dt>
<dd>This property contains a name of the category scheme. May be repeated for different versions of the name</dd>
<dt>Definition (en)</dt>
<dd>A name given to the resource.</dd>
<dt>Multiplicitet</dt>
<dd>1..*</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>

## Klassifikationsemne

<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/2004/02/skos/core#Concept</dd>
<dt>Anvendelsesnote (da) </dt>
<dd></dd>
<dt>Anvendelsesnote (en)</dt>
<dd></dd>
<dt>Definition (en)</dt>
<dd></dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>

### foretrukken betegnelse

<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/2004/02/skos/core#prefLabel</dd>
<dt>Anvendelsesnote (da)</dt>
<dd></dd>
<dt>Anvendelsesnote (en)</dt>
<dd>This property contains a preferred label of the category. This property can be repeated for parallel language versions of the label.</dd>
<dt>Definition (en)</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd>1..*</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>

## Checksum

<dl class="def">
<dt>URI</dt>
<dd>http://spdx.org/rdf/terms#Checksum</dd>
<dt>Anvendelsesnote (da) </dt>
<dd></dd>
<dt>Anvendelsesnote (en)</dt>
<dd></dd>
<dt>Definition (en)</dt>
<dd></dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>

### algoritme

<dl class="def">
<dt>URI</dt>
<dd>http://spdx.org/rdf/terms#algorithm</dd>
<dt>Anvendelsesnote (da)</dt>
<dd></dd>
<dt>Anvendelsesnote (en)</dt>
<dd>This property identifies the algorithm used to produce the subject Checksum. Currently, SHA-1 is the only supported algorithm. It is anticipated that other algorithms will be supported at a later time.</dd>
<dt>Definition (en)</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd>1..1</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>

### checksumværdi

<dl class="def">
<dt>URI</dt>
<dd>http://spdx.org/rdf/terms#checksumValue</dd>
<dt>Anvendelsesnote (da)</dt>
<dd></dd>
<dt>Anvendelsesnote (en)</dt>
<dd>This property provides a lower case hexadecimal encoded digest value produced using a specific algorithm</dd>
<dt>Definition (en)</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd>1..1</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>

## Katalogressource

<dl class="def">
<dt>URI</dt>
<dd></dd>
<dt>Anvendelsesnote (da) </dt>
<dd></dd>
<dt>Anvendelsesnote (en)</dt>
<dd></dd>
<dt>Definition (en)</dt>
<dd>the union of Catalog, Dataset and DataService</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>

## Identifikator

<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/adms#Identifier</dd>
<dt>Anvendelsesnote (da) </dt>
<dd></dd>
<dt>Anvendelsesnote (en)</dt>
<dd></dd>
<dt>Definition (en)</dt>
<dd></dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>

### notation

<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/2004/02/skos/core#notation</dd>
<dt>Anvendelsesnote (da)</dt>
<dd></dd>
<dt>Anvendelsesnote (en)</dt>
<dd>This property contains a string that is an identifier in the context of the identifier scheme referenced by its datatype.</dd>
<dt>Definition (en)</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd>0..1</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>

## Licensdokument

<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/LicenseDocument</dd>
<dt>Anvendelsesnote (da) </dt>
<dd></dd>
<dt>Anvendelsesnote (en)</dt>
<dd></dd>
<dt>Definition (en)</dt>
<dd></dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>

### licenstype

<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/type</dd>
<dt>Anvendelsesnote (da)</dt>
<dd></dd>
<dt>Anvendelsesnote (en)</dt>
<dd>This property refers to a type of licence, e.g. indicating ‘public domain’ or ‘royalties required’.</dd>
<dt>Definition (en)</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd>0..*</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>

## Lokation

<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/Location</dd>
<dt>Anvendelsesnote (da) </dt>
<dd></dd>
<dt>Anvendelsesnote (en)</dt>
<dd></dd>
<dt>Definition (en)</dt>
<dd></dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>

### bounding box

<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/dcat#bbox</dd>
<dt>Anvendelsesnote (da)</dt>
<dd></dd>
<dt>Anvendelsesnote (en)</dt>
<dd></dd>
<dt>Definition (en)</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd>0..1</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>

### geografisk tyngdepunkt

<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/dcat#centroid</dd>
<dt>Anvendelsesnote (da)</dt>
<dd></dd>
<dt>Anvendelsesnote (en)</dt>
<dd></dd>
<dt>Definition (en)</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd>0..1</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>

### geometri

<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/locn#geometry</dd>
<dt>Anvendelsesnote (da)</dt>
<dd></dd>
<dt>Anvendelsesnote (en)</dt>
<dd></dd>
<dt>Definition (en)</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd>0..1</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>

## Periode

<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/PeriodOfTime</dd>
<dt>Anvendelsesnote (da) </dt>
<dd></dd>
<dt>Anvendelsesnote (en)</dt>
<dd></dd>
<dt>Definition (en)</dt>
<dd></dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>

### startdato

<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/dcat#startDate</dd>
<dt>Anvendelsesnote (da)</dt>
<dd></dd>
<dt>Anvendelsesnote (en)</dt>
<dd></dd>
<dt>Definition (en)</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd>0..1</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>

### slutdato

<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/dcat#endDate</dd>
<dt>Anvendelsesnote (da)</dt>
<dd></dd>
<dt>Anvendelsesnote (en)</dt>
<dd></dd>
<dt>Definition (en)</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd>0..1</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>

### har begyndelse

<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/2006/time#hasBeginning</dd>
<dt>Anvendelsesnote (da)</dt>
<dd></dd>
<dt>Anvendelsesnote (en)</dt>
<dd>beginning of a temporal entity</dd>
<dt>Definition (en)</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd>0..1</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>

### har slut

<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/2006/time#hasEnd</dd>
<dt>Anvendelsesnote (da)</dt>
<dd></dd>
<dt>Anvendelsesnote (en)</dt>
<dd></dd>
<dt>Definition (en)</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd>0..1</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>

## Relation

<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/dcat#Relationship</dd>
<dt>Anvendelsesnote (da) </dt>
<dd></dd>
<dt>Anvendelsesnote (en)</dt>
<dd></dd>
<dt>Definition (en)</dt>
<dd></dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>

### relation

<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/relation</dd>
<dt>Anvendelsesnote (da)</dt>
<dd></dd>
<dt>Anvendelsesnote (en)</dt>
<dd></dd>
<dt>Definition (en)</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd>1..*</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>

### havde rolle

<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/dcat#hadRole</dd>
<dt>Anvendelsesnote (da)</dt>
<dd></dd>
<dt>Anvendelsesnote (en)</dt>
<dd></dd>
<dt>Definition (en)</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd>1..*</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>

## Tidsdatatype

<dl class="def">
<dt>URI</dt>
<dd></dd>
<dt>Anvendelsesnote (da) </dt>
<dd></dd>
<dt>Anvendelsesnote (en)</dt>
<dd></dd>
<dt>Definition (en)</dt>
<dd>Date time date disjunction shape checks that a datatype property receives a date or a dateTime literal</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>


# Klassifikationer

I forbindelse med DCAT-AP udpeger EU Kommissionen en række klassifikationer skal anvendes til opmærkning af dels kataloger, datasæt og datasætrepræsentationer.

Her under kan I se hvilke klassifikationer der er i anevndelse ift. forskellige egenskaber/felter. Se evt. også kapitel 5 [Controlled Vocabularies i DCAT-AP] (https://joinup.ec.europa.eu/sites/default/files/distribution/access_url/2019-12/12f0dc1d-50b6-43e4-90c2-0afe213ac2be/DCAT_AP_2.0.0.pdf)

Bemærk at hvis den pågældende egenskab anvendes så er det et krav at de(n) udpegede klassifikation anvendes (med enkelte undtagelser - se noter).


## Datatemaer

Egenskab: dct:theme

KLASSIFIKATION: EU Datatemaer

URI: http://publications.europa.eu/resource/authority/data-theme
[Se klassifikationens indhold](
https://op.europa.eu/en/web/eu-vocabularies/at-concept-scheme/-/resource/authority/data-theme/?target=Browse&uri=http://publications.europa.eu/resource/authority/data-theme)


## Forvaltningsopgaver

Egenskab: dct:theme

KLASSIFIKATION: FORM (FællesOffentligeReferenceModel)

KLASSIFIKATION: KLE (KL Emnesystematik)

[Se FORM](https://www.form-online.dk/soegning)

[Se KLE](http://www.kle-online.dk/soegning)



## Opdateringsfrekvenser

Egenskab: dct:accrualPeriodicity

KLASSIFIKATION: EU Frekvenser

URI: http://publications.europa.eu/resource/authority/frequency

[Se klassifikationens indhold](https://op.europa.eu/en/web/eu-vocabularies/at-concept-scheme/-/resource/authority/frequency/?target=Browse&uri=http://publications.europa.eu/resource/authority/frequency)


## Medietyper
Egenskab: dct:mediaType

KLASSIFIKATION: Internet Assigned Numbers Authority (IANA). 

URI: http://www.iana.org/assignments/media-types/

[Se klassifikationens indhold](http://www.iana.org/assignments/media-types/media-types.xhtml)

Eksempler:
* hhttps://www.iana.org/assignments/media-types/text/html
* hhttps://www.iana.org/assignments/media-types/text/xml
* hhttps://www.iana.org/assignments/media-types/text/csv
* hhttps://www.iana.org/assignments/media-types/text/plain
* hhttps://www.iana.org/assignments/media-types/application/json
* hhttps://www.iana.org/assignments/media-types/application/xml
* hhttps://www.iana.org/assignments/media-types/application/zip
* hhttps://www.iana.org/assignments/media-types/application/pdf
* hhttps://www.iana.org/assignments/media-types/application/ld+json
* hhttps://www.iana.org/assignments/media-types/application/vnd.ms-excel (.xls)
* hhttps://www.iana.org/assignments/media-types/application/vnd.openxmlformats-officedocument.spreadsheetml.sheet (.xlsx)


## Filformater

Egenskab: dct:format

KLASSIFIKATION: EU Filtyper

URI: http://publications.europa.eu/resource/authority/file-type

[Se klassifikationens indhold](https://op.europa.eu/en/web/eu-vocabularies/at-concept-scheme/-/resource/authority/file-type/?target=Browse&uri=http://publications.europa.eu/resource/authority/file-type)

Eksempler:
* http://publications.europa.eu/resource/authority/file-type/CSV
* http://publications.europa.eu/resource/authority/file-type/XLS
* http://publications.europa.eu/resource/authority/file-type/XML
* http://publications.europa.eu/resource/authority/file-type/GML
* http://publications.europa.eu/resource/authority/file-type/RDF
* http://publications.europa.eu/resource/authority/file-type/TXT
* http://publications.europa.eu/resource/authority/file-type/ZIP
* http://publications.europa.eu/resource/authority/file-type/JSON


## Sprog
Egenskab: dct:language

KLASSIFIKATION: EU Sprog

URI: http://publications.europa.eu/resource/authority/language
 
[Se klassifikationens indhold](https://op.europa.eu/en/web/eu-vocabularies/at-dataset/-/resource/dataset/language)

Eksempler:
* http://publications.europa.eu/resource/dataset/language/DAN
* http://publications.europa.eu/resource/dataset/language/ENG


## Geografiske områder

Egenskab: dct:spatial

KLASSIFIKATION: kontinenter

URI: http://publications.europa.eu/resource/authority/continent/

[Se klassifikations indhold](https://op.europa.eu/en/web/eu-vocabularies/at-concept-scheme/-/resource/authority/continent/?target=Browse&uri=http://publications.europa.eu/resource/authority/continent](http://publications.europa.eu/resource/authority/continent) 

KLASSIFIKATION: lande

URI: http://publications.europa.eu/resource/authority/country

[Se klassifikations indhold](https://op.europa.eu/en/web/eu-vocabularies/at-concept-scheme/-/resource/authority/country/?target=Browse&uri=http://publications.europa.eu/resource/authority/country](http://publications.europa.eu/resource/authority/country)

KLASSIFIKATION: stednavne

URI: http://publications.europa.eu/resource/authority/place/

[Se klassifikations indhold](
https://op.europa.eu/en/web/eu-vocabularies/at-concept-scheme/-/resource/authority/place/?target=Browse&uri=http://publications.europa.eu/resource/authority/place](http://publications.europa.eu/resource/authority/place)

KLASSIFIKATION: Geonames

URI: http://sws.geonames.org/

[Se klassifikations indhold](http://sws.geonames.org/](http://sws.geonames.org/)


Note: The EU Vocabularies Name Authority Lists must be used for continents, countries and places that are in those lists; if a particular location is not in one of the mentioned Named Authority Lists, Geonames URIs must be used.


## Statusser
Egenskab: adms:status

KLASSIFIKATION: ADMS Statusser

URI: http://purl.org/adms/status/

[Se klassifikationens indhold](http://purl.org/adms/status/)
* http://purl.org/adms/status/Completed
* http://purl.org/adms/status/Deprecated
* http://purl.org/adms/status/UnderDevelopment
* http://purl.org/adms/status/Withdrawn


## Udgivertyper
Egenskab: dct:type (på foaf:Agent)

KLASSIFIKATION: ADMS udgivertyper

URI: http://purl.org/adms/publishertype/


[Se klassifikationens indhold](http://purl.org/adms/publishertype/)
* http://purl.org/adms/publishertype/Academia-ScientificOrganisation
* http://purl.org/adms/publishertype/Company
* http://purl.org/adms/publishertype/IndustryConsortium
* http://purl.org/adms/publishertype/LocalAuthority
* http://purl.org/adms/publishertype/NationalAuthority
* http://purl.org/adms/publishertype/NonGovernmentalOrganisation
* http://purl.org/adms/publishertype/NonProfitOrganisation
* http://purl.org/adms/publishertype/PrivateIndividual(s)
* http://purl.org/adms/publishertype/RegionalAuthority
* http://purl.org/adms/publishertype/StandardisationBody
* http://purl.org/adms/publishertype/SupraNationalAuthority"


Note: evt. fremtidig mapning til klassifikationen Offentlige organisationstyper herunder

KLASSIFIKATION: Offentlige organisationstyper 

URI: https://data.gov.dk/concept/profile/public-org-types

[Se klassifikationens indhold](https://digst.github.io/IT-System-AP/SYS-AP/docs/#klassifikation-offentlige-organisationstyper)


## Licenstyper

Egenskab: dct:license 

KLASSIFIKATION: ADMS licenstyper

URI: http://purl.org/adms/licencetype/

[Se klassifikationens indhold](http://purl.org/adms/licencetype/)  
* http://purl.org/adms/licencetype/Attribution
* http://purl.org/adms/licencetype/PublicDomain
* http://purl.org/adms/licencetype/ViralEffect-ShareAlike
* http://purl.org/adms/licencetype/ShareAlike-NotCompatible
* http://purl.org/adms/licencetype/ShareAlike-Compatible
* http://purl.org/adms/licencetype/NonCommercialUseOnly
* http://purl.org/adms/licencetype/NoDerivativeWork
* http://purl.org/adms/licencetype/RoyaltiesRequired
* http://purl.org/adms/licencetype/ReservedNames-Endorsement-OfficialStatus
* http://purl.org/adms/licencetype/NominalCost
* http://purl.org/adms/licencetype/GrantBack
* http://purl.org/adms/licencetype/JurisdictionWithinTheEU
* http://purl.org/adms/licencetype/OtherRestrictiveClauses
* http://purl.org/adms/licencetype/KnownPatentEncumbrance
* http://purl.org/adms/licencetype/UnknownIPR


## Tilgængelighedstyper

Egenskab: dcat-ap:availability

KLASSIFIKATION: Tilgængeligshedstyper (for distributioner)

URI: http://data.europa.eu/r5r/availability/

[Se klassifikationens indhold](http://data.europa.eu/r5r/availability/)
* http://data.europa.eu/r5r/availability/temporary
* http://data.europa.eu/r5r/availability/experimental
* http://data.europa.eu/r5r/availability/available
* http://data.europa.eu/r5r/availability/stable





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


