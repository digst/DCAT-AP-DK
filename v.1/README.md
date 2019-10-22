## Anvendelsesprofil: DCAT-AP-DK V.1 (udtrykt med SHACL) - under udvikling

* SHACL-Specifikation: https://www.w3.org/TR/shacl/
* SHACL-Playground: https://shacl.org/playground/
* Interoperability Test Bed: https://joinup.ec.europa.eu/solution/interoperability-test-bed/news/shacl-validator-updates
* RDF converter: http://www.easyrdf.org/converter

Se DCAT-AP-DK (v.1) Shapes Graph samt Example Data Graphs (i RDF-XML, TTL, og JSON-LD) i filerne ovenfor

## UML-diagram for anvendelseprofil
![alt text](https://github.com/digst/DCAT-AP-DK/blob/master/v.1/DCAT-AP-DKv1.png "UML Diagram")


DATASET PROPERTIES:

Property|	URI|	Range|	Usage note|	Card |
|---|---|---|---|---|
| description|  dct:description	 |  rdfs:Literal |  This property contains a free-text account of the Dataset. This property can be repeated for parallel language versions of the description.	 |  1..n |   |	
| title	|dct:title	|rdfs:Literal|	This property contains a name given to the Dataset. This property can be repeated for parallel language versions of the name.	|1..n|		
| publisher	|dct:publisher|	foaf:Agent	|This property refers to an entity (organisation) responsible for making the Dataset available.|	0..1|
| theme/ category	|dcat:theme, subproperty of dct:subject	|skos:Concept	|This property refers to a category of the Dataset. A Dataset may be associated with multiple themes.	|0..n|			
| conforms to	|dct:conformsTo	|dct:Standard	|This property refers to an implementing rule or other specification.|	0..n|
| documentation	|foaf:page	|foaf:Document|	This property refers to a page or document about this Dataset.|	0..n|
| frequency	|dct:accrualPeriodicity	|dct:Frequency|	This property refers to the frequency at which Dataset is updated|.	0..1|
| landing page|	dcat:landingPage|	foaf:Document|	This property refers to a web page that provides access to the Dataset, its Distributions and/or additional information. |	0..1|
| language	|dct:language	|dct:LinguisticSystem	|This property refers to a language of the Dataset. This property can be repeated if there are multiple languages in the Dataset.|	0..n|
| spatial/ geographical coverage|	dct:spatial|	dct:Location|	This property refers to a geographic region that is covered by the Dataset. |	0..n|
| data responsible organisation |	dcat-dk:dataResponsibleOrganisation|	dcat-dk:DataResponsibleOrganisation	|Dataansvarlig organisation: organisation der er ansvarlig for indsamlingen af data, og som har dispositionsretten og træffer afgørelse om hvordan data skal behandles|0..1|
| payment imposed|	dcat-dk:paymentImposedContents|	xsd:Boolean	|	Betalingspålagt: Angiver om der er pålagt en betaling på det pågældende datasæt. |0..1|
public administrative task type|	dcat-dk:publicAdministrativeTaskType|	skos:Concept|Forvaltningsopgave: Angiver en eller flere forvaltningsopgaver jf. FORM som har dannet grundlag for dataindsamlingen|	0..n	|
| personal data category 	|dcat-dk:personalDataCategory	|skos:Concept	|Personoplysningskategori: Angiver hvilken type af personoplysninger som datasættet indeholder.|0..n	
| legal ressource |cv:hasLegalResource	|eli:LegalResource|	Hjemmel: Den hjemmel forankret i lovgivningen som har været gældende for dataindsamlingen.	 |0..n	|
