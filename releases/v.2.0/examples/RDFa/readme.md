# Indlejring af DCAT-metadata i html-sider med RDFa

DCAT-metadata kan indlejres i eksisterende html-sider vha. JSON-LD eller RFDa. 

RDFa er en W3C-anbefaling der tilføjer et sæt attributniveauudvidelser til HTML, XHTML og forskellige XML-baserede dokumenttyper til indlejring af metadata i webdokumenter.

## Læs mere om RDFa:
- W3C RDFa 1.1 Primer (Intro til RDFa): https://www.w3.org/TR/rdfa-primer/ 
- W3C RDFa Lite (Forenklet RDFa-specifikation): https://www.w3.org/TR/rdfa-lite/
- W3C RFDa Core 1.1 (Fuld RDFa-specifikation): https://www.w3.org/TR/rdfa-core/ 
- Linked Data in HTML: http://rdfa.info/
- Wikipedia om RDFa: https://en.wikipedia.org/wiki/RDFa

## Praktiske vejledninger til DCAT-opmærkning med RDFa : 
- https://theodi.org/article/marking-up-your-dataset-with-dcat/
- https://developers.google.com/search/docs/data-types/dataset
- https://github.com/SEMICeu/dcat-ap-rdf2html The XSLT transforming a set of DCAT-AP records from RDF/XML to HTML+RDFa.

## Eksempler
Med fx [W3Cs RDF distiller](https://www.w3.org/2012/pyRdfa/Overview.html) eller [HTML Structured Data Extractor to RDF](https://www.w3.org/2012/sde/) kan DCAT-metadata udtrækkes fra eksempel-html-filer i denne mappe.
- **HTML**-filen [RDFa1_basic-example1.html](https://htmlpreview.github.io/?https://raw.githubusercontent.com/digst/DCAT-AP-DK/master/releases/v.2.0/examples/RDFa/RDFa1_basic-example1.html)  -- giver **DCAT RDF/XML**-fil --> https://www.w3.org/2012/sde/extract?uri=https%3A%2F%2Fraw.githubusercontent.com%2Fdigst%2FDCAT-AP-DK%2Fmaster%2Freleases%2Fv.2.0%2Fexamples%2FRDFa%2FRDFa1_basic-example1.html&source=rdfa&source=microdata&source=hturtle&format=xml&vocab_expansion=false
- **HTML**-filen [RDFa2_basic-example1.html](https://htmlpreview.github.io/?https://raw.githubusercontent.com/digst/DCAT-AP-DK/master/releases/v.2.0/examples/RDFa/RDFa2_basic-example1.html)  -- giver **DCAT RDF/XML**-fil --> https://www.w3.org/2012/sde/extract?uri=https%3A%2F%2Fraw.githubusercontent.com%2Fdigst%2FDCAT-AP-DK%2Fmaster%2Freleases%2Fv.2.0%2Fexamples%2FRDFa%2FRDFa2_basic-example1.html&source=rdfa&source=microdata&source=hturtle&format=xml&vocab_expansion=false





