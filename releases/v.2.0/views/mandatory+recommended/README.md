# DCAT-AP-DK-visning: obligatoriske/ anbefalede klasser
samt obligatoriske/anbefalede egenskaber for disse klasser

			
## Klasse: Katalog (Catalog) 
<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/dcat#Catalog</dd>
<dt>Anvendelsesnote (da) </dt>
<dd>En kurateret samling af metadata om datasæt og datatjenester i et katalog.</dd>
<dt>Kravniveau</dt>
<dd>Obligatorisk</dd>
</dl>
	 
### Klassens obligatoriske/anbefalede egenskaber:

Property|	URI|	Range|	Usage note|	Card |Requirement|
|---|---|---|---|---|---|
|titel (title)|http://purl.org/dc/terms/title	|http://www.w3.org/2000/01/rdf-schema#Literal|Denne egenskab giver det eller de ord der navngiver kataloget. Egenskaben kan gentages for hver sprogvariant af titlen. | 1..*|	 Obligatorisk|
|beskrivelse (description)|http://purl.org/dc/terms/description	|http://www.w3.org/2000/01/rdf-schema#Literal|Denne egenskab giver en tekstbaseret beskrivelse af datakatalogets formål og indhold. Egenskaben kan gentages for hvert sprogvariant af beskrivelsen| 1..*|	 Obligatorisk|
|har datasæt (dataset)|http://www.w3.org/ns/dcat#dataset	|http://www.w3.org/ns/dcat#Dataset|Denne egenskab angiver et datasæt som er opført i kataloget| 1..*|	 Obligatorisk|
|udgiver (publisher)|http://purl.org/dc/terms/publisher	|http://xmlns.com/foaf/0.1/Agent|Denne egenskab angiver den aktør (organisation) der er ansvarlig for at gøre kataloget tilgængeligt.| 1..1|	 Obligatorisk|	
			
## Klasse: Datasæt (Dataset) 
<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/dcat#Dataset</dd>
<dt>Anvendelsesnote (da) </dt>
<dd>En samling a data, udgivet eller kurateret af en enkelt kilde og som der er adgang til i en eller flere repræsentationer.</dd>
<dt>Kravniveau</dt>
<dd>Obligatorisk</dd>
</dl>
	 
### Klassens obligatoriske/anbefalede egenskaber:

Property|	URI|	Range|	Usage note|	Card |Requirement|
|---|---|---|---|---|---|
|identifikator (identifier)|http://purl.org/dc/terms/identifier	|http://www.w3.org/2000/01/rdf-schema#Literal|Denne egenskab angiver en global identifikator for datasættet, for eksempel en URI eller anden identifikator som er stabil og globalt unik| 0..*|	 Obligatorisk|
|titel (title)|http://purl.org/dc/terms/title	|http://www.w3.org/2000/01/rdf-schema#Literal|Denne egenskab angiver det eller de ord som navngiver datasættet. Egenskaben kan gentages for hver sprogvariant.| 1..*|	 Obligatorisk|
|beskrivelse (description)|http://purl.org/dc/terms/description	|http://www.w3.org/2000/01/rdf-schema#Literal|Denne egenskab giver en tekstbaseret beskrivelse af datasættets formål og indhold. Egenskaben kan gentages for hvert sprog.| 1..*|	 Obligatorisk|	
			
## Klasse: Distribution (Distribution) 
<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/dcat#Distribution</dd>
<dt>Anvendelsesnote (da) </dt>
<dd>En fysisk repræsentation af datasættet. Et datasæt kan være tilgængelig i mange serialiseringer der kan variere på forskellige vis, herunder sprog, medietype eller format, systemorganisering, tidslig- og geografisk opløsning, detaljeringsniveau eller profiler (der kan specificere en eller flere af ovenstående)
	</dd>
<dt>Kravniveau</dt>
<dd>Anbefalet</dd>
</dl>
	 
### Klassens obligatoriske/anbefalede egenskaber:

Property|	URI|	Range|	Usage note|	Card |Requirement|
|---|---|---|---|---|---|
|adgangsadresse (access address)|http://www.w3.org/ns/dcat#accessURL	|http://www.w3.org/2001/XMLSchema#anyURI|Denne egenskab angiver en URL som giver adgang til en distribution af datasættet. | 1..*|	 Obligatorisk|	
			
## Klasse: Aktør (Agent) 
<dl class="def">
<dt>URI</dt>
<dd>http://xmlns.com/foaf/0.1/Agent</dd>
<dt>Anvendelsesnote (da) </dt>
<dd>En entitet som er tilknyttet kataloget, datasættet eller datatjenesten. Hvis aktøren er en organisation, så anbefales det at denne opmærkes med W3Cs The Organization Ontology (https://www.w3.org/TR/vocab-org/)</dd>
<dt>Kravniveau</dt>
<dd>Obligatorisk</dd>
</dl>
	 
### Klassens obligatoriske/anbefalede egenskaber:

Property|	URI|	Range|	Usage note|	Card |Requirement|
|---|---|---|---|---|---|
|navn (name)|http://xmlns.com/foaf/0.1/name	|http://www.w3.org/2000/01/rdf-schema#Literal|Denne egenskab angiver aktørens navn. Egenskaben kan gentages for hver sprogvariant af navnet.| 1..*|	 Obligatorisk|	
			
## Klasse: Begrebssystem (Category Scheme) 
<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/2004/02/skos/core#ConceptScheme</dd>
<dt>Anvendelsesnote (da) </dt>
<dd>En samling af begreber (fx. et kontrolleret udfaldsrum) hvori et givet begreb indgår.</dd>
<dt>Kravniveau</dt>
<dd>Anbefalet</dd>
</dl>
	 
### Klassens obligatoriske/anbefalede egenskaber:

Property|	URI|	Range|	Usage note|	Card |Requirement|
|---|---|---|---|---|---|
|titel (title)|http://purl.org/dc/terms/title	|http://www.w3.org/2000/01/rdf-schema#Literal|Denne egenskab angiver det eller de ord som navngiver emneklassifikationen. Egenskaben kan gentages for hver sprogvariant.| 1..*|	 Obligatorisk|	
			
## Klasse: Begreb (Category) 
<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/2004/02/skos/core#Concept</dd>
<dt>Anvendelsesnote (da) </dt>
<dd>En emne som klassificerer datasættet. </dd>
<dt>Kravniveau</dt>
<dd>Anbefalet</dd>
</dl>
	 
### Klassens obligatoriske/anbefalede egenskaber:

Property|	URI|	Range|	Usage note|	Card |Requirement|
|---|---|---|---|---|---|
|foretrukken betegnelse (preferred label)|http://www.w3.org/2004/02/skos/core#prefLabel	|http://www.w3.org/2000/01/rdf-schema#Literal|Denne egenskab angiver begrebets foretrukne betegnelse. Egenskaben kan gentages for hver sprogvariant af betegnelsen.| 1..*|	 Obligatorisk|	
			
## Klasse: Licensdokument (Licence Document) 
<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/LicenseDocument</dd>
<dt>Anvendelsesnote (da) </dt>
<dd>Et juridisk dokument der fastlægger de officielle tilladelser vedrørende en ressource.</dd>
<dt>Kravniveau</dt>
<dd>Anbefalet</dd>
</dl>
	 
