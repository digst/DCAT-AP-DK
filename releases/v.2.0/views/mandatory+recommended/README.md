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

Property|	URI (Range)|	Usage note|	Card |Requirement|
|---|---|---|---|---|
|titel (title)|http://purl.org/dc/terms/title	(http://www.w3.org/2000/01/rdf-schema#Literal)|Denne egenskab giver det eller de ord der navngiver kataloget. Egenskaben kan gentages for hver sprogvariant af titlen. | 1..*|	 Obligatorisk|
|beskrivelse (description)|http://purl.org/dc/terms/description	(http://www.w3.org/2000/01/rdf-schema#Literal)|Denne egenskab giver en tekstbaseret beskrivelse af datakatalogets formål og indhold. Egenskaben kan gentages for hvert sprogvariant af beskrivelsen| 1..*|	 Obligatorisk|
|har datasæt (dataset)|http://www.w3.org/ns/dcat#dataset	(http://www.w3.org/ns/dcat#Dataset)|Denne egenskab angiver et datasæt som er opført i kataloget| 1..*|	 Obligatorisk|
|udgiver (publisher)|http://purl.org/dc/terms/publisher	(http://xmlns.com/foaf/0.1/Agent)|Denne egenskab angiver den aktør (organisation) der er ansvarlig for at gøre kataloget tilgængeligt.| 1..1|	 Obligatorisk|
|websted (homepage)|http://xmlns.com/foaf/0.1/homepage	(http://xmlns.com/foaf/0.1/Document)|Denne egenskab angiver en webside som fungerer som katalogets hjemmeside.| 0..1|	 Anbefalet|
|udgivelsesdato (release date)|http://purl.org/dc/terms/issued	(http://www.w3.org/2001/XMLSchema#date;   http://www.w3.org/2001/XMLSchema#dateTime)|Denne egenskab angiver den dato hvor kataloget først blev formelt udgivet| 0..1|	 Anbefalet|
|seneste ændringsdato (update/modification date)|http://purl.org/dc/terms/modified	(http://www.w3.org/2001/XMLSchema#date;   http://www.w3.org/2001/XMLSchema#dateTime)|Denne egenskab angiver den dato hvor kataloget senest er blevet ændret.| 0..1|	 Anbefalet|
|emneklassifikation (themes)|http://www.w3.org/ns/dcat#themeTaxonomy	(http://www.w3.org/2004/02/skos/core#ConceptScheme)|Denne egenskab angiver en emneklassifikation der anvendes til klassifikation af datasæt og datatjenester i kataloget.| 0..*|	 Anbefalet|
|geografisk område (spatial/geographic)|http://purl.org/dc/terms/spatial	(http://purl.org/dc/terms/Location)|Denne egenskab angiver et geografisk område som kataloget dækker. Afgræsningen kan enten udtrykkes ved udpegnings af geofrafisk område eller ved anvendelse af en af følgende klassifikationen: EU Vocabularies Continents Named Authority List, EU Vocabularies Countries Named Authority List, EU Vocabularies Places Named Authority List eller Geonames (Sidstnævnte bør kun anvendes såfremt lokationen ikke findes i et af de nævnte EU Authority Lists.| 0..*|	 Anbefalet|
|sprog (language)|http://purl.org/dc/terms/language	(Anvend følgende klassifikation: ^http://publications.europa.eu/resource/dataset/language/)|Denne egenskab angiver et sprog som er anvendt til tekstbaserede metadata om datasæt og datatjenester i kataloget. Egenskaben kan gentages for hver sprogvariant metadata forefindes på. Til angivelse af sprog skal følgende klassifikation anvendes: EU Vocabularies Languages Named Authority List,  http://publications.europa.eu/resource/authority/language| 0..*|	 Anbefalet|
|licens (license)|http://purl.org/dc/terms/license	(http://purl.org/dc/terms/LicenseDocument)|Denne egenskab angiver den licens kataloget kan anvendes eller genbruges under.Et juridisk dokument der fastlægger de officielle tilladelser vedrørende en ressource.| 0..1|	 Anbefalet|	
			
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

