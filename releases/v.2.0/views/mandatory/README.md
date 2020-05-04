# DCAT-AP-DK-visning: obligatoriske klasser
samt obligatoriske egenskaber for disse klasser
			
## Klasse: Katalog (Catalog) 
<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/dcat#Catalog</dd>
<dt>Anvendelsesnote (da) </dt>
<dd>En kurateret samling af metadata om datasæt og datatjenester i et katalog.</dd>
<dt>Kravniveau</dt>
<dd>Obligatorisk</dd>
</dl>
	 
### Klassens obligatoriske egenskaber:

Property|	URI (Range)|	Usage note|	Card |Requirement|
|---|---|---|---|---|
|titel (title)|http://purl.org/dc/terms/title	(http://www.w3.org/2000/01/rdf-schema#Literal)|Denne egenskab giver det eller de ord der navngiver kataloget. Egenskaben kan gentages for hver sprogvariant af titlen. | 1..*|	 Obligatorisk|
|beskrivelse (description)|http://purl.org/dc/terms/description	(http://www.w3.org/2000/01/rdf-schema#Literal)|Denne egenskab giver en tekstbaseret beskrivelse af datakatalogets formål og indhold. Egenskaben kan gentages for hvert sprogvariant af beskrivelsen| 1..*|	 Obligatorisk|
|har datasæt (dataset)|http://www.w3.org/ns/dcat#dataset	(http://www.w3.org/ns/dcat#Dataset)|Denne egenskab angiver et datasæt som er opført i kataloget| 1..*|	 Obligatorisk|
|udgiver (publisher)|http://purl.org/dc/terms/publisher	(http://xmlns.com/foaf/0.1/Agent)|Denne egenskab angiver den aktør (organisation) der er ansvarlig for at gøre kataloget tilgængeligt.| 1..1|	 Obligatorisk|	
			
## Klasse: Datasæt (Dataset) 
<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/dcat#Dataset</dd>
<dt>Anvendelsesnote (da) </dt>
<dd>En samling a data, udgivet eller kurateret af en enkelt kilde og som der er adgang til i en eller flere repræsentationer.</dd>
<dt>Kravniveau</dt>
<dd>Obligatorisk</dd>
</dl>
	 
### Klassens obligatoriske egenskaber:

Property|	URI (Range)|	Usage note|	Card |Requirement|
|---|---|---|---|---|
|identifikator (identifier)|http://purl.org/dc/terms/identifier	(http://www.w3.org/2000/01/rdf-schema#Literal)|Denne egenskab angiver en global identifikator for datasættet, for eksempel en URI eller anden identifikator som er stabil og globalt unik| 0..*|	 Obligatorisk|
|titel (title)|http://purl.org/dc/terms/title	(http://www.w3.org/2000/01/rdf-schema#Literal)|Denne egenskab angiver det eller de ord som navngiver datasættet. Egenskaben kan gentages for hver sprogvariant.| 1..*|	 Obligatorisk|
|beskrivelse (description)|http://purl.org/dc/terms/description	(http://www.w3.org/2000/01/rdf-schema#Literal)|Denne egenskab giver en tekstbaseret beskrivelse af datasættets formål og indhold. Egenskaben kan gentages for hvert sprog.| 1..*|	 Obligatorisk|	
			
## Klasse: Aktør (Agent) 
<dl class="def">
<dt>URI</dt>
<dd>http://xmlns.com/foaf/0.1/Agent</dd>
<dt>Anvendelsesnote (da) </dt>
<dd>En entitet som er tilknyttet kataloget, datasættet eller datatjenesten. Hvis aktøren er en organisation, så anbefales det at denne opmærkes med W3Cs The Organization Ontology (https://www.w3.org/TR/vocab-org/)</dd>
<dt>Kravniveau</dt>
<dd>Obligatorisk</dd>
</dl>
	 
### Klassens obligatoriske egenskaber:

Property|	URI (Range)|	Usage note|	Card |Requirement|
|---|---|---|---|---|
|navn (name)|http://xmlns.com/foaf/0.1/name	(http://www.w3.org/2000/01/rdf-schema#Literal)|Denne egenskab angiver aktørens navn. Egenskaben kan gentages for hver sprogvariant af navnet.| 1..*|	 Obligatorisk|</BODY>
</HTML>
