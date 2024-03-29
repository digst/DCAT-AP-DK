# DCAT-AP-DK-visning: obligatoriske klasser 
obligatoriske klasser samt obligatoriske egenskaber for disse klasser

<img src="https://github.com/digst/DCAT-AP-DK/blob/master/releases/v.2.0/docs/img/Illustration-DCAT-AP-DK-v2.0-UML-mandatory.png" alt="Diagram som viser obligatoriske klasser samt obligatoriske egenskaber for disse klasser (minimumsmodellen)">
			
## Klasse: Katalog (Catalog) 
<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/dcat#Catalog</dd>
<dt>Anvendelsesnote (da) </dt>
<dd>En udvalgt og arrangeret samling af metadata om datasæt og datatjenester i et katalog.</dd>
<dt>Kravniveau</dt>
<dd>Obligatorisk</dd>
</dl>
	 
### Klassens obligatoriske egenskaber:

Property|	URI (Range)|	Usage note|	Card |Requirement|
|---|---|---|---|---|
|titel (title)|http://purl.org/dc/terms/title	(http://www.w3.org/2001/XMLSchema#string)|Denne egenskab giver det eller de ord der navngiver kataloget. Egenskaben kan optræde én gang for hver sprogvariant af titlen. | 1..*|	 Obligatorisk|
|beskrivelse (description)|http://purl.org/dc/terms/description	(http://www.w3.org/2001/XMLSchema#string)|Denne egenskab giver en tekstbaseret beskrivelse af datakatalogets formål og indhold. Egenskaben kan optræde én gang for hver sprogvariant af beskrivelsen.| 1..*|	 Obligatorisk|
|har datasæt (dataset)|http://www.w3.org/ns/dcat#dataset	(http://www.w3.org/ns/dcat#Dataset)|Denne egenskab angiver et datasæt som er opført i kataloget| 1..*|	 Obligatorisk|
|udgiver (publisher)|http://purl.org/dc/terms/publisher	(http://xmlns.com/foaf/0.1/Agent)|Denne egenskab angiver den aktør (organisation) der er ansvarlig for at gøre kataloget tilgængeligt.| 1..1|	 Obligatorisk|	
			
## Klasse: Datasæt (Dataset) 
<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/dcat#Dataset</dd>
<dt>Anvendelsesnote (da) </dt>
<dd>En samling af data, udgivet eller udvalgt og arrangeret af en enkelt kilde og som er til rådighed for adgang eller download i en eller flere repræsentationer.</dd>
<dt>Kravniveau</dt>
<dd>Obligatorisk</dd>
</dl>
	 
### Klassens obligatoriske egenskaber:

Property|	URI (Range)|	Usage note|	Card |Requirement|
|---|---|---|---|---|
|titel (title)|http://purl.org/dc/terms/title	(http://www.w3.org/2001/XMLSchema#string)|Denne egenskab angiver det eller de ord som navngiver datasættet. Egenskaben kan optræde én gang for hver sprogvariant af titlen.| 1..*|	 Obligatorisk|
|beskrivelse (description)|http://purl.org/dc/terms/description	(http://www.w3.org/2001/XMLSchema#string)|Denne egenskab giver en tekstbaseret beskrivelse af datasættets formål og indhold. Egenskaben kan optræde én gang for hver sprogvariant af beskrivelsen.| 1..*|	 Obligatorisk|	
|udgiver (publisher)|http://purl.org/dc/terms/publisher	(http://xmlns.com/foaf/0.1/Agent)|Denne egenskab angiver den aktør (organisation) som primært er ansvarlig for at gøre datasættet tilgængelig. Ethvert datasæt i et givet katalog skal være tilknyttet mindst én aktør, enten en udgiver eller en datasætanvarlig organisation.| 0..1|	 Anbefalet|
|datasætansvarlig organisation DK (dataset responsible organisation)|https://data.gov.dk/model/core/dcat-dk/datasetResponsibleOrganisation	(https://www.w3.org/ns/org#Organization)|Denne egenskab angiver den organisation der har det juridiske ansvar for datasættet. Ethvert datasæt i et givet katalog skal være tilknyttet mindst én aktør, enten en udgiver eller en datasætanvarlig organisation. (dansk tilføjelse) | 0..1|	 Anbefalet|
			
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
|navn (name)|http://xmlns.com/foaf/0.1/name	(http://www.w3.org/2001/XMLSchema#string)|Denne egenskab angiver aktørens navn. Egenskaben kan optræde én gang for hver sprogvariant af navnet.| 1..*|	 Obligatorisk|</BODY>
