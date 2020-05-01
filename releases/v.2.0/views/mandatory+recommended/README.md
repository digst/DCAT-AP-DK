# DCAT-AP-DK-visning: obligatoriske/ anbefalede klasser
samt obligatoriske/anbefalede egenskaber for disse klasser

			
## Klasse: Katalog (Catalog) 
<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/dcat#Catalog</dd>
<dt>Anvendelsesnote (da) </dt>
<dd>En kurateret samling af metadata om datasæt og datatjenester i et katalog.</dd>
<dt>Anvendelsesnote (en)</dt>
<dd>A catalogue or repository that hosts the Datasets being described.</dd>
<dt>Definition (da)</dt>
<dd>En kurateret samling af metadata om ressourcer (fx. datasæt og datatjenester i kontekst af et datakatalog).</dd>
<dt>Definition (en)</dt>
<dd>A curated collection of metadata about resources (e.g., datasets and data services in the context of a data catalog).</dd>
<dt>Kravniveau</dt>
<dd>Obligatorisk</dd>
</dl>
	 
**Klassens obligatoriske/anbefalede egenskaber:**	


				
### Egenskab: titel (title) 
<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/title</dd>
<dt>Rækkevidde</dt>
<dd>http://www.w3.org/2000/01/rdf-schema#Literal</dd>
<dt>Anvendelsesnote (da)</dt>
<dd>Denne egenskab giver det eller de ord der navngiver kataloget. Egenskaben kan gentages for hver sprogvariant af titlen. </dd>
<dt>Anvendelsesnote (en)</dt>
<dd>This property contains a name given to the Catalogue. This property can be repeated for parallel language versions of the name.</dd>
<dt>Definition (da)</dt>
<dd>Et navn givet til ressourcen.</dd>
<dt>Definition (en)</dt>
<dd>A name given to the resource.</dd>
<dt>Multiplicitet</dt>
<dd>1..*</dd>
<dt>Kravniveau</dt>
<dd>Obligatorisk</dd>
</dl>
				
### Egenskab: beskrivelse (description) 
<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/description</dd>
<dt>Rækkevidde</dt>
<dd>http://www.w3.org/2000/01/rdf-schema#Literal</dd>
<dt>Anvendelsesnote (da)</dt>
<dd>Denne egenskab giver en tekstbaseret beskrivelse af datakatalogets formål og indhold. Egenskaben kan gentages for hvert sprogvariant af beskrivelsen</dd>
<dt>Anvendelsesnote (en)</dt>
<dd>This property contains a free-text account of the Catalogue. This property can be repeated for parallel language versions of the description.</dd>
<dt>Definition (da)</dt>
<dd>En forklaring af ressourcen.</dd>
<dt>Definition (en)</dt>
<dd>An account of the resource.</dd>
<dt>Multiplicitet</dt>
<dd>1..*</dd>
<dt>Kravniveau</dt>
<dd>Obligatorisk</dd>
</dl>
				
### Egenskab: har datasæt (dataset) 
<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/dcat#dataset</dd>
<dt>Rækkevidde</dt>
<dd>http://www.w3.org/ns/dcat#Dataset</dd>
<dt>Anvendelsesnote (da)</dt>
<dd>Denne egenskab angiver et datasæt som er opført i kataloget</dd>
<dt>Anvendelsesnote (en)</dt>
<dd>This property links the Catalogue with a Dataset that is part of the Catalogue.</dd>
<dt>Definition (da)</dt>
<dd>En samling af data som er opført i kataloget.</dd>
<dt>Definition (en)</dt>
<dd>A collection of data that is listed in the catalog.</dd>
<dt>Multiplicitet</dt>
<dd>1..*</dd>
<dt>Kravniveau</dt>
<dd>Obligatorisk</dd>
</dl>
				
### Egenskab: udgiver (publisher) 
<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/publisher</dd>
<dt>Rækkevidde</dt>
<dd>http://xmlns.com/foaf/0.1/Agent</dd>
<dt>Anvendelsesnote (da)</dt>
<dd>Denne egenskab angiver den aktør (organisation) der er ansvarlig for at gøre kataloget tilgængeligt.</dd>
<dt>Anvendelsesnote (en)</dt>
<dd>This property refers to an entity (organisation) responsible for making the Catalogue available. </dd>
<dt>Definition (da)</dt>
<dd>En entitet som er ansvarlig for at gøre ressourcen tilgængelig.</dd>
<dt>Definition (en)</dt>
<dd>An entity responsible for making the resource available.</dd>
<dt>Multiplicitet</dt>
<dd>1..1</dd>
<dt>Kravniveau</dt>
<dd>Obligatorisk</dd>
</dl>	
			
