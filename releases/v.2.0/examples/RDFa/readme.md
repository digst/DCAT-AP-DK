# Indlejring af eksisterende DCAT-metadata med RDFa

DCAT-metadata kan indlejres i eksisterende opmærkning vha. JSON-LD eller RFDa. 

RDFa er en W3C-anbefaling der tilføjer et sæt attributniveauudvidelser til HTML, XHTML og forskellige XML-baserede dokumenttyper til indlejring af metadata i webdokumenter, https://en.wikipedia.org/wiki/RDFa

Læs mere om RFDa i disse vejledninger: 

- https://theodi.org/article/marking-up-your-dataset-with-dcat/
- https://developers.google.com/search/docs/data-types/dataset

Og se et eksempel her:
https://data.gov.dk/test/rdfa/RDFa2_basic-example1.html

Med fx [W3Cs RDF distiller](https://www.w3.org/2012/pyRdfa/Overview.html) kan  DCAT-metadata udtrækkes fra denne eksempel-html-fil:
- RDFa example 1 uri= https://data.gov.dk/test/rdfa/RDFa1_basic-example1.html
- RDFa example 2 uri= https://data.gov.dk/test/rdfa/RDFa2_basic-example1.html

Mini-guide på engelsk til direkte brug af RDF distiller:
- Extract the RDF with whitespace preservation and without warnings, serialized in Turtle:
http://www.w3.org/2012/pyRdfa/extract?uri=https://data.gov.dk/test/rdfa/RDFa2_basic-example1.html
- Extract the RDF with whitespace preservation and without warnings, serialized in RDF/XML:
http://www.w3.org/2012/pyRdfa/extract?format=xml&uri=https://data.gov.dk/test/rdfa/RDFa2_basic-example1.html
- Extract the RDF from  with whitespace preservation and including warnings, serialized in Turtle:
http://www.w3.org/2012/pyRdfa/extract?graph=default,processor&uri=https://data.gov.dk/test/rdfa/RDFa2_basic-example1.html
- Use a fixed, pseudo URI to extract the RDF from the current page without specifying its URI (with default options); this can be used, say, as a link for a button on the page: http://www.w3.org/2012/pyRdfa/extract?uri=referer


