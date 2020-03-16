I ovenstående TTL-fil har vi indsat forslag til danske oversættelser af DCAT-elementerne:

Da oversættelser optræder sammen med mange andre oversættelser har vi herunder lavet et udtræk af de danske oversættelser fra.  
Følgende egenskaber er blevet oversat rdfs:label, rdfs:comment (kopi i skos:definition) samt skos:scopeNote og skos:editorialNote)

================================
Search "@da" (144 hits in 1 file)

	Line 122:   rdfs:comment "DCAT er et RDF-vokabular som har til formål at understøtte interoperabilitet mellem datakataloger udgivet på nettet. Ved at anvende DCAT til at beskrive datasæt i datakataloger, kan udgivere optimere synlighed og gøre det gøre det lettere for applikationer at anvende metadata fra forskellige kataloger. Derudover understøttes decentraliseret udstilling af kataloger og fødererede datasætsøgninger på tværs af websider. Aggregerede DCAT-metadata kan fungere som fortegnelsesfiler der kan understøtte digital bevaring. "@da ;  
  
  
	Line 131:   rdfs:label "Vokabular for datakataloger"@da ;
	Line 156:   rdfs:comment "En organiseret samling af metadata om ressourcer (fx. datasæt og dataservices i kontekst af et datakatalog). "@da ;   
	Line 166:   rdfs:label "Katalog"@da ;  
	Line 181:   skos:definition "En organiseret samling af metadata om ressourcer (fx. datasæt og dataservices i kontekst af et datakatalog)."@da ;       
  
	Line 201:   rdfs:comment "En optegnelse i et datakatalog der beskriver registreringen af et enkelt datasæt eller en dataservice."@da ;   
	Line 210:   rdfs:label "Katalogoptegnelse"@da ;  
	Line 229:   skos:definition "En optegnelse i et datakatalog der beskriver registreringen af et enkelt datasæt eller en dataservice."@da ;       
	Line 238:   skos:scopeNote "Denne klasse er valgfri og ikke alle kataloger vil anvende denne klasse. Den kan anvendes i de kataloger for der skelnes mellem metadata om datasættet eller dataservicen og metadata om selve optegnelsen af datasættet eller dataservicen i kataloget. Udgivelsesdatoen for datasættet afspejler for eksempel den data hvor informationerne oprindeligt blev gjort tilgængelige af udgiveren, hvorimod udgivelsesdatoen for katalogoptegnelsen er den dato hvor datasættet blev føjet til kataloget. I de tilfælde hvor de to datoer er forskellige eller hvor blot sidstnævnte er kendt, bør udgivelsesdatoen kun angives for katalogoptegnelsen. Bemærk at W3Cs PROV ontologi gør til muligt at tilføje yderligere proveniensoplysninger for eksempelvis hvilken proces eller aktør der er involveret i en given ændring af datasættet."@da; 
  
	Line 249:   rdfs:comment "Et site eller endpoint der giver operationer relateret til opdagelse af, adgang til eller behandlende funktioner på data eller relaterede ressourcer."@da ;   
	Line 254:   rdfs:label "Dataservice"@da ;  
	Line 265:   skos:changeNote "Ny klasse tilføjet i DCAT 2.0."@da ;    
	Line 270:   skos:definition "Et site eller endpoint der giver operationer relateret til opdagelse af, adgang til eller behandlende funktioner på data eller relaterede ressourcer."@da ;    
  
	Line 288:   rdfs:comment "En samling a data, udgivet eller organiseret af en enkelt kilde og som der er adgang til i en eller flere repræsentationer."@da ;    
	Line 298:   rdfs:label "Datasæt"@da ;  
	Line 308:   skos:changeNote "2018-02 - subklasse af dctype:Dataset fjernet da scope af dcat:Dataset omfatter flere forskellige typer fra dctype-vokabularet."@da ;  
	Line 314:   skos:definition "En samling a data, udgivet eller organiseret af en enkelt kilde og som der er adgang til i en eller flere repræsentationer."@da ;    
  
	Line 335:   rdfs:comment "En specifik repræsentation af et datasæt. Et datasæt kan være tilgængelig i mange serialiseringer der kan variere på forskellige vis, herunder sprog, medietype eller format, systemorganisering, tidslig- og rumlig opløsning, detaljeringsniveau eller profiler (der kan specificere en eller flere af ovenstående)"@da ;   
	Line 345:   rdfs:label "Datasætrepræsentation"@da ;  
	Line 354:   skos:definition "En specifik repræsentation af et datasæt. Et datasæt kan være tilgængelig i mange serialiseringer der kan variere på forskellige vis, herunder sprog, medietype eller format, systemorganisering, tidslig- og rumlig opløsning, detaljeringsniveau eller profiler (der kan specificere en eller flere af ovenstående)"@da ;   
	Line 363:   skos:scopeNote "Denne klasse repræsenterer datasættets overordnede tilgængelighed og giver ikke oplysninger om hvilken metode der kan anvendes til at få adgang til data, dvs. om adgang til datasættet realises ved direkte download, API eller via en webside. Anvendelsen af egenskaben dcat:downloadURL indikerer at distributionen kan downloades direkte."@da ;   
  
	Line 374:   rdfs:comment "En associationsklasse til brug for tilknytning af yderligere information til en relation mellem DCAT-ressourcer."@da ;     
	Line 379:   rdfs:label "Relation"@da ;  
	Line 389:   skos:changeNote "Ny klasse i DCAT 2.0."@da ;    
	Line 394:   skos:definition "En associationsklasse til brug for tilknytning af yderligere information til en relation mellem DCAT-ressourcer."@da ;    
	Line 399:   skos:scopeNote "Anvendes til at karakterisere en relation mellem datasæt, og potentielt andre ressourcer, hvor relationen er kendt men ikke tilstrækkeligt beskrevet af de standardiserede egenskaberi Dublin Core (dct:hasPart, dct:isPartOf, dct:conformsTo, dct:isFormatOf, dct:hasFormat, dct:isVersionOf, dct:hasVersion, dct:replaces, dct:isReplacedBy, dct:references, dct:isReferencedBy, dct:requires, dct:isRequiredBy) or PROV-O properties (prov:wasDerivedFrom, prov:wasInfluencedBy, prov:wasQuotedFrom, prov:wasRevisionOf, prov:hadPrimarySource, prov:alternateOf, prov:specializationOf)."@da ;  
  
	Line 407:   rdfs:comment "Ressource udgivet eller organiseret af en enkelt aktør."@da ;     
	Line 412:   rdfs:label "Katalogressource"@da ;  
	Line 417:   skos:changeNote "Ny klasse i DCAT 2.0."@da ;  
	Line 422:   skos:definition "Ressource udgivet eller organiseret af en enkelt aktør."@da ;    
	Line 427:   skos:scopeNote "Klassen for alle katalogiserede ressourcer, den overordnede klasse for dcat:Dataset, dcat:DataService, dcat:Catalog og enhvert medlem af et dcat:Catalog. Denne klasse bærer egenskaber der gælder alle katalogiserede ressourcer, herunder datset og dataservices. Det anbefales kraftigt at mere specifikke subklasser oprettes. Når der beskrives ressourcer der ikke er dcat:Dataset eller dcat:DataService, anbefales det at oprette passende subklasser af dcat:Resource eller at dcat:Resource anvendes sammen med egenskaben dct:type til opmærkning med en specifik typeangivelse."@da ;   
  
	Line 439:   rdfs:comment "En rolle er den funktion en ressource eller aktør har i forhold til en anden ressource, i forbindelse med ressourcetildeling eller ressourcerelationer."@da ;     
	Line 444:   rdfs:label "Rolle"@da ;  
	Line 456:   skos:definition "En rolle er den funktion en ressource eller aktør har i forhold til en anden ressource, i forbindelse med ressourcetilskrivning eller ressourcerelationer."@da ;    
	Line 461:   skos:editorialNote "Introduceret i DCAT for at komplementere prov:Role (hvis anvendelse er begrænset til roller i forbindelse med en aktivitet, som er rækkevidde for prov:hadRole)."@da ;  
	Line 466:   skos:scopeNote "Anvendes i forbindelse med præciserede tilskrivninger til at angive aktørens rolle i forhold til en entitet. Det anbefales at værdierne styres som en klassifikation af aktørroller, såsom http://registry.it.csiro.au/def/isotc211/CI_RoleCode."@da ;  
  
	Line 478:   rdfs:comment "En side eller endpoint der giver adgang til en distribution af datasættet."@da ;     
	Line 483:   rdfs:label "dataadgangsservice"@da ;  
	Line 489:   skos:changeNote "Ny egenskab tilføjet i DCAT 2.0."@da ;  
  
	Line 502:   rdfs:comment "En URL for en ressource som giver adgang til en repræsentation af datsættet. Fx, landing page, feed, SPARQL-endpoint. Anvendes i alle sammenhænge undtagen til angivelse af et simpelt download link hvor anvendelse af egenskaben downloadURL foretrækkes. "@da ;     
	Line 513:   rdfs:label "andgangsURL"@da ;  
	Line 527:   skos:definition "En URL for en ressource som giver adgang til en repræsentation af datsættet. Fx, landing page, feed, SPARQL-endpoint. Anvendes i alle sammenhænge undtagen til angivelse af et simpelt download link hvor anvendelse af egenskaben downloadURL foretrækkes. "@da ;        
	Line 538:   skos:scopeNote "Hvis en eller flere datasætrepræsentationer kun er tilgængelige via en landing page (dvs. en URL til direkte download er ikke kendt), så bør landing page linket gentages som adgangsURL for datasætrepræsentationen."@da ;  
  
	Line 551:   rdfs:label "bounding box"@da ;  
	Line 557:   skos:changeNote "Ny egenskab tilføjet i DCAT 2.0."@da ;  
	Line 569:   skos:scopeNote "Rækkevidden for denne egenskab er bevidst generisk definere med det formål at tillade forskellige geokodninger. Geometrien kan eksempelvis repræsenteres som WKT (geosparql:asWKT [GeoSPARQL]) eller [GML] (geosparql:asGML [GeoSPARQL])."@da ;  
  
	Line 576:   rdfs:comment "Størrelsen af en datasætrepræsentationen angivet i bytes."@da ;     
	Line 587:   rdfs:label "bytestørrelse"@da ;  
	Line 597:   skos:definition "Størrelsen af en datasætrepræsentationen angivet i bytes."@da ;     
	Line 606:   skos:scopeNote "Bytestørrelsen kan approximeres hvis den præcise størrelse ikke er kendt. Værdien af dcat:byteSize bør angives som xsd:decimal."@da ;  
  
	Line 618:   rdfs:comment "Et katalog hvis indhold er relevant i forhold til det aktuelle katalog."@da ;     
	Line 624:   rdfs:label "katalog"@da ;  
	Line 636:   skos:definition "Et katalog hvis indhold er relevant i forhold til det aktuelle katalog."@da ; 
  
	Line 646:   rdfs:label "geometrisk tyngdepunkt"@da ;  
	Line 652:   skos:changeNote "Ny egenskab tilføjet i DCAT 2.0."@da ;  
	Line 657:   skos:definition "Det geometrisk tyngdepunkt (centroid) for en ressource."@da ;  
	Line 662:   skos:scopeNote "Rækkevidden for denne egenskab er bevidst generisk definere med det formål at tillade forskellige geokodninger. Geometrien kan eksempelvis repræsenteres som WKT (geosparql:asWKT [GeoSPARQL]) eller [GML] (geosparql:asGML [GeoSPARQL])."@da ; 
  
	Line 671:   rdfs:comment "Kompressionsformatet for datasætrepræsentationen som indeholder data i et komprimeret format, fx. for at reducere størrelsen af downloadfilen, "@da ;     
	Line 678:   rdfs:label "kompressionsformat"@da ;  
	Line 685:   skos:changeNote "Ny egenskab tilføjet i DCAT 2.0."@da ;  
	Line 690:   skos:definition "Kompressionsformatet for datasætrepræsentationen som indeholder data i et komprimeret format, fx. for at reducere størrelsen af downloadfilen, "@da ;  
	Line 695:   skos:scopeNote "Denne egenskab kan anvendes når filerne i en datasætrepræsentation er blevet komprimeret, fx i en ZIP-fil. Formatet BØR udtrykkes ved en medietype som defineret i 'IANA media types registry', hvis der optræder en relevant medietype dér: https://www.iana.org/assignments/media-types/."@da ;  
  
	Line 704:   rdfs:comment "Relevante kontaktoplysinger for katalogressourcen. Anvendelse af vCard anbefales."@da ;     
	Line 714:   rdfs:label "kontaktpunkt"@da ;  
	Line 724:   skos:definition "Relevante kontaktoplysinger for katalogressourcen. Anvendelse af vCard anbefales."@da ;  
  
	Line 738:   rdfs:comment "En samling af data som er en del af kataloget."@da ;     
	Line 749:   rdfs:label "datasæt"@da ;  
	Line 761:   skos:definition "En samling af data som er en del af kataloget."@da ;   
  
	Line 775:   rdfs:comment "En tilgængelig repræsentation af datsættet."@da ;     
	Line 786:   rdfs:label "datasætrepræsentaiton"@da ;  
	Line 797:   skos:definition "En tilgængelig repræsentation af datsættet."@da ;   
  
	Line 811:   rdfs:comment "URL til fil der kan downloades i et bestemt format. Fx en CSV-fil eller en RDF-fil. Formatet for datasætrepræsentaionen angives ved hjælp af egenskaberne dct:format og/eller dcat:mediaType."@da ;  
	Line 822:   rdfs:label "download-URL"@da ;  
	Line 832:   skos:definition "URL til fil der kan downloades i et bestemt format. Fx en CSV-fil eller en RDF-fil. Formatet for datasætrepræsentaionen angives ved hjælp af egenskaberne dct:format og/eller dcat:mediaType."@da ;    
	Line 843:   skos:scopeNote "dcat:downloadURL BØR bør anvendes til angivelse af den adresse hvor datasætrepræsentaionen er tilgængelig direkte, typisk gennem et HTTP Get request."@da ;  
  
	Line 855:   rdfs:label "slutdato"@da ;  
	Line 861:   skos:changeNote "Ny egenskab i DCAT 2.0."@da ;  
  
	Line 866:   skos:definition "Periodens slutdao."@da ;   
	Line 871:   skos:scopeNote "Rækkeviden for denne egenskab er bevidst generisk defineret med det formål at tillade forskellige niveauer af tidslig præcision ifm. angivelse af slutdatoen for en periode. Den kan eksempelvis udtrykkes som en dato(xsd:date), en dato og et tidspunkt (xsd:dateTime), eller et årstal (xsd:gYear)."@da ;  
  
	Line 879:   rdfs:comment "En beskrivelse af det pågældende serviceendpoint, inklusiv dets operationer, parametre etc."@da ;     
	Line 885:   rdfs:label "endpointbeskrivelse"@da ;  
	Line 890:   skos:changeNote "Ny egenskab i DCAT 2.0."@da ;  
	Line 895:   skos:definition "En beskrivelse af det pågældende serviceendpoint, inklusiv dets operationer, parametre etc."@da ;    
	Line 900:   skos:scopeNote "En beskrivelse af et endpoint kan udtrykkes i et maskinlæsbart format, såsom OpenAPI (Swagger)-beskrivelser, et OGC GetCapabilities svar, en SPARQL servicebeskrivelse, en OpenSearch- eller et WSDL-dokument, en Hydra-API-beskrivelse, eller i tekstformat eller i et andet uformelt format, hvis en formel repræsentation ikke er mulig."@da ;  
  
	Line 912:   rdfs:comment "Rodplaceringen eller det primære endpoint for en service (en web-resolverbar IRI)"@da ;     
	Line 918:   rdfs:label "serviceendpoint"@da ;  
	Line 929:   skos:definition "Rodplaceringen eller det primære endpoint for en service (en web-resolverbar IRI)"@da ;   
  
	Line 937:   rdfs:comment "Den funktion en entitet eller aktør har i forhold til en anden ressource."@da ;     
	Line 949:   rdfs:label "havde rolle"@da ;   
	Line 960:   skos:definition "Den funktion en entitet eller aktør har i forhold til en anden ressource."@da ;   
	Line 965:   skos:editorialNote "Introduceret i DCAT for at komplementere prov:hadRole (hvis anvendelse er begrænset til roller i forbindelse med en aktivitet med domænet prov:Association)."@da ;   
	Line 970:   skos:scopeNote "Kan vendes ved præciserede tilskrivninger til at angive en aktørs rolle i forhold en entitet. Det anbefales at værdierne styres som en klassifikation af aktørroller, såsom http://registry.it.csiro.au/def/isotc211/CI_RoleCode."@da ;
  
	Line 983:   rdfs:comment "Et nøgleord eller tag til beskrivelse af en ressource"@da ;     
	Line 993:   rdfs:label "nøgleord"@da ;  
	Line 1004:   skos:definition "Et nøgleord eller tag til beskrivelse af en ressource"@da ;    
  
	Line 1017:   rdfs:comment "En webside som en webbrowser kan navigeres til for at få adgang til kataloget, et datasæt, dets datasætrepræsentaitoner og/eller yderligere information "@da ;   
	Line 1027:   rdfs:label "landing page"@da ;  
	Line 1038:   skos:definition "En webside som en webbrowser kan navigeres til for at få adgang til kataloget, et datasæt, dets datasætrepræsentaitoner og/eller yderligere information "@da ;   
	Line 1047:   skos:scopeNote "Hvis en eller flere datasætrepræsentationer kun er tilgængelige via en landing page (dvs. en URL til direkte download er ikke kendt), så bør landing page linket gentages som adgangsURL for datsætrepræsentationen."@da ;    
  
	Line 1059:   rdfs:comment "Medietypen for datasætrepræsentationen som den er defineret af IANA"@da ;     
	Line 1070:   rdfs:label "medietype"@da ;  
	Line 1085:   skos:definition "Medietypen for datasætrepræsentationen som den er defineret af IANA"@da ;    
	Line 1095:   skos:scopeNote "Denne egenskab BØR anvendes hvis datasætrepræsentationens medietype optræder i 'IANA media types registry' https://www.iana.org/assignments/media-types/, ellers KAN egenskaben dct:format anvendes med et andet udfaldsrum."@da ;   
  
	Line 1104:   rdfs:comment "Pakkeformatet for en datasætrepræsentation hvor en eller flere datafiler er grupperet, fx. med det formål at gøre det muligt at downloade en samling af relaterede filer på én gang."@da ;     
	Line 1111:   rdfs:label "pakkeformat"@da ;  
	Line 1118:   skos:changeNote "Ny egenskab tilføjet i DCAT 2.0."@da ;  
	Line 1127:   skos:scopeNote "Denne egenskab kan anvendes hvis filerne i en distribution er pakket, fx. i en TAR-fil, en Frictionless Data Package eller en Bagit-fil. Formatet BØR udtrykkes ved en medietype som defineret i 'IANA media types registry', hvis der optræder en relevant medietype dér: https://www.iana.org/assignments/media-types/."@da ;   
  
	Line 1135:   rdfs:comment "Reference til en beskrivelse af en relation med en anden ressource."@da ;     
	Line 1141:   rdfs:label "Præciseret relation"@da ;  
	Line 1147:   skos:changeNote "Ny egenskab tilføjet i DCAT 2.0."@da ;  
	Line 1156:   skos:editorialNote "Introduceret i DCAT med henblik på at komplementere de øvrige præciserede relationer fra PROV. "@da ;  
	Line 1161:   skos:scopeNote "Anvendes til at referere til en anden ressource hvor relationens betydning er kendt men ikke matcher en af de standardiserede egenskaber fra Dublin Core (dct:hasPart, dct:isPartOf, dct:conformsTo, dct:isFormatOf, dct:hasFormat, dct:isVersionOf, dct:hasVersion, dct:replaces, dct:isReplacedBy, dct:references, dct:isReferencedBy, dct:requires, dct:isRequiredBy) or PROV-O properties (prov:wasDerivedFrom, prov:wasInfluencedBy, prov:wasQuotedFrom, prov:wasRevisionOf, prov:hadPrimarySource, prov:alternateOf, prov:specializationOf)."@da ;     
  
	Line 1170:   rdfs:comment "En optegnelse der beskriver registreringen af et enkelt datasæt eller en dataservice som er en del af kataloget."@da ;     
	Line 1182:   rdfs:label "optegnelse"@da ;  
	Line 1192:   skos:definition "En optegnelse der beskriver registreringen af et enkelt datasæt eller en dataservice som er en del af kataloget."@da ;  
  
	Line 1206:   rdfs:comment "En samling af data som denne dataservice kan levere."@da ;     
	Line 1212:   rdfs:label "leverer datasæt"@da ;  
	Line 1223:   skos:definition "En samling af data som denne dataservice kan levere."@da ;  
  
	Line 1231:   rdfs:comment "En side eller et endpoint som er en del af kataloget."@da ;     
	Line 1237:   rdfs:label "service"@da ;  
	Line 1250:   skos:definition "En side eller et endpoint som er en del af kataloget."@da ;    
  
	Line 1258:   rdfs:comment "mindste rumlige afstand som kan resolveres i et datasæt, målt i meter."@da ;     
	Line 1264:   rdfs:label "rumlig opløsning (meter)"@da ;  
	Line 1271:   skos:changeNote "Ny genskab tilføjet i DCAT 2.0."@da ;  
	Line 1276:   skos:definition "mindste rumlige afstand som kan resolveres i et datasæt, målt i meter.."@da ;   
	Line 1282:   skos:editorialNote "Kan optræde i forbindelse med beskrivelse af datasættet eller datasætditributionen, så der er ikke angivet et domæne for egenskaben."@da ;  
	Line 1285:   skos:scopeNote "Alternative rumlige opløsninger kan leveres som forskellige datasætdistributioner."@da ;  
	Line 1286:   skos:scopeNote "Hvis datasættet udgøres af et billede eller et grid, så bør dette svare til afstanden mellem elementerne. For andre typer af spatiale datasæt, vil denne egenskab typisk indikere den mindste afstand mellem elementerne i datasættet."@da ; 
  
	Line 1300:   rdfs:label "startdato"@da ;  
	Line 1305:   skos:changeNote "Ny egenskab tilføjet i DCAT 2.0."@da ;  
	Line 1315:   skos:scopeNote "Rækkeviden for denne egenskab er bevidst generisk defineret med det formål at tillade forskellige niveauer af tidslig præcision ifm. angivelse af startdatoen for en periode. Den kan eksempelvis udtrykkes som en dato(xsd:date), en dato og et tidspunkt (xsd:dateTime), eller et årstal (xsd:gYear)."@da ;    
  
	Line 1323:   rdfs:comment "mindste tidsperiode der kan resolveres i datasættet."@da ;     
	Line 1328:   rdfs:label "tidslig opløsning"@da ;  
	Line 1339:   skos:definition "mindste tidsperiode der kan resolveres i datasættet."@da ;    
	Line 1344:   skos:editorialNote "Kan optræde i forbindelse med beskrivelse af datasættet eller datasætditributionen, så der er ikke angivet et domæne for egenskaben."@da ;    
	Line 1347:   skos:scopeNote "Alternative tidslige opløsninger kan leveres som forskellige datasætdistributioner."@da ;   
  
	Line 1360:   rdfs:comment "Et centralt emne for ressourcen. En ressource kan have flere centrale emner."@da ;     
	Line 1370:   rdfs:label "emne"@da ;  
	Line 1381:   skos:definition "Et centralt emne for ressourcen. En ressource kan have flere centrale emner."@da ;      
	Line 1391:   skos:scopeNote "Samlingen af begreber (skos:Concept) der anvendes til at klassificere ressourcer organiseres i et begrebssystem (skos:ConceptScheme) som beskriver alle emnerne og deres relationer i kataloget"@da ;  
  
	Line 1406:   rdfs:comment "Vidensorganiseringssystem (KOS) som anvendes til at klassificere datasæt i kataloget"@da ;     
	Line 1417:   rdfs:label "emnetaksonomi"@da ;  
	Line 1427:   skos:definition"Vidensorganiseringssystem (KOS) som anvendes til at klassificere datasæt i kataloget"@da ;   
	Line 1436:   skos:scopeNote "Det anbefales at taksonomien organiseres i et skos:ConceptScheme, skos:Collection, owl:Ontology eller lignende, som giver mulighed for at ethvert medlem af taksonomien kan forsynes med en IRI og udgives som linked-data."@da ;  