## Klasse: Datasæt (Dataset) 
<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/dcat#Dataset</dd>
<dt>Anvendelsesnote (da) </dt>
<dd>En samling a data, udgivet eller kurateret af en enkelt kilde og som der er adgang til i en eller flere repræsentationer.</dd>
<dt>Anvendelsesnote (en)</dt>
<dd>A conceptual entity that represents the information published. </dd>
<dt>Definition (da)</dt>
<dd>En samling af data, udgivet eller kurateret af en enkelt kilde og som er tilråde for adgang til eller download af i en eller flere repræsentationer.</dd>
<dt>Definition (en)</dt>
<dd>A collection of data, published or curated by a single agent, and available for access or download in one or more representations.</dd>
<dt>Kravniveau</dt>
<dd>Obligatorisk</dd>
</dl>
	 
**Klassens obligatoriske/anbefalede egenskaber:**	


				
### Egenskab: identifikator (identifier) 
<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/identifier</dd>
<dt>Rækkevidde</dt>
<dd>http://www.w3.org/2000/01/rdf-schema#Literal</dd>
<dt>Anvendelsesnote (da)</dt>
<dd>Denne egenskab angiver en global identifikator for datasættet, for eksempel en URI eller anden identifikator som er stabil og globalt unik</dd>
<dt>Anvendelsesnote (en)</dt>
<dd>This property contains the main identifier for the Dataset, e.g. the URI or other unique identifier in the context of the Catalogue.</dd>
<dt>Definition (da)</dt>
<dd>En entydig reference til ressourcen i en givet kontekst.</dd>
<dt>Definition (en)</dt>
<dd>An unambiguous reference to the resource within a given context.</dd>
<dt>Multiplicitet</dt>
<dd>0..*</dd>
<dt>Kravniveau</dt>
<dd>Obligatorisk</dd>
</dl>
				
### Egenskab: titel (title) 
<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/title</dd>
<dt>Rækkevidde</dt>
<dd>http://www.w3.org/2000/01/rdf-schema#Literal</dd>
<dt>Anvendelsesnote (da)</dt>
<dd>Denne egenskab angiver det eller de ord som navngiver datasættet. Egenskaben kan gentages for hver sprogvariant.</dd>
<dt>Anvendelsesnote (en)</dt>
<dd>This property contains a name given to the Dataset. This property can be repeated for parallel language versions of the name.</dd>
<dt>Definition (da)</dt>
<dd>Et navn givet til ressourcen.</dd>
<dt>Definition (en)</dt>
<dd>A name given to the resource.</dd>
<dt>Multiplicitet</dt>
<dd>1..*</dd>
<dt>Kravniveau</dt>
<dd>Obligatorisk</dd>
</dl>
				
### Egenskab: beskrivelse (description) 
<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/description</dd>
<dt>Rækkevidde</dt>
<dd>http://www.w3.org/2000/01/rdf-schema#Literal</dd>
<dt>Anvendelsesnote (da)</dt>
<dd>Denne egenskab giver en tekstbaseret beskrivelse af datasættets formål og indhold. Egenskaben kan gentages for hvert sprog.</dd>
<dt>Anvendelsesnote (en)</dt>
<dd>This property contains a free-text account of the Dataset. This property can be repeated for parallel language versions of the description.</dd>
<dt>Definition (da)</dt>
<dd>En forklaring af ressourcen.</dd>
<dt>Definition (en)</dt>
<dd>An account of the resource.</dd>
<dt>Multiplicitet</dt>
<dd>1..*</dd>
<dt>Kravniveau</dt>
<dd>Obligatorisk</dd>
</dl>	
			
## Klasse: Distribution (Distribution) 
<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/dcat#Distribution</dd>
<dt>Anvendelsesnote (da) </dt>
<dd>En fysisk repræsentation af datasættet. Et datasæt kan være tilgængelig i mange serialiseringer der kan variere på forskellige vis, herunder sprog, medietype eller format, systemorganisering, tidslig- og geografisk opløsning, detaljeringsniveau eller profiler (der kan specificere en eller flere af ovenstående)
	</dd>