Property|	URI (Range)|	Usage note|	Card |Requirement|
|---|---|---|---|---|
|identifikator (identifier)|http://purl.org/dc/terms/identifier	(http://www.w3.org/2000/01/rdf-schema#Literal)|Denne egenskab angiver en global identifikator for datasættet, for eksempel en URI eller anden identifikator som er stabil og globalt unik| 0..*|	 Anbefalet|
|titel (title)|http://purl.org/dc/terms/title	(http://www.w3.org/2000/01/rdf-schema#Literal)|Denne egenskab angiver det eller de ord som navngiver datasættet. Egenskaben kan gentages for hver sprogvariant.| 1..*|	 Obligatorisk|
|beskrivelse (description)|http://purl.org/dc/terms/description	(http://www.w3.org/2000/01/rdf-schema#Literal)|Denne egenskab giver en tekstbaseret beskrivelse af datasættets formål og indhold. Egenskaben kan gentages for hvert sprog.| 1..*|	 Obligatorisk|
|udgiver (publisher)|http://purl.org/dc/terms/publisher	(http://xmlns.com/foaf/0.1/Agent)|Denne egenskab angiver den aktør (organisation) som primært er ansvarlig for at gøre datasættet tilgængelig.| 0..1|	 Anbefalet|
|datasætansvarlig organisation DK (dataset responsible organisation)|https://data.gov.dk/model/core/dcat-dk/datasetresponsibleorganisation	(http://xmlns.com/foaf/0.1/Agent)|Denne egenskab angiver den aktør der er ansvarlig for den overordnede administration af alle forhold omkring et datasæt. (dansk tilføjelse) | 0..1|	 Anbefalet|
|kontaktpunkt (contact point)|http://www.w3.org/ns/dcat#contactPoint	(http://www.w3.org/2006/vcard/ns#Kind)|Denne egenskab angiver kontaktoplysninger som kan anvendes til at indsende spørgsmål eller kommentarer om datasættet.| 0..*|	 Anbefalet|
|har distribution (dataset distribution)|http://www.w3.org/ns/dcat#distribution	(http://www.w3.org/ns/dcat#Distribution)|Denne egenskab angiver en tilgængelig distribution af datasættet.| 0..*|	 Anbefalet|
|destinationsside (landing page)|http://www.w3.org/ns/dcat#landingPage	(http://xmlns.com/foaf/0.1/Document)|Denne egenskab angiver en webside som giver adgang til datasættet, dets distributioner og/eller yderligere information. Egenskaben bør pege på en webside hos den oprindelige dataudstiller - ikke en side eller et websted hos tredjepart, såsom en aggregator.| 0..*|	 Anbefalet|
|overenstemmelse (conforms to)|http://purl.org/dc/terms/conformsTo	(http://purl.org/dc/terms/Standard)|Denne egenskab angiver en specifikation som datasættet er i overensstemmmelse med.| 0..*|	 Anbefalet|
|dokumentation (documentation)|http://xmlns.com/foaf/0.1/page	(http://xmlns.com/foaf/0.1/Document)|Denne egenskab angiver en webside eller et dokument som beskriver datasættet.| 0..*|	 Anbefalet|
|emne (theme/ category)|http://www.w3.org/ns/dcat#theme	(Anvend følgende klassifikation: ^http://publications.europa.eu/resource/authority/data-theme/)|Denne egenskab angiver et centralt emne for datasættet. Et datasæt kan have flere centrale emner. Til angivelse af emne skal følgende klassifikation anvendes: EU Dataset Theme Vocabulary:  http://publications.europa.eu/resource/authority/data-theme| 0..*|	 Anbefalet|
|sprog (language)|http://purl.org/dc/terms/language	(Anvend følgende klassifikation: ^http://publications.europa.eu/resource/dataset/language/)|Denne egenskab angiver det sprog der er anvendt i datasættet. Egenskaben kan gentages for hver sprogvariant. Til angivelse af sprog skal følgende klassifikation anvendes: EU Vocabularies Languages Named Authority List, http://publications.europa.eu/resource/authority/language | 0..*|	 Anbefalet|
|opdateringsfrekvens (frequency)|http://purl.org/dc/terms/accrualPeriodicity	(Anvend følgende klassifikation: ^http://publications.europa.eu/resource/authority/frequency/)|Denne egenskab angiver med hvilken frekvens datasættet opdateres. Til angivelse af frekvens skal følgende klassifikation anvendes: EU Authority Table Frequencym http://publications.europa.eu/resource/authority/frequency | 0..1|	 Anbefalet|	
			
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

