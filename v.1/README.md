# Anvendelsesprofil: DCAT-AP-DK v.1.1.0 (Under udvikling)
DCAT-AP-DK er en anvendelsesprofil til beskrivelse af datasæt i det fællesoffentlige datasætkatalog.

DCAT-AP-DK er baseret på DCAT-AP som er EU-Kommissionens specifikation for datasætkataloger der har til formål at standardisere og etablere sammenhæng mellem dataportaler i medlemslandene. DCAT-AP-DK v.1.1 anvender elementer fra og er i overenstemmelse med DCAT-AP v. 1.1, men tilføjer også enkelte elementer for at opfylde behovet i en dansk administrativ kontekst


Anvendelsesprofilen er visualiseret med UML og udtrykt med SHACL 
(SHACL-shapes og dataeksempler mangler pt. opdatering da distribution fx mangler). 

## Anvendelseprofil visualiseret med UML-diagram
![alt text](https://github.com/digst/DCAT-AP-DK/blob/master/v.1/DCAT-AP-DKv1.png "UML Diagram")
Bemærk at modelleringen af relationen til kontrollerede udfaldsrum (EU-kodelisterne m.fl) vil blive revideret.

EU-kodelisterne for fx frequency og language kan findes her: https://publications.europa.eu/en/web/eu-vocabularies/authority-tables

* DCAT Application Profile for Data Portals in Europe - Final 1.1: 
https://joinup.ec.europa.eu/solution/dcat-application-profile-data-portals-europe/release/11
* DOCX-fil med specifikation: https://github.com/SEMICeu/DCAT-AP/raw/master/releases/1.1/dcat-ap_1.1.docx
+ enkelte danske tilføjelser (se nederst)


## Klasse:Dataset (datasæt) - MANDATORY:
Property|	URI|	Range|	Usage note|	Card |
|---|---|---|---|---|
| description|  dct:description	 |  rdfs:Literal |  This property contains a free-text account of the Dataset. This property can be repeated for parallel language versions of the description.	 |  1..n |   |	
| title	|dct:title	|rdfs:Literal|	This property contains a name given to the Dataset. This property can be repeated for parallel language versions of the name.	|1..n|		
| publisher	|dct:publisher|	foaf:Agent	|This property refers to an entity (organisation) responsible for making the Dataset available.|	0..1|
| theme/ category	|dcat:theme, subproperty of dct:subject	|skos:Concept	|This property refers to a category of the Dataset. A Dataset may be associated with multiple themes.	|0..n|			
| conforms to	|dct:conformsTo	|dct:Standard	|This property refers to an implementing rule or other specification.|	0..n|
| documentation	|foaf:page	|foaf:Document|	This property refers to a page or document about this Dataset.|	0..n|
| frequency	|dct:accrualPeriodicity	|dct:Frequency|	This property refers to the frequency at which Dataset is updated|	0..1|
| landing page|	dcat:landingPage|	foaf:Document|	This property refers to a web page that provides access to the Dataset, its Distributions and/or additional information. |	0..1|
| language	|dct:language	|dct:LinguisticSystem	|This property refers to a language of the Dataset. This property can be repeated if there are multiple languages in the Dataset.|	0..n|
| spatial/ geographical coverage|	dct:spatial|	dct:Location|	This property refers to a geographic region that is covered by the Dataset. |	0..n|
| data responsible organisation |	dcat-dk: dataResponsible Organisation|	org:FormalOrganisation	|(OBS: Dansk tilføjelse) Dataansvarlig organisation: organisation der er ansvarlig for indsamlingen af data, og som har dispositionsretten og træffer afgørelse om hvordan data skal behandles|0..1|
| payment imposed|	dcat-dk: payment ImposedContents|	xsd:Boolean	|	(OBS: Dansk tilføjelse) Betalingspålagt: Angiver om der er pålagt en betaling på det pågældende datasæt. |0..1|
public administrative task type|	dcat-dk: publicAdministrative TaskType|	skos:Concept|(OBS: Dansk tilføjelse) Forvaltningsopgave: Angiver en eller flere forvaltningsopgaver jf. FORM som har dannet grundlag for dataindsamlingen|	0..n	|
| personal data category 	|dcat-dk: personalDataCategory	|skos:Concept	|(OBS: Dansk tilføjelse) Personoplysningskategori: Angiver hvilken type af personoplysninger som datasættet indeholder.|0..n	
| legal ressource |cv:hasLegalResource	|eli:LegalResource|(OBS: Dansk tilføjelse)	Hjemmel: Den hjemmel forankret i lovgivningen som har været gældende for dataindsamlingen.	 |0..n	|


## Klasse:Distribution (Datasætrepræsentation) - RECCOMMENDED:
Property|	URI|	Range|	Usage note|	Card |
|---|---|---|---|---|
| accessURL	|dcat:accessURL	|rdfs:Resource|	A URL of the resource that gives access to a distribution of the dataset. E.g. landing page, feed, SPARQL endpoint.	|1..n|		
| description|  dct:description	 |  rdfs:Literal |  This property contains a free-text account of the Distribution. This property can be repeated for parallel language versions of the description.	 |  0..n |   |	
| title	|dct:title	|rdfs:Literal|	This property contains a name given to the Distribution. This property can be repeated for parallel language versions of the name.	|0..n|		
| byte size|dcat:byteSize|xsd:decimal|This property contains the size of a Distribution in bytes.|0..1|
| format |dct:format|dct:MediaTypeOrExtent|This property refers to the media type of the Distribution as defined in the official register of media types managed by IANA|0..1|
| licence|dct:license|dct:LicenseDocument|This property refers to the licence under which the Distribution is made available. |0..1|
| language	|dct:language	|dct:LinguisticSystem	|This property refers to a language of the Distribution. This property can be repeated if there are multiple languages in the Dataset.|	0..n|




## Om Shapes Constraint Language (SHACL)

* SHACL-Specifikation: https://www.w3.org/TR/shacl/
* SHACL-Playground: https://shacl.org/playground/ 
(I denne SHACL-sandkasse kan eksempeldatagrafer automatisk valideres op imod SHACL-anvendelssprofilen -dcat-ap-dk-v1-shapes.ttl) 
* RDF converter: http://www.easyrdf.org/converter

Se DCAT-AP-DK (v.1) Shapes Graph samt Example Data Graphs (i RDF-XML, TTL, og JSON-LD) i filerne ovenfor

Se evt. også: Interoperability Test Bed: https://joinup.ec.europa.eu/solution/interoperability-test-bed/news/shacl-validator-updates
