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
<dt>Definition</dt>
<dd>A curated collection of metadata about datasets</dd>
<dt>Anvendelsesnote</dt>
<dd>A catalogue or repository that hosts the Datasets being described.</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>				
### titel
<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/title</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>This property contains a name given to the Catalogue. This property can be repeated for parallel language versions of the name.</dd>
<dt>Multiplicitet</dt>
<dd>1..*</dd>
<dt>Kravniveau</dt>
<dd>Obligatorisk</dd>
</dl>				
### beskrivelse
<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/description</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>This property contains a free-text account of the Catalogue. This property can be repeated for parallel language versions of the description.</dd>
<dt>Multiplicitet</dt>
<dd>1..*</dd>
<dt>Kravniveau</dt>
<dd>Obligatorisk</dd>
</dl>				
### udgiver
<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/publisher</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>This property refers to an entity (organisation) responsible for making the Catalogue available. </dd>
<dt>Multiplicitet</dt>
<dd>1..1</dd>
<dt>Kravniveau</dt>
<dd>Obligatorisk</dd>
</dl>				
### skaber
<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/creator</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>This property refers to the entity primarily responsible for producing the catalogue</dd>
<dt>Multiplicitet</dt>
<dd>0..1</dd>
<dt>Kravniveau</dt>
<dd>Obligatorisk</dd>
</dl>				
### udgivelsesdato
<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/issued</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>This property contains the date of formal issuance (e.g., publication) of the Catalogue.</dd>
<dt>Multiplicitet</dt>
<dd>0..1</dd>
<dt>Kravniveau</dt>
<dd>Obligatorisk</dd>
</dl>				
### seneste opdateringsdato
<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/modified</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>This property contains the most recent date on which the Catalogue was changed or modified.</dd>
<dt>Multiplicitet</dt>
<dd>0..1</dd>
<dt>Kravniveau</dt>
<dd>Obligatorisk</dd>
</dl>				
### geografisk område
<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/spatial</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>This property refers to a geographical area covered by the Catalogue. </dd>
<dt>Multiplicitet</dt>
<dd>0..*</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>				
### sprog
<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/language</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>This property refers to a language used in the textual metadata describing titles, descriptions, etc. of the Datasets in the Catalogue. This property can be repeated if the metadata is provided in multiple languages.</dd>
<dt>Multiplicitet</dt>
<dd>0..*</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>				
### licens
<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/license</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>This property refers to the licence under which the Catalogue can be used or reused.</dd>
<dt>Multiplicitet</dt>
<dd>0..1</dd>
<dt>Kravniveau</dt>
<dd>Obligatorisk</dd>
</dl>				
### adgangsrettigheder
<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/rights</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>This property refers to a statement that specifies rights associated with the Catalogue.</dd>
<dt>Multiplicitet</dt>
<dd>0..1</dd>
<dt>Kravniveau</dt>
<dd>Obligatorisk</dd>
</dl>				
### katalogpost
<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/dcat#record</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>This property refers to a Catalogue Record that is part of the Catalogue</dd>
<dt>Multiplicitet</dt>
<dd>0..*</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>				
### emneklassifikation
<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/dcat#themeTaxonomy</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>This property refers to a knowledge organization system used to classify the Catalogue's Datasets.</dd>
<dt>Multiplicitet</dt>
<dd>0..*</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>				
### dataservice
<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/dcat#service</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>This property refers to a site or end-point that is listed in the catalog.</dd>
<dt>Multiplicitet</dt>
<dd>0..*</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>				
### katalog
<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/dcat#catalog</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>This property refers to a catalog whose contents are of interest in the context of this catalog</dd>
<dt>Multiplicitet</dt>
<dd>0..*</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>				
### datasæt
<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/dcat#dataset</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>This property links the Catalogue with a Dataset that is part of the Catalogue.</dd>
<dt>Multiplicitet</dt>
<dd>1..*</dd>
<dt>Kravniveau</dt>
<dd>Obligatorisk</dd>
</dl>				
### websted
<dl class="def">
<dt>URI</dt>
<dd>http://xmlns.com/foaf/0.1/homepage</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>This property refers to a web page that acts as the main page for the Catalogue.</dd>
<dt>Multiplicitet</dt>
<dd>0..1</dd>
<dt>Kravniveau</dt>
<dd>Obligatorisk</dd>
</dl>				
### delkatalog
<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/hasPart</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>This property refers to a related Catalogue that is part of the described Catalogue</dd>
<dt>Multiplicitet</dt>
<dd>0..*</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>				
### del af katalog
<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/isPartOf</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>This property refers to a related Catalogue in which the described Catalogue is physically or logically included.</dd>
<dt>Multiplicitet</dt>
<dd>0..1</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>				
## Katalogpost
<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/dcat#CatalogRecord</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>A description of a Dataset’s entry in the Catalogue. </dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>				
### genstand for registrering
<dl class="def">
<dt>URI</dt>
<dd>http://xmlns.com/foaf/0.1/primaryTopic</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>This property links the Catalogue Record to the Dataset, Data service or Catalog described in the record.</dd>
<dt>Multiplicitet</dt>
<dd>1..1</dd>
<dt>Kravniveau</dt>
<dd>Obligatorisk</dd>
</dl>				
### seneste ændringsdato
<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/modified</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>This property contains the most recent date on which the Catalogue entry was changed or modified.</dd>
<dt>Multiplicitet</dt>
<dd>1..1</dd>
<dt>Kravniveau</dt>
<dd>Obligatorisk</dd>
</dl>				
### udgivelsesdato
<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/issued</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>This property contains the date on which the description of the Dataset was included in the Catalogue.</dd>
<dt>Multiplicitet</dt>
<dd>0..1</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>				
### titel
<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/title</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>This property contains a name given to the Catalogue Record. This property can be repeated for parallel language versions of the name.</dd>
<dt>Multiplicitet</dt>
<dd>0..*</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>				
### beskrivelse
<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/description</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>This property contains a free-text account of the record. This property can be repeated for parallel language versions of the description.</dd>
<dt>Multiplicitet</dt>
<dd>0..*</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>				
### status
<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/adms#status</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>This property refers to the type of the latest revision of a Dataset's entry in the Catalogue. </dd>
<dt>Multiplicitet</dt>
<dd>0..1</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>				
### sprog
<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/language</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>This property refers to a language used in the textual metadata describing titles, descriptions, etc. of the Dataset. This property can be repeated if the metadata is provided in multiple languages.</dd>
<dt>Multiplicitet</dt>
<dd>0..*</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>				
### kilde
<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/source</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>This property refers to the original metadata that was used in creating metadata for the Dataset</dd>
<dt>Multiplicitet</dt>
<dd>0..1</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>				
### overenstemmelse
<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/conformsTo</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>This property refers to an Application Profile that the Dataset’s metadata conforms to</dd>
<dt>Multiplicitet</dt>
<dd>0..1</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>				
## Datasæt
<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/dcat#Dataset</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>A conceptual entity that represents the information published. </dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>				
### identifikator
<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/identifier</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>This property contains the main identifier for the Dataset, e.g. the URI or other unique identifier in the context of the Catalogue.</dd>
<dt>Multiplicitet</dt>
<dd>0..*</dd>
<dt>Kravniveau</dt>
<dd>Obligatorisk</dd>
</dl>				
### anden identifikator
<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/adms#identifier</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>This property refers to a secondary identifier of the Dataset, such as MAST/ADS[1], DataCite[2], DOI[3], EZID[4] or W3ID[5].</dd>
<dt>Multiplicitet</dt>
<dd>0..*</dd>
<dt>Kravniveau</dt>
<dd>Valgfri</dd>
</dl>				
### titel
<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/title</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>This property contains a name given to the Dataset. This property can be repeated for parallel language versions of the name.</dd>
<dt>Multiplicitet</dt>
<dd>1..*</dd>
<dt>Kravniveau</dt>
<dd>Obligatorisk</dd>
</dl>				
### beskrivelse
<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/description</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>This property contains a free-text account of the Dataset. This property can be repeated for parallel language versions of the description.</dd>
<dt>Multiplicitet</dt>
<dd>1..*</dd>
<dt>Kravniveau</dt>
<dd>Obligatorisk</dd>
</dl>				
### udgiver
<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/publisher</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>This property refers to the entity (organisation) responsible for making the Dataset available.</dd>
<dt>Multiplicitet</dt>
<dd>0..1</dd>
<dt>Kravniveau</dt>
<dd>Anbefalet</dd>
</dl>				
### dataansvarlig organisation
<dl class="def">
<dt>URI</dt>
<dd>https://data.gov.dk/model/core/dcat-dk/dataresponsibleorganisation</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>This property refers to the agent responsible for the general administration of all aspects concerning a dataset</dd>
<dt>Multiplicitet</dt>
<dd>0..1</dd>
<dt>Kravniveau</dt>
<dd>Anbefalet</dd>
</dl>				
### skaber
<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/creator</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>This property refers to the entity primarily responsible for producing the dataset</dd>
<dt>Multiplicitet</dt>
<dd>0..1</dd>
<dt>Kravniveau</dt>
<dd>Valgfri</dd>
</dl>				
### bidragsyder
<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/contributor</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>This property refers to the entity responsible for making contributions to the resource.</dd>
<dt>Multiplicitet</dt>
<dd>0..</dd>
<dt>Kravniveau</dt>
<dd>Valgfri</dd>
</dl>				
### vedligeholder
<dl class="def">
<dt>URI</dt>
<dd>http://schema.org/maintainer</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>This property refers to the agent that manages contributions to, and/or publication of a dataset</dd>
<dt>Multiplicitet</dt>
<dd>0..</dd>
<dt>Kravniveau</dt>
<dd>Valgfri</dd>
</dl>				
### kontaktpunkt
<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/dcat#contactPoint</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>This property contains contact information that can be used for sending comments about the Dataset.</dd>
<dt>Multiplicitet</dt>
<dd>0..*</dd>
<dt>Kravniveau</dt>
<dd>Anbefalet</dd>
</dl>				
### distribution
<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/dcat#distribution</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>This property links the Dataset to an available Distribution.</dd>
<dt>Multiplicitet</dt>
<dd>0..*</dd>
<dt>Kravniveau</dt>
<dd>Anbefalet</dd>
</dl>				
### prøve
<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/adms#sample</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>This property refers to a sample distribution of the dataset.</dd>
<dt>Multiplicitet</dt>
<dd>0..*</dd>
<dt>Kravniveau</dt>
<dd>Valgfri</dd>
</dl>				
### destinationsside
<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/dcat#landingPage</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>This property refers to a web page that provides access to the Dataset, its Distributions and/or additional information. It is intended to point to a landing page at the original data provider, not to a page on a site of a third party, such as an aggregator.</dd>
<dt>Multiplicitet</dt>
<dd>0..*</dd>
<dt>Kravniveau</dt>
<dd>Anbefalet</dd>
</dl>				
### overenstemmelse
<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/conformsTo</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>This property refers to an implementing rule or other specification.</dd>
<dt>Multiplicitet</dt>
<dd>0..*</dd>
<dt>Kravniveau</dt>
<dd>Anbefalet</dd>
</dl>				
### dokumentation
<dl class="def">
<dt>URI</dt>
<dd>http://xmlns.com/foaf/0.1/page</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>This property refers to a page or document about this Dataset.</dd>
<dt>Multiplicitet</dt>
<dd>0..*</dd>
<dt>Kravniveau</dt>
<dd>Anbefalet</dd>
</dl>				
### emne
<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/dcat#theme</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>This property refers to a category of the Dataset. A Dataset may be associated with multiple themes.</dd>
<dt>Multiplicitet</dt>
<dd>0..*</dd>
<dt>Kravniveau</dt>
<dd>Anbefalet</dd>
</dl>				
### type
<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/type</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>This property refers to the type of the Dataset. A controlled vocabulary for the values has not been established.</dd>
<dt>Multiplicitet</dt>
<dd>0..1</dd>
<dt>Kravniveau</dt>
<dd>Valgfri</dd>
</dl>				
### nøgleord
<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/dcat#keyword</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>This property contains a keyword or tag describing the Dataset.</dd>
<dt>Multiplicitet</dt>
<dd>0..*</dd>
<dt>Kravniveau</dt>
<dd>Valgfri</dd>
</dl>				
### sprog
<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/language</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>This property refers to a language of the Dataset. This property can be repeated if there are multiple languages in the Dataset.</dd>
<dt>Multiplicitet</dt>
<dd>0..*</dd>
<dt>Kravniveau</dt>
<dd>Anbefalet</dd>
</dl>				
### adgangsrettigheder
<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/accessRights</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>This property refers to information that indicates whether the Dataset is open data, has access restrictions or is not public. A controlled vocabulary with three members (:public, :restricted, :non-public) will be created and maintained by the Publications Office of the EU. </dd>
<dt>Multiplicitet</dt>
<dd>0..1</dd>
<dt>Kravniveau</dt>
<dd>Valgfri</dd>
</dl>				
### geografisk område
<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/spatial</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>This property refers to a geographic region that is covered by the Dataset. </dd>
<dt>Multiplicitet</dt>
<dd>0..*</dd>
<dt>Kravniveau</dt>
<dd>Valgfri</dd>
</dl>				
### rumlig opløsning (i meter)
<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/dcat#spatialResolutionInMeters</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd>0..*</dd>
<dt>Kravniveau</dt>
<dd>Valgfri</dd>
</dl>				
### dækningsperiode
<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/temporal</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>This property refers to a temporal period that the Dataset covers.</dd>
<dt>Multiplicitet</dt>
<dd>0..*</dd>
<dt>Kravniveau</dt>
<dd>Valgfri</dd>
</dl>				
### tidslig opløsning
<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/dcat#temporalResolution</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>This property refers to the minimum time period resolvable in the dataset.</dd>
<dt>Multiplicitet</dt>
<dd>0..*</dd>
<dt>Kravniveau</dt>
<dd>Valgfri</dd>
</dl>				
### opdateringsfrekvens
<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/accrualPeriodicity</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>This property refers to the frequency at which the Dataset is updated.</dd>
<dt>Multiplicitet</dt>
<dd>0..1</dd>
<dt>Kravniveau</dt>
<dd>Anbefalet</dd>
</dl>				
### udgivelsesdato
<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/issued</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>This property contains the date of formal issuance (e.g., publication) of the Dataset.</dd>
<dt>Multiplicitet</dt>
<dd>0..1</dd>
<dt>Kravniveau</dt>
<dd>Valgfri</dd>
</dl>				
### opdateringsdato
<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/modified</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>This property contains the most recent date on which the Dataset was changed or modified.</dd>
<dt>Multiplicitet</dt>
<dd>0..1</dd>
<dt>Kravniveau</dt>
<dd>Valgfri</dd>
</dl>				
### har kvalitetsmetadata
<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/dqv#hasQualityMetadata</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>This property refers to a grouping of quality information such as certificates, policies, measurements and annotations as a named graph.</dd>
<dt>Multiplicitet</dt>
<dd>0..1</dd>
<dt>Kravniveau</dt>
<dd>Valgfri</dd>
</dl>				
### har anvendelse
<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/duv#usage</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>This property refers to dataset or distribution usage guidance/instructions.</dd>
<dt>Multiplicitet</dt>
<dd>0..1</dd>
<dt>Kravniveau</dt>
<dd>Valgfri</dd>
</dl>				
### betalingspålagt
<dl class="def">
<dt>URI</dt>
<dd>https://data.gov.dk/model/core/dcat-dk/paymentImposedContents</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>This property specifies whether payment is imposed on the dataset or not</dd>
<dt>Multiplicitet</dt>
<dd>0..1</dd>
<dt>Kravniveau</dt>
<dd>Valgfri</dd>
</dl>				
### personoplysningskategori
<dl class="def">
<dt>URI</dt>
<dd>https://data.gov.dk/model/core/dcat-dk/paymentImposedContents</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>This property specifies a relation to specific personal data category</dd>
<dt>Multiplicitet</dt>
<dd>0..*</dd>
<dt>Kravniveau</dt>
<dd>Valgfri</dd>
</dl>				
### fortrolighedsgrad
<dl class="def">
<dt>URI</dt>
<dd>https://data.gov.dk/model/core/dcat-dk/paymentImposedContents</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>This property specifies the extent by which information contained in a dataset can be disclosed</dd>
<dt>Multiplicitet</dt>
<dd>0..1</dd>
<dt>Kravniveau</dt>
<dd>Valgfri</dd>
</dl>				
### hjemmel
<dl class="def">
<dt>URI</dt>
<dd>http://data.europa.eu/m8g/hasLegalResource</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>This property specifies the legal framework for the dataset</dd>
<dt>Multiplicitet</dt>
<dd>0..*</dd>
<dt>Kravniveau</dt>
<dd>Valgfri</dd>
</dl>				
### versionsnummer
<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/2002/07/owl#versionInfo</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>This property contains a version number or other version designation of the Dataset.</dd>
<dt>Multiplicitet</dt>
<dd>0..1</dd>
<dt>Kravniveau</dt>
<dd>Valgfri</dd>
</dl>				
### versionsnoter
<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/adms#versionNotes</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>This property contains a description of the differences between this version and a previous version of the Dataset. This property can be repeated for parallel language versions of the version notes.</dd>
<dt>Multiplicitet</dt>
<dd>0..*</dd>
<dt>Kravniveau</dt>
<dd>Valgfri</dd>
</dl>				
### har version
<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/hasVersion</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>This property refers to a related Dataset that is a version, edition, or adaptation of the described Dataset.</dd>
<dt>Multiplicitet</dt>
<dd>0..*</dd>
<dt>Kravniveau</dt>
<dd>Valgfri</dd>
</dl>				
### er version af
<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/isVersionOf</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>This property refers to a related Dataset of which the described Dataset is a version, edition, or adaptation.</dd>
<dt>Multiplicitet</dt>
<dd>0..*</dd>
<dt>Kravniveau</dt>
<dd>Valgfri</dd>
</dl>				
### proveniensudsagn
<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/provenance</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>This property contains a statement about the lineage of a Dataset.</dd>
<dt>Multiplicitet</dt>
<dd>0..*</dd>
<dt>Kravniveau</dt>
<dd>Valgfri</dd>
</dl>				
### relateret ressource
<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/relation</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>This property refers to a related resource.</dd>
<dt>Multiplicitet</dt>
<dd>0..*</dd>
<dt>Kravniveau</dt>
<dd>Valgfri</dd>
</dl>				
### kildedatasæt
<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/source</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>This property refers to a related Dataset from which the described Dataset is derived.</dd>
<dt>Multiplicitet</dt>
<dd>0..*</dd>
<dt>Kravniveau</dt>
<dd>Valgfri</dd>
</dl>				
### refereres af
<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/elements/1.1/isReferencedBy</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>This property provides a link to a description of a relationship with another resource</dd>
<dt>Multiplicitet</dt>
<dd>0..*</dd>
<dt>Kravniveau</dt>
<dd>Valgfri</dd>
</dl>				
### præciseret tilskrivning
<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/prov#qualifiedAttribution</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>This property refers to a liink to an Agent having some form of responsibility for the resource</dd>
<dt>Multiplicitet</dt>
<dd>0..*</dd>
<dt>Kravniveau</dt>
<dd>Valgfri</dd>
</dl>				
### præciseret relation
<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/dcat#qualifiedRelation</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>This property is about a related resource, such as a publication, that references, cites, or otherwise points to the dataset.</dd>
<dt>Multiplicitet</dt>
<dd>0..*</dd>
<dt>Kravniveau</dt>
<dd>Valgfri</dd>
</dl>				
### blev genereret ved
<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/prov#wasGeneratedBy</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>This property refers to an activity that generated, or provides the business context for, the creation of the dataset.</dd>
<dt>Multiplicitet</dt>
<dd>0..*</dd>
<dt>Kravniveau</dt>
<dd>Valgfri</dd>
</dl>				
## Distribution
<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/dcat#Distribution</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>A physical embodiment of the Dataset in a particular format.</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>				
### adgangsURL
<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/dcat#accessURL</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>This property contains a URL that gives access to a Distribution of the Dataset. The resource at the access URL may contain information about how to get the Dataset. </dd>
<dt>Multiplicitet</dt>
<dd>1..*</dd>
<dt>Kravniveau</dt>
<dd>Obligatorisk</dd>
</dl>				
### download-URL
<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/dcat#downloadURL</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>This property contains a URL that is a direct link to a downloadable file in a given format. </dd>
<dt>Multiplicitet</dt>
<dd>0..*</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>				
### adgangsservice
<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/dcat#accessService</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>This property refers to a data service that gives access to the distribution of the dataset</dd>
<dt>Multiplicitet</dt>
<dd>0..*</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>				
### 
<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/title</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>titleThis property contains a name given to the Distribution. This property can be repeated for parallel language versions of the description.</dd>
<dt>Multiplicitet</dt>
<dd>0..*</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>				
### beskrivelse
<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/description</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>This property contains a free-text account of the Distribution. This property can be repeated for parallel language versions of the description.</dd>
<dt>Multiplicitet</dt>
<dd>0..*</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>				
### overenstemmelse
<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/conformsTo</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>This property refers to an established schema to which the described Distribution conforms.</dd>
<dt>Multiplicitet</dt>
<dd>0..*</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>				
### udgivelsesdato
<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/issued</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>This property contains the date of formal issuance (e.g., publication) of the Distribution.</dd>
<dt>Multiplicitet</dt>
<dd>0..1</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>				
### seneste ændringsdato
<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/modified</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>This property contains the most recent date on which the Distribution was changed or modified.</dd>
<dt>Multiplicitet</dt>
<dd>0..1</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>				
### status
<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/adms#status</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>This property refers to the maturity of the Distribution. It MUST take one of the values Completed, Deprecated, Under Development, Withdrawn. </dd>
<dt>Multiplicitet</dt>
<dd>0..1</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>				
### tilgængeligstype
<dl class="def">
<dt>URI</dt>
<dd>http://data.europa.eu/r5r/availability</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>This property indicates how long it is planned to keep the Distribution of the Dataset available. </dd>
<dt>Multiplicitet</dt>
<dd>0..1</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>				
### sprog
<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/language</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>This property refers to a language used in the Distribution. This property can be repeated if the metadata is provided in multiple languages.</dd>
<dt>Multiplicitet</dt>
<dd>0..*</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>				
### checksum
<dl class="def">
<dt>URI</dt>
<dd>http://spdx.org/rdf/terms#checksum</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>This property provides a mechanism that can be used to verify that the contents of a distribution have not changed. The checksum is related to the downloadURL</dd>
<dt>Multiplicitet</dt>
<dd>0..1</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>				
### bytestørrelse
<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/dcat#byteSize</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>This property contains the size of a Distribution in bytes.</dd>
<dt>Multiplicitet</dt>
<dd>0..1</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>				
### medietype
<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/dcat#mediaType</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>This property refers to the media type of the Distribution as defined in the official register of media types managed by IANA.</dd>
<dt>Multiplicitet</dt>
<dd>0..1</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>				
### format
<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/format</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>This property refers to the file format of the Distribution</dd>
<dt>Multiplicitet</dt>
<dd>0..1</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>				
### kompressionsformat
<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/dcat#compressFormat</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>This property refers to the format of the file in which the data is contained in a compressed form, e.g. to reduce the size of the downloadable file. It SHOULD be expressed using a media type as defined in the official register of media types managed by IANA.</dd>
<dt>Multiplicitet</dt>
<dd>0..1</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>				
### pakkeformat
<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/dcat#packageFormat</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>This property refers to the format of the file in which one or more data files are grouped together, e.g. to enable a set of related files to be downloaded together. It SHOULD be expressed using a media type as defined in the official register of media types managed by IANA.</dd>
<dt>Multiplicitet</dt>
<dd>0..1</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>				
### dokumentation
<dl class="def">
<dt>URI</dt>
<dd>http://xmlns.com/foaf/0.1/page</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>This property refers to a page or document about this Distribution.</dd>
<dt>Multiplicitet</dt>
<dd>0..*</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>				
### har politik
<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/odrl/2/hasPolicy</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>This property refers to the policy expressing the rights associated with the distribution if using the ODRL vocabulary</dd>
<dt>Multiplicitet</dt>
<dd>0..1</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>				
### adgangsrettigheder
<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/rights</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>This property refers to a statement that specifies rights associated with the Distribution.</dd>
<dt>Multiplicitet</dt>
<dd>0..1</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>				
### licens
<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/license</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>This property refers to the licence under which the Distribution is made available.</dd>
<dt>Multiplicitet</dt>
<dd>0..1</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>				
### tidslig opløsning
<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/dcat#temporalResolution</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>This property refers to the minimum time period resolvable in the dataset distribution.</dd>
<dt>Multiplicitet</dt>
<dd>0..*</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>				
### rumlig opløsning (i meter)
<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/dcat#spatialResolutionInMeters</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>This property refers to the  minimum spatial separation resolvable in a dataset distribution, measured in meters.</dd>
<dt>Multiplicitet</dt>
<dd>0..*</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>				
## 
<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/dcat#DataService</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>A collection of operations that provides access to one or more datasets or data processing functions.</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>				
### endpoint-URL
<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/dcat#endpointURL</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>The root location or primary endpoint of the service (an IRI).</dd>
<dt>Multiplicitet</dt>
<dd>1..*</dd>
<dt>Kravniveau</dt>
<dd>Obligatorisk</dd>
</dl>				
### titel
<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/title</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>This property contains a name given to the Data Service. This property can be repeated for parallel language versions of the name.</dd>
<dt>Multiplicitet</dt>
<dd>1..*</dd>
<dt>Kravniveau</dt>
<dd>Obligatorisk</dd>
</dl>				
### endpointbeskrivelse
<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/dcat#endpointDescription</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>This property contains a description of the services available via the end-points, including their operations, parameters etc.The property gives specific details of the actual endpoint instances, while dct:conformsTo is used to indicate the general standard or specification that the endpoints implement.</dd>
<dt>Multiplicitet</dt>
<dd>0..*</dd>
<dt>Kravniveau</dt>
<dd>Anbefalet</dd>
</dl>				
### beskrivelse
<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/description</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>This property contains a free-text account of the Data Service. This property can be repeated for parallel language versions of the description.</dd>
<dt>Multiplicitet</dt>
<dd>0..*</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>				
### leverer datasæt
<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/dcat#servesDataset</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>This property refers to a collection of data that this data service can distribute</dd>
<dt>Multiplicitet</dt>
<dd>0..*</dd>
<dt>Kravniveau</dt>
<dd>Anbefalet</dd>
</dl>				
### licens
<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/licence</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>This property contains the licence under which the Data service is made available.</dd>
<dt>Multiplicitet</dt>
<dd>0..1</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>				
### adgangsrettigheder
<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/accessRights</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>This property MAY include information regarding access or restrictions based on privacy, security, or other policies.</dd>
<dt>Multiplicitet</dt>
<dd>0..1</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>				
## Aktør
<dl class="def">
<dt>URI</dt>
<dd>http://xmlns.com/foaf/0.1/Agent</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>An entity that is associated with Catalogues and/or Datasets. If the Agent is an organisation, the use of the Organization Ontology  is recommended. </dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>				
### navn
<dl class="def">
<dt>URI</dt>
<dd>http://xmlns.com/foaf/0.1/name</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>This property contains a name of the agent. This property can be repeated for different versions of the name (e.g. the name in different languages)</dd>
<dt>Multiplicitet</dt>
<dd>1..*</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>				
### aktørtype
<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/type</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>This property refers to a type of the agent that makes the Catalogue or Dataset available</dd>
<dt>Multiplicitet</dt>
<dd>0..1</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>				
## Emneklassifikation
<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/2004/02/skos/core#ConceptScheme</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>A concept collection (e.g. controlled vocabulary) in which the Category is defined.</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>				
### titel
<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/title</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>This property contains a name of the category scheme. May be repeated for different versions of the name</dd>
<dt>Multiplicitet</dt>
<dd>1..*</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>				
## Klassifikationsemne
<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/2004/02/skos/core#Concept</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd></dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>				
### foretrukken betegnelse
<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/2004/02/skos/core#prefLabel</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>This property contains a preferred label of the category. This property can be repeated for parallel language versions of the label.</dd>
<dt>Multiplicitet</dt>
<dd>1..*</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>				
## Checksum
<dl class="def">
<dt>URI</dt>
<dd>http://spdx.org/rdf/terms#Checksum</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd></dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>				
### algoritme
<dl class="def">
<dt>URI</dt>
<dd>http://spdx.org/rdf/terms#algorithm</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>This property identifies the algorithm used to produce the subject Checksum. Currently, SHA-1 is the only supported algorithm. It is anticipated that other algorithms will be supported at a later time.</dd>
<dt>Multiplicitet</dt>
<dd>1..1</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>				
### checksumværdi
<dl class="def">
<dt>URI</dt>
<dd>http://spdx.org/rdf/terms#checksumValue</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>This property provides a lower case hexadecimal encoded digest value produced using a specific algorithm</dd>
<dt>Multiplicitet</dt>
<dd>1..1</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>				
## Katalogressource
<dl class="def">
<dt>URI</dt>
<dd></dd>
<dt>Definition</dt>
<dd>the union of Catalog, Dataset and DataService</dd>
<dt>Anvendelsesnote</dt>
<dd></dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>				
## Identifikator
<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/adms#Identifier</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd></dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>				
### notation
<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/2004/02/skos/core#notation</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>This property contains a string that is an identifier in the context of the identifier scheme referenced by its datatype.</dd>
<dt>Multiplicitet</dt>
<dd>0..1</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>				
## Licensdokument
<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/LicenseDocument</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd></dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>				
### licenstype
<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/type</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>This property refers to a type of licence, e.g. indicating ‘public domain’ or ‘royalties required’.</dd>
<dt>Multiplicitet</dt>
<dd>0..*</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>				
## Lokation
<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/Location</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd></dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>				
### bounding box
<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/dcat#bbox</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
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
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
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
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
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
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd></dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>				
### startdato
<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/dcat#startDate</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
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
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
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
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>beginning of a temporal entity</dd>
<dt>Multiplicitet</dt>
<dd>0..1</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>				
### har slut
<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/2006/time#hasEnd</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
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
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd></dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>				
### relation
<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/relation</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
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
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
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
<dt>Definition</dt>
<dd>Date time date disjunction shape checks that a datatype property receives a date or a dateTime literal</dd>
<dt>Anvendelsesnote</dt>
<dd></dd>
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