<dt>Anvendelsesnote (en)</dt>
<dd>A physical embodiment of the Dataset in a particular format.</dd>
<dt>Definition (da)</dt>
<dd>En specifik repræsentation af et datasæt. Et datasæt kan være tilgængelig i mange serialiseringer der kan variere på forskellige vis, herunder sprog, medietype eller format, systemorganisering, tidslig- og geografisk opløsning, detaljeringsniveau eller profiler (der kan specificere en eller flere af ovenstående).</dd>
<dt>Definition (en)</dt>
<dd>A specific representation of a dataset. A dataset might be available in multiple serializations that may differ in various ways, including natural language, media-type or format, schematic organization, temporal and spatial resolution, level of detail or profiles (which might specify </dd>
<dt>Kravniveau</dt>
<dd>Anbefalet</dd>
</dl>
	 
**Klassens obligatoriske/anbefalede egenskaber:**	


				
### Egenskab: adgangsadresse (access address) 
<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/ns/dcat#accessURL</dd>
<dt>Rækkevidde</dt>
<dd>http://www.w3.org/2001/XMLSchema#anyURI</dd>
<dt>Anvendelsesnote (da)</dt>
<dd>Denne egenskab angiver en URL som giver adgang til en distribution af datasættet. </dd>
<dt>Anvendelsesnote (en)</dt>
<dd>This property contains a URL that gives access to a Distribution of the Dataset. The resource at the access URL may contain information about how to get the Dataset. </dd>
<dt>Definition (da)</dt>
<dd>En URL for en ressource som giver adgang til en distribution af datasættet. Fx, destinationsside, feed, SPARQL-endpoint. Anvendes i alle sammenhænge undtagen til angivelse af et simpelt download link hvor anvendelse af egenskaben download-URL foretrækkes.</dd>
<dt>Definition (en)</dt>
<dd>A URL of a resource that gives access to a distribution of the dataset. E.g. landing page, feed, SPARQL endpoint. Use for all cases except a simple download link, in which case downloadURL is preferred.</dd>
<dt>Multiplicitet</dt>
<dd>1..*</dd>
<dt>Kravniveau</dt>
<dd>Obligatorisk</dd>
</dl>	
			
## Klasse: Aktør (Agent) 
<dl class="def">
<dt>URI</dt>
<dd>http://xmlns.com/foaf/0.1/Agent</dd>
<dt>Anvendelsesnote (da) </dt>
<dd>En entitet som er tilknyttet kataloget, datasættet eller datatjenesten. Hvis aktøren er en organisation, så anbefales det at denne opmærkes med W3Cs The Organization Ontology (https://www.w3.org/TR/vocab-org/)</dd>
<dt>Anvendelsesnote (en)</dt>
<dd>An entity that is associated with Catalogues and/or Datasets. If the Agent is an organisation, the use of the Organization Ontology  is recommended. </dd>
<dt>Definition (da)</dt>
<dd>En aktør (fx. person, gruppe, software eller fysisk artefakt).</dd>
<dt>Definition (en)</dt>
<dd>An agent (eg. person, group, software or physical artifact).</dd>
<dt>Kravniveau</dt>
<dd>Obligatorisk</dd>
</dl>
	 
**Klassens obligatoriske/anbefalede egenskaber:**	


				
### Egenskab: navn (name) 
<dl class="def">
<dt>URI</dt>
<dd>http://xmlns.com/foaf/0.1/name</dd>
<dt>Rækkevidde</dt>
<dd>http://www.w3.org/2000/01/rdf-schema#Literal</dd>
<dt>Anvendelsesnote (da)</dt>
<dd>Denne egenskab angiver aktørens navn. Egenskaben kan gentages for hver sprogvariant af navnet.</dd>
<dt>Anvendelsesnote (en)</dt>
<dd>This property contains a name of the agent. This property can be repeated for different versions of the name (e.g. the name in different languages)</dd>
<dt>Definition (da)</dt>
<dd>Et navn for noget</dd>
<dt>Definition (en)</dt>
<dd>A name for some thing.</dd>
<dt>Multiplicitet</dt>
<dd>1..*</dd>
<dt>Kravniveau</dt>
<dd>Obligatorisk</dd>
</dl>	
			
## Klasse: Begrebssystem (Category Scheme) 
<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/2004/02/skos/core#ConceptScheme</dd>
<dt>Anvendelsesnote (da) </dt>
<dd>En samling af begreber (fx. et kontrolleret udfaldsrum) hvori et givet begreb indgår.</dd>
<dt>Anvendelsesnote (en)</dt>
<dd>A concept collection (e.g. controlled vocabulary) in which the Category is defined.</dd>
<dt>Definition (da)</dt>
<dd>En samling af ét eller flere begreber, samt eventuelt også udsagn om de indbyrdes semantiske relationer mellem disse begreber.</dd>
<dt>Definition (en)</dt>
<dd>A set of concepts, optionally including statements about semantic relationships between those concepts.</dd>
<dt>Kravniveau</dt>
<dd>Anbefalet</dd>
</dl>
	 
**Klassens obligatoriske/anbefalede egenskaber:**	


				
### Egenskab: titel (title) 
<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/title</dd>
<dt>Rækkevidde</dt>
<dd>http://www.w3.org/2000/01/rdf-schema#Literal</dd>
<dt>Anvendelsesnote (da)</dt>
<dd>Denne egenskab angiver det eller de ord som navngiver emneklassifikationen. Egenskaben kan gentages for hver sprogvariant.</dd>
<dt>Anvendelsesnote (en)</dt>
<dd>This property contains a name of the category scheme. May be repeated for different versions of the name</dd>
<dt>Definition (da)</dt>
<dd>Et navn givet til ressourcen.</dd>
<dt>Definition (en)</dt>
<dd>A name given to the resource.</dd>
<dt>Multiplicitet</dt>
<dd>1..*</dd>
<dt>Kravniveau</dt>
<dd>Obligatorisk</dd>
</dl>	
			
## Klasse: Begreb (Category) 
<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/2004/02/skos/core#Concept</dd>
<dt>Anvendelsesnote (da) </dt>
<dd>En emne som klassificerer datasættet. </dd>
<dt>Anvendelsesnote (en)</dt>
<dd>A subject of a Dataset.</dd>
<dt>Definition (da)</dt>
<dd>En idé eller en forestilling; en tankeenhed</dd>
<dt>Definition (en)</dt>
<dd>An idea or notion; a unit of thought.</dd>
<dt>Kravniveau</dt>
<dd>Anbefalet</dd>
</dl>
	 
**Klassens obligatoriske/anbefalede egenskaber:**	


				
### Egenskab: foretrukken betegnelse (preferred label) 
<dl class="def">
<dt>URI</dt>
<dd>http://www.w3.org/2004/02/skos/core#prefLabel</dd>
<dt>Rækkevidde</dt>
<dd>http://www.w3.org/2000/01/rdf-schema#Literal</dd>
<dt>Anvendelsesnote (da)</dt>
<dd>Denne egenskab angiver begrebets foretrukne betegnelse. Egenskaben kan gentages for hver sprogvariant af betegnelsen.</dd>
<dt>Anvendelsesnote (en)</dt>
<dd>This property contains a preferred label of the category. This property can be repeated for parallel language versions of the label.</dd>
<dt>Definition (da)</dt>
<dd>Det foretrukne leksikalske udtryk for en ressource på et givet sprog.</dd>
<dt>Definition (en)</dt>
<dd>The preferred lexical label for a resource, in a given language.</dd>
<dt>Multiplicitet</dt>
<dd>1..*</dd>
<dt>Kravniveau</dt>
<dd>Obligatorisk</dd>
</dl>	
			
## Klasse: Licensdokument (Licence Document) 
<dl class="def">
<dt>URI</dt>
<dd>http://purl.org/dc/terms/LicenseDocument</dd>
<dt>Anvendelsesnote (da) </dt>
<dd>Et juridisk dokument der fastlægger de officielle tilladelser vedrørende en ressource.</dd>
<dt>Anvendelsesnote (en)</dt>
<dd>A legal document giving official permission to do something with a resource.</dd>
<dt>Definition (da)</dt>
<dd>Et juridisk dokument der fastlægger de officielle tilladelser vedrørende en ressource.</dd>
<dt>Definition (en)</dt>
<dd>A legal document giving official permission to do something with a resource.</dd>
<dt>Kravniveau</dt>
<dd>Anbefalet</dd>
</dl>