Property|	URI (Range)|	Usage note|	Card |Requirement|
|---|---|---|---|---|
|adgangsadresse (access address)|http://www.w3.org/ns/dcat#accessURL	(http://www.w3.org/2001/XMLSchema#anyURI)|Denne egenskab angiver en URL som giver adgang til en distribution af datasættet. | 1..*|	 Obligatorisk|
|beskrivelse (description)|http://purl.org/dc/terms/description	(http://www.w3.org/2000/01/rdf-schema#Literal)|Denne egenskab giver en tekstbaseret beskrivelse af distributionen| 0..*|	 Anbefalet|
|tilgængeligstype (availability)|http://data.europa.eu/r5r/availability	(Anvend følgende klassifikation: ^http://data.europa.eu/r5r/availability/)|Denne egenskab indikerer hvor længe det er planlagt at distributionen af datasættet skal være tilgængelig. Til angivelse af tilgængelighedstype skal følgende klassifikation anvendes: Distribution Availability Vocabulary, http://data.europa.eu/r5r/availability/| 0..1|	 Anbefalet|
|format (format)|http://purl.org/dc/terms/format	(Anvend følgende klassifikation: ^http://publications.europa.eu/resource/authority/file-type/)|Denne egenskab angiver filformatet for distributionen som den er defineret af 'EU Vocabularies File Type Named Authority List' (http://publications.europa.eu/resource/authority/file-type)| 0..1|	 Anbefalet|
|licens (license)|http://purl.org/dc/terms/license	(http://purl.org/dc/terms/LicenseDocument)|Denne egenskab angiver den licens distributionen er gjort tilgængelig under.| 0..1|	 Anbefalet|	
			
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

Property|	URI (Range)|	Usage note|	Card |Requirement|
|---|---|---|---|---|
|navn (name)|http://xmlns.com/foaf/0.1/name	(http://www.w3.org/2000/01/rdf-schema#Literal)|Denne egenskab angiver aktørens navn. Egenskaben kan gentages for hver sprogvariant af navnet.| 1..*|	 Obligatorisk|	
			
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

Property|	URI (Range)|	Usage note|	Card |Requirement|
|---|---|---|---|---|
|titel (title)|http://purl.org/dc/terms/title	(http://www.w3.org/2000/01/rdf-schema#Literal)|Denne egenskab angiver det eller de ord som navngiver emneklassifikationen. Egenskaben kan gentages for hver sprogvariant.| 1..*|	 Obligatorisk|	
			
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

Property|	URI (Range)|	Usage note|	Card |Requirement|
|---|---|---|---|---|
|foretrukken betegnelse (preferred label)|http://www.w3.org/2004/02/skos/core#prefLabel	(http://www.w3.org/2000/01/rdf-schema#Literal)|Denne egenskab angiver begrebets foretrukne betegnelse. Egenskaben kan gentages for hver sprogvariant af betegnelsen.| 1..*|	 Obligatorisk|	
			
## Klasse: Licensdokument (Licence Document) 
<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/LicenseDocument</dd>
<dt>Anvendelsesnote (da) </dt>
<dd>Et juridisk dokument der fastlægger de officielle tilladelser vedrørende en ressource.</dd>
<dt>Kravniveau</dt>
<dd>Anbefalet</dd>
</dl>
	 
### Klassens obligatoriske/anbefalede egenskaber:

Property|	URI (Range)|	Usage note|	Card |Requirement|
|---|---|---|---|---|
|licenstype (licence type)|http://purl.org/dc/terms/type	(Anvend følgende klassifikation: ^http://purl.org/adms/licencetype/)|Denne egenskab angiver licensens type som defineret af ADMS licence type vocabulary (http://purl.org/adms/licencetype/) | 0..*|	 Anbefalet|
