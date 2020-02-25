# DCAT-AP-DK v.2.0 (Under udvikling)
DCAT-AP-DK v.2.0 anvender elementer fra og er i overenstemmelse med DCAT-AP v. 2.0, men tilføjer også enkelte elementer for at opfylde behovet i en dansk administrativ og fællesoffentlig kontekst

## Link til specifikation
Link til udkast til v.2.0: https://digst.github.io/DCAT-AP-DK/releases/v.2.0/docs/

## Anvendelseprofil visualiseret med UML-diagram
![UML-diagram](https://github.com/digst/DCAT-AP-DK/blob/developmente/DCAT-AP-DKv2.png "UML Diagram")

* DCAT Application Profile for Data Portals in Europe - 2.0: 
https://joinup.ec.europa.eu/solution/dcat-application-profile-data-portals-europe/release/200
* DOCX-fil med specifikation: https://joinup.ec.europa.eu/sites/default/files/distribution/access_url/2019-12/a3dc67cb-6670-4ad2-83b9-61b118aec1f0/DCAT_AP_2.0.0.docx
+ enkelte danske tilføjelser (se nederst)


## Klasse: Catalog (katalog) 
### MANDATORY:
Property|	URI|	Range|	Usage note|	Card |
|---|---|---|---|---|
|dataset	|dcat:dataset	|dcat:Dataset|	This property links the Catalogue with a Dataset that is part of the Catalogue.|	1..n|
|description	|dct:description	|rdfs:Literal|	This property contains a free-text account of the Catalogue. |1..n|
|publisher	|dct:publisher|	foaf:Agent|	This property refers to an entity (organisation) responsible for making the Catalogue available. |	1..1||
|title	|dct:title	|rdfs:Literal|	This property contains a name given to the Catalogue. This property can be repeated for parallel language versions of the name.	|1..n|


## Klasse: Dataset (datasæt) - 
### MANDATORY:
Property|	URI|	Range|	Usage note|	Card |
|---|---|---|---|---|
| description|  dct:description	 |  rdfs:Literal |  This property contains a free-text account of the Dataset. This property can be repeated for parallel language versions of the description.	 |  1..n |   |	
| title	|dct:title	|rdfs:Literal|	This property contains a name given to the Dataset. This property can be repeated for parallel language versions of the name.	|1..n|		
| publisher	|dct:publisher|	foaf:Agent	|This property refers to an entity (organisation) responsible for making the Dataset available.|	0..1|
| data responsible organisation |	dcat-dk: dataResponsible Organisation|	org:FormalOrganisation	|(OBS: Dansk tilføjelse) Dataansvarlig organisation: organisation der er ansvarlig for indsamlingen af data, og som har dispositionsretten og træffer afgørelse om hvordan data skal behandles|0..1|

### RECOMMENDED:
Property|	URI|	Range|	Usage note|	Card |
|---|---|---|---|---|
| conforms to	|dct:conformsTo	|dct:Standard	|This property refers to an implementing rule or other specification.|	0..n|
| documentation	|foaf:page	|foaf:Document|	This property refers to a page or document about this Dataset.|	0..n|
| frequency	|dct:accrualPeriodicity	|dct:Frequency|	This property refers to the frequency at which Dataset is updated|	0..1|
| landing page|	dcat:landingPage|	foaf:Document|	This property refers to a web page that provides access to the Dataset, its Distributions and/or additional information. |	0..1|
| language	|dct:language	|dct:LinguisticSystem	|This property refers to a language of the Dataset. This property can be repeated if there are multiple languages in the Dataset.|	0..n|
| spatial/ geographical coverage|	dct:spatial|	dct:Location|	This property refers to a geographic region that is covered by the Dataset. |	0..n|
| payment imposed|	dcat-dk: payment ImposedContents|	xsd:Boolean	|	(OBS: Dansk tilføjelse) Betalingspålagt: Angiver om der er pålagt en betaling på det pågældende datasæt. |0..1|
| personal data category 	|dcat-dk: personalDataCategory	|skos:Concept	|(OBS: Dansk tilføjelse) Personoplysningskategori: Angiver hvilken type af personoplysninger som datasættet indeholder.|0..n	
| legal ressource |cv:hasLegalResource	|eli:LegalResource|(OBS: Dansk tilføjelse)	Hjemmel: Den hjemmel forankret i lovgivningen som har været gældende for dataindsamlingen.	 |0..n	|
| theme/ category	|dcat:theme, subproperty of dct:subject	|skos:Concept	|This property refers to a category of the Dataset. A Dataset may be associated with multiple themes.	|0..n|			
| public administrative task type|	dcat-dk: publicAdministrative TaskType|	skos:Concept|(OBS: Dansk tilføjelse) Forvaltningsopgave: Angiver en eller flere forvaltningsopgaver jf. FORM som har dannet grundlag for dataindsamlingen|	0..n	|
| FORMversionNumber|	dcat-dk:FORMversionNumber TaskType|	rdfs:Literal|(OBS: Dansk tilføjelse) FORM-versionsnummer: angivelse af den version af klassifikationen FORM som anvendes til angivelse af relaterede forvaltningsopgaver |	0..1	|
|contact point	|dcat:contactPoint	|vcard:Kind	|This property contains contact information that can be used for sending comments about the Dataset.|	0..n|

### OPTIONAL:
Property|	URI|	Range|	Usage note|	Card |
|---|---|---|---|---|
|release date	| dct:issued	| rdfs:Literal  typed as xsd:date or xsd:dateTime|	This property contains the date of formal issuance (e.g., publication) of the Dataset.	|0..1|
|update/ modification date |	dct:modified|	rdfs:Literal typed as xsd:date or xsd:dateTime|	This property contains the most recent date on which the Dataset was changed or modified.	|0..1|
|type|	dct:type|	skos:Concept	|This property refers to the type of the Dataset. A controlled vocabulary for the values has not been established.	|0..1|
|keyword/ tag|	dcat:keyword	|rdfs:Literal	|This property contains a keyword or tag describing the Dataset.|	0..n|
|access rights	|dct:accessRights|	dct:RightsStatement|	This property refers to information that indicates whether the Dataset is open data, has access restrictions or is not public. |0..1|
|creator	|dct:creator|	foaf:Agent|	This property refers to the  entity primarily responsible for producing the dataset	|0..1|
|identifier	|dct:identifier|	rdfs:Literal|	This property contains the main identifier for the Dataset, e.g. the URI or other unique identifier in the context of the Catalogue.	|0..n|
|other identifier	|adms:identifier|	adms:Identifier|	This property refers to a secondary identifier of the Dataset, such as MAST/ADS , DataCite , DOI , EZID  or W3ID .|	0..n|
|related resource|	dct:relation	|rdfs:Resource|	This property refers to a related resource.	|0..n|
|source	|dct:source	|dcat:Dataset|	This property refers to a related Dataset from which the described Dataset is derived.	|0..n|
|provenance	|dct:provenance|	dct:ProvenanceStatement	|This property contains a statement about the lineage of a Dataset.	|0..n|
|qualified attribution |	prov:qualifiedAttribution |	prov:Attribution	|This property refers to a liink to an Agent having some form of responsibility for the resource	|0..n|
|qualified relation|	dcat:qualifiedRelation|	dcat:Relationship|	This property is about a  related resource, such as a publication, that references, cites, or otherwise points to the dataset.	|0..n|
|sample	|adms:sample	|dcat:Distribution	|This property refers to a sample distribution of the dataset	|0..n|
|was generated by|	prov:wasGeneratedBy	|prov:Activity	|This property refers to an activity that generated, or provides the business context for, the creation of the dataset.|	0..n|
|is referenced by	|dct:isReferencedBy|	rdfs:Resource|	This property provides a link to a description of a relationship with another resource	|0..n|
|version|	owl:versionInfo|	rdfs:Literal	|This property contains a version number or other version designation of the Dataset.	|0..1|
|version notes|	adms:versionNotes	|rdfs:Literal	|This property contains a description of the differences between this version and a previous version of the Dataset. This property can be repeated for parallel language versions of the version notes.	|0..n|
|is version of	|dct:isVersionOf|	dcat:Dataset|	This property refers to a related Dataset of which the described Dataset is a version, edition, or adaptation.	|0..n|
|has version	|dct:hasVersion|	dcat:Dataset|	This property refers to a related Dataset that is a version, edition, or adaptation of the described Dataset.	|0..n|
|spatial resolution	|dcat:spatialResolutionInMeters	|	xsd:decimal|	This property refers to the minimum spatial separation resolvable in a dataset, measured in meters.	|0..n|
|temporal resolution	| dcat:temporalResolution	|xsd:duration	|This property refers to the minimum time period resolvable in the dataset.	|0..n|

## Klasse: Distribution (Datasætrepræsentation) 

### MANDATORY:
Property|	URI|	Range|	Usage note|	Card |
|---|---|---|---|---|
| accessURL	|dcat:accessURL	|rdfs:Resource|	A URL of the resource that gives access to a distribution of the dataset. E.g. landing page, feed, SPARQL endpoint.	|1..n|		

### RECOMMENDED:
Property|	URI|	Range|	Usage note|	Card |
|---|---|---|---|---|
| availability	| dcatap:availability	| skos:Concept	| This property indicates how long it is planned to keep the Distribution of the Dataset available. 	| 0..1| 
| description	| dct:description	| rdfs:Literal	| This property contains a free-text account of the Distribution. This property can be repeated for parallel language versions of the description.	| 0..n| 
| format	| dct:format	| dct:MediaTypeOrExtent	| This property refers to the file format of the Distribution.	| 0..1| 
| licence	| dct:license	| dct:LicenseDocument	| This property refers to the licence under which the Distribution is made available.	| 0..1| 

### OPTIONAL:
Property|	URI|	Range|	Usage note|	Card |
|---|---|---|---|---|
| access service 	| dcat:accessService	| dcat:DataService	| This property refers to a data service that gives access to the distribution of the dataset | 	0..n | 
| byte size	| dcat:byteSize		|rdfs:Literal typed as xsd:decimal	| This property contains the size of a Distribution in bytes.	| 0..1| 
| checksum	| spdx:checksum		|spdx:Checksum	| This property provides a mechanism that can be used to verify that the contents of a distribution have not changed. The checksum is related to the downloadURL.	| 0..1| 
| compression format	| dcat:compressFormat	| dct:MediaType	| This property refers to the format of the file in which the data is contained in a compressed form, e.g. to reduce the size of the downloadable file. It SHOULD be expressed using a media type as defined in the official register of media types managed by IANA.	| 0..1| 
| documentation	| foaf:page	| foaf:Document	| This property refers to a page or document about this Distribution.	| 0..n| 
| download URL	| dcat:downloadURL	| rdfs:Resource	| This property contains a URL that is a direct link to a downloadable file in a given format. | 	0..n| 
| has policy	| odrl:hasPolicy	| odrl:Policy	| This property refers to the policy expressing the rights associated with the distribution if using the ODRL vocabulary	| 0..1| 
| language	| dct:language	| dct:LinguisticSystem	| This property refers to a language used in the Distribution. This property can be repeated if the metadata is provided in multiple languages.	| 0..n| 
| linked schemas	| dct:conformsTo	| dct:Standard	| This property refers to an established schema to which the described Distribution conforms.| 	0..n| 
| media type	| dcat:mediaType, subproperty of dct:format	| dct:MediaType	| This property refers to the media type of the Distribution as defined in the official register of media types managed by IANA.	| 0..1| 
| packaging format	| dcat:packageFormat	| dct:MediaType	| This property refers to the format of the file in which one or more data files are grouped together, e.g. to enable a set of related files to be downloaded together. It SHOULD be expressed using a media type as defined in the official register of media types managed by IANA.	| 0..1| 
| release date	| dct:issued	| rdfs:Literal typed as xsd:date or xsd:dateTime	| This property contains the date of formal issuance (e.g., publication) of the Distribution.	| 0..1| 
| rights	| dct:rights| 	dct:RightsStatement	| This property refers to a statement that specifies rights associated with the Distribution.	| 0..1| 
| spatial resolution 	| dcat:spatialResolutionInMeters	| xsd:decimal	| This property refers to the  minimum spatial separation resolvable in a dataset distribution, measured in meters.| 	0..n| 
| status	| adms:status	| skos:Concept	| This property refers to the maturity of the Distribution. It MUST take one of the values Completed, Deprecated, Under Development, Withdrawn. 	| 0..1| 
| temporal resolution	| dcat:temporalResolution | 	xsd:duration| 	This property refers to the minimum time period resolvable in the dataset distribution.	| 0..n| 
| title | 	dct:title	| rdfs:Literal | 	This property contains a name given to the Distribution. This property can be repeated for parallel language versions of the description.	| 0..n| 
| update/ modification date	| dct:modified | 	rdfs:Literal typed as xsd:date or xsd:dateTime	| This property contains the most recent date on which the Distribution was changed or modified.	| 0..1| 

### Namespaces


### Om Shapes Constraint Language (SHACL)
* SHACL-Specifikation: https://www.w3.org/TR/shacl/
* SHACL-Playground: https://shacl.org/playground/ (I denne SHACL-sandkasse kan eksempeldatagrafer automatisk valideres op imod SHACL-anvendelssprofilen -dcat-ap-dk-v1-shapes.ttl)
* RDF converter: http://www.easyrdf.org/converter
* Interoperability Test Bed DCAT-AP validator: https://www.itb.ec.europa.eu/shacl/dcat-ap/upload
