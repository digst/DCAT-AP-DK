# Indlejring af eksisterende DCAT-metadata med RDFa

DCAT-metadata kan indlejres i eksisterende opmærkning vha. JSON-LD eller RFDa. 

RDFa er en W3C-anbefaling der tilføjer et sæt attributniveauudvidelser til HTML, XHTML og forskellige XML-baserede dokumenttyper til indlejring af metadata i webdokumenter.

## Læs mere om RDFa:
- W3C RDFa 1.1 Primer: https://www.w3.org/TR/rdfa-primer/ 
- W3C RFDa Core 1.1 specifikationen:  https://www.w3.org/TR/rdfa-core/ 
- Wikipedia om RDFa: https://en.wikipedia.org/wiki/RDFa
- Praktiske vejledninger til DCAT-opmærkning med RDFa på følgende websider: 
  - https://theodi.org/article/marking-up-your-dataset-with-dcat/
  - https://developers.google.com/search/docs/data-types/dataset

## Og se et par eksempler her:
- RDFa example 1 uri= https://data.gov.dk/test/rdfa/RDFa1_basic-example1.html
- RDFa example 2 uri= https://data.gov.dk/test/rdfa/RDFa2_basic-example1.html

Med fx [W3Cs RDF distiller](https://www.w3.org/2012/pyRdfa/Overview.html) kan  DCAT-metadata udtrækkes fra ovenstående eksempel-html-filer:

Mini-guide (på engelsk) til direkte brug af RDF distiller:
- Extract the RDF with whitespace preservation and without warnings, serialized in Turtle:
http://www.w3.org/2012/pyRdfa/extract?uri=https://data.gov.dk/test/rdfa/RDFa2_basic-example1.html
- Extract the RDF with whitespace preservation and without warnings, serialized in RDF/XML:
http://www.w3.org/2012/pyRdfa/extract?format=xml&uri=https://data.gov.dk/test/rdfa/RDFa2_basic-example1.html
- Extract the RDF from  with whitespace preservation and including warnings, serialized in Turtle:
http://www.w3.org/2012/pyRdfa/extract?graph=default,processor&uri=https://data.gov.dk/test/rdfa/RDFa2_basic-example1.html
- Use a fixed, pseudo URI to extract the RDF from the current page without specifying its URI (with default options); this can be used, say, as a link for a button on the page: http://www.w3.org/2012/pyRdfa/extract?uri=referer


