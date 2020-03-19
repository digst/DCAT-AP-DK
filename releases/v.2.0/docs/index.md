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

<h3>## Datakatalog</h3>
<dl class="def">
<dt>URI</dt>
<dd></dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>En organiseret samling af datarelaterede ressourcer i et katalog.</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>
<h4>### titel</h4>
<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/title</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>datakatalogets titel</dd>
<dt>Multiplicitet</dt>
<dd>1</dd>
<dt>Kravniveau</dt>
<dd>Obligatorisk</dd>
</dl>
<h4>### beskrivelse</h4>
<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/description</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>tekstbaseret beskrivelse af datakatalogets formål og indhold</dd>
<dt>Multiplicitet</dt>
<dd>1</dd>
<dt>Kravniveau</dt>
<dd>Obligatorisk</dd>
</dl>
<h4>### udgiver</h4>
<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/publisher</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>aktør der har udgivet kataloget</dd>
<dt>Multiplicitet</dt>
<dd>1..1</dd>
<dt>Kravniveau</dt>
<dd>Obligatorisk</dd>
</dl>
<h4>### skaber</h4>
<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/creator</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>aktør der har skabt kataloget</dd>
<dt>Multiplicitet</dt>
<dd>..1</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>
<h4>### udgivelsesdato</h4>
<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/issued</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>den dato datakataloget først blev udgivet</dd>
<dt>Multiplicitet</dt>
<dd>..1</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>
<h4>### seneste opdateringsdato</h4>
<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/modified</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>den dato hvor indholdet i datakataloget seneste er blevet ændret</dd>
<dt>Multiplicitet</dt>
<dd>..1</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>
<h4>### geografisk område</h4>
<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/spatial</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd></dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>
<h4>### sprog</h4>
<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/language</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd></dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>
<h4>### licens</h4>
<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/license</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd>..1</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>
<h4>### adgangsrettigheder</h4>
<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/rights</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd>..1</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>
<h4>### katalogpost</h4>
<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/dcat#record</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd></dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>
<h4>### emneklassifikation</h4>
<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/dcat#themeTaxonomy</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd></dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>
<h4>### dataservice</h4>
<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/dcat#service</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd></dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>
<h4>### katalog</h4>
<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/dcat#catalog</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd></dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>
<h4>### datasæt</h4>
<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/dcat#dataset</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd>1</dd>
<dt>Kravniveau</dt>
<dd>Obligatorisk</dd>
</dl>
<h4>### websted</h4>
<dl class="def">
<dt>URI</dt>
<dd>http://xmlns.com/foaf/0.1/homepage</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd>..1</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>
<h4>### delkatalog</h4>
<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/hasPart</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd></dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>
<h4>### del af katalog</h4>
<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/isPartOf</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd>..1</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>
<h3>## katalogpost</h3>
<dl class="def">
<dt>URI</dt>
<dd></dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>Post i et datakatalog der beskriver registreringen af et enkelt datasæt eller en dataservice.</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>
<h4>### </h4>
<dl class="def">
<dt>URI</dt>
<dd>http://xmlns.com/foaf/0.1/primaryTopic</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd>1..1</dd>
<dt>Kravniveau</dt>
<dd>Obligatorisk</dd>
</dl>
<h4>### titel</h4>
<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/title</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd></dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>
<h4>### beskrivelse</h4>
<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/description</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd></dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>
<h4>### udgivelsesdato</h4>
<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/issued</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd>..1</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>
<h4>### seneste ændringsdato</h4>
<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/modified</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd>1..1</dd>
<dt>Kravniveau</dt>
<dd>Obligatorisk</dd>
</dl>
<h4>### status</h4>
<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/adms#status</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd>..1</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>
<h4>### sprog</h4>
<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/language</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd></dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>
<h4>### kilde</h4>
<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/source</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd>..1</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>
<h4>### overenstemmelse</h4>
<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/conformsTo</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd>..1</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>
<h3>## Datasæt</h3>
<dl class="def">
<dt>URI</dt>
<dd></dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>En samling a data, udgivet eller organiseret af en enkelt kilde og som der er adgang til i en eller flere repræsentationer.</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>
<h4>### identifikator</h4>
<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/identifier</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>Global identifikator for datasættet, for eksempel en URI eller anden identifikator som er stabil og globalt unik</dd>
<dt>Multiplicitet</dt>
<dd></dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>
<h4>### anden identifikator</h4>
<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/adms#identifier</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd></dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>
<h4>### titel</h4>
<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/title</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>Datasættets titel. Egenskaben kan gentages for hvert sprog.</dd>
<dt>Multiplicitet</dt>
<dd>1</dd>
<dt>Kravniveau</dt>
<dd>Obligatorisk</dd>
</dl>
<h4>### beskrivelse</h4>
<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/description</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>Tekstbaseret beskrivelse af datasættets formål og indhold.  Egenskaben kan gentages for hvert sprog.</dd>
<dt>Multiplicitet</dt>
<dd>1</dd>
<dt>Kravniveau</dt>
<dd>Obligatorisk</dd>
</dl>
<h4>### udgiver</h4>
<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/publisher</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd>..1</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>
<h4>### skaber</h4>
<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/creator</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd>..1</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>
<h4>### kontaktpunkt</h4>
<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/dcat#contactPoint</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd></dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>
<h4>### distribution</h4>
<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/dcat#distribution</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd></dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>
<h4>### prøve</h4>
<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/adms#sample</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd></dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>
<h4>### destinationsside</h4>
<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/dcat#landingPage</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd></dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>
<h4>### overenstemmelse</h4>
<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/conformsTo</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd></dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>
<h4>### dokumentation</h4>
<dl class="def">
<dt>URI</dt>
<dd>http://xmlns.com/foaf/0.1/page</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd></dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>
<h4>### emne</h4>
<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/dcat#theme</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd></dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>
<h4>### type</h4>
<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/type</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd></dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>
<h4>### nøgleord</h4>
<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/dcat#keyword</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd></dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>
<h4>### sprog</h4>
<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/language</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd></dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>
<h4>### adgangsrettigheder</h4>
<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/accessRights</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd>..1</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>
<h4>### geografisk område</h4>
<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/spatial</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd></dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>
<h4>### rumlig opløsning (i meter)</h4>
<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/dcat#spatialResolutionInMeters</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd></dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>
<h4>### dækningsperiode</h4>
<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/temporal</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd></dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>
<h4>### tidslig opløsning</h4>
<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/dcat#temporalResolution</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd></dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>
<h4>### opdateringsfrekvens</h4>
<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/accrualPeriodicity</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd>..1</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>
<h4>### udgivelsesdato</h4>
<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/issued</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd>..1</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>
<h4>### ændringsdato</h4>
<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/modified</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd>..1</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>
<h4>### versionsnummer</h4>
<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/2002/07/owl#versionInfo</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd>..1</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>
<h4>### versionsnoter</h4>
<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/adms#versionNotes</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd></dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>
<h4>### har version</h4>
<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/hasVersion</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd></dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>
<h4>### er version af</h4>
<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/isVersionOf</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd></dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>
<h4>### proveniensudsagn</h4>
<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/provenance</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd></dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>
<h4>### relation</h4>
<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/relation</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd></dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>
<h4>### kildedatasæt</h4>
<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/source</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd></dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>
<h4>### refereres af</h4>
<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/elements/1.1/isReferencedBy</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd></dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>
<h4>### præciseret tilskrivning</h4>
<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/prov#qualifiedAttribution</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd></dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>
<h4>### præciseret relation</h4>
<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/dcat#qualifiedRelation</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd></dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>
<h4>### blev genereret ved</h4>
<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/prov#wasGeneratedBy</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd></dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>
<h3>## Distribution</h3>
<dl class="def">
<dt>URI</dt>
<dd></dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd></dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>
<h4>### adgangsURL</h4>
<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/dcat#accessURL</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd>1</dd>
<dt>Kravniveau</dt>
<dd>Obligatorisk</dd>
</dl>
<h4>### download-URL</h4>
<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/dcat#downloadURL</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd></dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>
<h4>### adgangsservice</h4>
<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/dcat#accessService</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd></dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>
<h4>### </h4>
<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/title</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>distributionens titel</dd>
<dt>Multiplicitet</dt>
<dd></dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>
<h4>### beskrivelse</h4>
<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/description</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>tekstbaseret beskrivelse af distributionen</dd>
<dt>Multiplicitet</dt>
<dd></dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>
<h4>### overenstemmelse</h4>
<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/conformsTo</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd></dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>
<h4>### udgivelsesdato</h4>
<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/issued</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd>..1</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>
<h4>### seneste ændringsdato</h4>
<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/modified</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd>..1</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>
<h4>### status</h4>
<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/adms#status</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd>..1</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>
<h4>### sprog</h4>
<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/language</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd></dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>
<h4>### adgangsrettigheder</h4>
<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/rights</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd>..1</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>
<h4>### checksum</h4>
<dl class="def">
<dt>URI</dt>
<dd>http://spdx.org/rdf/terms#checksum</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd>..1</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>
<h4>### byteSize</h4>
<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/dcat#byteSize</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd>..1</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>
<h4>### medietype</h4>
<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/dcat#mediaType</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd>..1</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>
<h4>### dokumentation</h4>
<dl class="def">
<dt>URI</dt>
<dd>http://xmlns.com/foaf/0.1/page</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd></dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>
<h4>### har politik</h4>
<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/odrl/2/hasPolicy</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd>..1</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>
<h4>### kompressionsformat</h4>
<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/dcat#compressFormat</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd>..1</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>
<h4>### pakkeformat</h4>
<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/dcat#packageFormat</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd>..1</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>
<h4>### tidslig opløsning</h4>
<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/dcat#temporalResolution</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd></dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>
<h4>### rumlig opløsning (i meter)</h4>
<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/dcat#spatialResolutionInMeters</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd></dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>
<h4>### tilgængeligstype</h4>
<dl class="def">
<dt>URI</dt>
<dd>http://data.europa.eu/r5ravailability</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd>..1</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>
<h4>### format</h4>
<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/format</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd>..1</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>
<h4>### licens</h4>
<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/license</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd>..1</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>
<h3>## </h3>
<dl class="def">
<dt>URI</dt>
<dd></dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd></dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>
<h4>### titel</h4>
<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/title</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>dataservicens titel</dd>
<dt>Multiplicitet</dt>
<dd>1</dd>
<dt>Kravniveau</dt>
<dd>Obligatorisk</dd>
</dl>
<h4>### beskrivelse</h4>
<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/description</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>tekstbaseret beskrivelse af dataservicen</dd>
<dt>Multiplicitet</dt>
<dd></dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>
<h4>### endpoint-URL</h4>
<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/dcat#endpointURL</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd>1</dd>
<dt>Kravniveau</dt>
<dd>Obligatorisk</dd>
</dl>
<h4>### endpointbeskrivelse</h4>
<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/dcat#endpointDescription</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd></dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>
<h4>### leverer datasæt</h4>
<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/dcat#servesDataset</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd></dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>
<h4>### licens</h4>
<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/licence</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd>..1</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>
<h4>### adgangsrettigheder</h4>
<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/accessRights</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd>..1</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>
<h3>## Aktør</h3>
<dl class="def">
<dt>URI</dt>
<dd></dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd></dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>
<h4>### navn</h4>
<dl class="def">
<dt>URI</dt>
<dd>http://xmlns.com/foaf/0.1/name</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd>1</dd>
<dt>Kravniveau</dt>
<dd>Obligatorisk</dd>
</dl>
<h4>### type</h4>
<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/type</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd>..1</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>
<h3>## Klassifikationssystem</h3>
<dl class="def">
<dt>URI</dt>
<dd></dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd></dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>
<h4>### titel</h4>
<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/title</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd>1</dd>
<dt>Kravniveau</dt>
<dd>Obligatorisk</dd>
</dl>
<h3>## Klassifikationsemne</h3>
<dl class="def">
<dt>URI</dt>
<dd></dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd></dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>
<h4>### foretrukken betegnelse</h4>
<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/2004/02/skos/core#prefLabel</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd>1</dd>
<dt>Kravniveau</dt>
<dd>Obligatorisk</dd>
</dl>
<h3>## Checksum</h3>
<dl class="def">
<dt>URI</dt>
<dd></dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd></dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>
<h4>### algoritme</h4>
<dl class="def">
<dt>URI</dt>
<dd>http://spdx.org/rdf/terms#algorithm</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd>1..1</dd>
<dt>Kravniveau</dt>
<dd>Obligatorisk</dd>
</dl>
<h4>### checksumværdi</h4>
<dl class="def">
<dt>URI</dt>
<dd>http://spdx.org/rdf/terms#checksumValue</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd>1..1</dd>
<dt>Kravniveau</dt>
<dd>Obligatorisk</dd>
</dl>
<h3>## Katalogressource</h3>
<dl class="def">
<dt>URI</dt>
<dd></dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>the union of Catalog, Dataset and DataService</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>
<h3>## Identifikator</h3>
<dl class="def">
<dt>URI</dt>
<dd></dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd></dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>
<h4>### </h4>
<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/2004/02/skos/core#notation</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd>..1</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>
<h3>## Licensdokument</h3>
<dl class="def">
<dt>URI</dt>
<dd></dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd></dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>
<h4>### </h4>
<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/type</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd></dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>
<h3>## Lokation</h3>
<dl class="def">
<dt>URI</dt>
<dd></dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd></dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>
<h4>### </h4>
<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/dcat#bbox</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd>..1</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>
<h4>### geografisk tyngdepunkt</h4>
<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/dcat#centroid</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd>..1</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>
<h4>### geometri</h4>
<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/locn#geometry</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd>..1</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>
<h3>## Periode</h3>
<dl class="def">
<dt>URI</dt>
<dd></dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd></dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>
<h4>### </h4>
<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/dcat#endDate</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd>..1</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>
<h4>### har begyndelse</h4>
<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/2006/time#hasBeginning</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd>..1</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>
<h4>### har slut</h4>
<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/2006/time#hasEnd</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd>..1</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>
<h4>### startdato</h4>
<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/dcat#startDate</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd>..1</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>
<h3>## relation</h3>
<dl class="def">
<dt>URI</dt>
<dd></dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd></dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>
<h4>### relation</h4>
<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/relation</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd>1</dd>
<dt>Kravniveau</dt>
<dd>Obligatorisk</dd>
</dl>
<h4>### havde rolle</h4>
<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/dcat#hadRole</dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd></dd>
<dt>Multiplicitet</dt>
<dd>1</dd>
<dt>Kravniveau</dt>
<dd>Obligatorisk</dd>
</dl>
<h3>## Tidsdatatype</h3>
<dl class="def">
<dt>URI</dt>
<dd></dd>
<dt>Definition</dt>
<dd></dd>
<dt>Anvendelsesnote</dt>
<dd>Date time date disjunction shape checks that a datatype property receives a date or a dateTime literal</dd>
<dt>Kravniveau</dt>
<dd></dd>
</dl>

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


