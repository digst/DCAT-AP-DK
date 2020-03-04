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
Editor: SDFE
Editor: ERST
Editor: STAR
Editor: KL
Editor: MFVM – Miljøportalen
Editor: Danmarks Statistik
Group: Udvalget for Arkitektur og Standarder (UAS) 


Abstract: Dette dokument 'Standard for beskrivelse af datasæt (DCAT-AP-DK)' udgør en fællesoffentlig standard for beskrivelse af offentlige myndigheders datasæt.
Boilerplate: copyright no, conformance no, abstract no
Shortname: DCAT-AP-DK
Revision: 2.0.0
Date: 2019-02-25
Max ToC Depth: 3
Markup Shorthands: markdown yes
Repository: digst/DCAT-AP-DK/DCAT-AP-DK/releases/v.2.0
Inline Github Issues: full
Logo: digst...
</pre>


<h1>UDKAST: Standard for beskrivelse af datasæt (DCAT-AP-DK 2.0)</h1>

UDKAST til Version 2.0
Februar 2020
   



# Introduktion


Dette dokument udgør en fællesoffentlig standard for beskrivelse af offentlige myndigheders datasæt. Standarden omfatter basisoplysninger om datasæt, som fx titel, beskrivelse, udgiver, udgivelsesdato mv., samt en ensartet struktur for disse oplysninger i et fælles udvekslingsformat, som gør det muligt at dele oplysninger om it-systemer på en effektiv måde. 

## Formål




## Baggrund




## Metode


Denne standard udgøres af en dansk basisprofil for datsæt (DCAT-AP-DK), som indeholder de basisoplysninger om datsæt, der indgår i typiske datasætoverblik.  Basisoplysningerne udgør en fælles kerne, der kan udvides med yderligere kontekstafhængige oplysninger, i nye og mere specifikke anvendelsesprofiler. Informationer dannet på baggrund af to eller flere specifikke anvendelsesprofiler kan potentielt bringes til at hænge sammen via denne fælles kerne.

Selve udviklingsarbejdet er foretaget i henhold de Fællesoffentlige regler for begrebs- og datamodellering, og standarden udgøres af en basisprofil, der sammensætter flere eksisterende nationale og internationale modeller.


## Konformans og afvigelser fra DCAT-AP



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


# Modellens elementer


## Katalog

A catalogue or repository that hosts the Datasets being described.


<table class=".def">
	<tr><td>URI</td><td>test</td></tr>
	<tr><td>label</td><td>test</td></tr>	
<table>	

## Aktør

An entity that is associated with Catalogues and/or Datasets. 


## Datasæt

A conceptual entity that represents the information published.


## Datasætrepræsentation

physical embodiment of the Dataset in a particular format


## Dataservice

A collection of operations that provides access to one or more datasets or data processing functions.



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


