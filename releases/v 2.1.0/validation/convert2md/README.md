# RDFXML2MD-instructions:



- Åbn SHACL-masterfilen (RDF/XML-serialiseringen). https://github.com/digst/DCAT-AP-DK/blob/master/releases/v.2.0/validation/DRAFT_dcat-ap-dk_2.0.0_shacl_shapes.xml



- Indfør ændringer

  - rdfs:comment er til vokabulardefinitioner 

  - sh:description er til de kontekstspecifikke anvendelsesnoter 

  - sh:name er til kontekstspecifikke betegnelser

  - sh:targetClass er klassens uri

  - sh:path er egenskabens uri

  - sh:nodeKind er range for egenskaber

  - sh:minCount/maxCount er input til multipliciteten



-  konverter med xslt-stylesheet: Markdown-styling af udkast til SHACL shapes fil: https://data.gov.dk/model/profile/draft/dcat-ap-dk_2.0.0_shacl_shapes.xml
