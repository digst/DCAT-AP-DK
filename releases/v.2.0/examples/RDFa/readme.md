# Indlejring af eksisterende DCAT-metadata med RDFa

DCAT-metadata kan indlejres i eksisterende opmærkning vha. JSON-LD eller RFDa. 

RDFa er en W3C-anbefaling der tilføjer et sæt attributniveauudvidelser til HTML, XHTML og forskellige XML-baserede dokumenttyper til indlejring af metadata i webdokumenter, https://en.wikipedia.org/wiki/RDFa

Læs mere om RFDa i disse vejledninger: 

- https://theodi.org/article/marking-up-your-dataset-with-dcat/
- https://developers.google.com/search/docs/data-types/dataset

Og se et eksempel her:
https://data.gov.dk/test/rdfa/RDFa2_basic-example1.html

Med fx [W3Cs RDF distiller](https://www.w3.org/2012/pyRdfa/Overview.html) kan  DCAT-metadata udtrækkes fra denne eksempel-html-fil:
- uri= https://data.gov.dk/test/rdfa/RDFa2_basic-example1.html

Mini-guide på engelsk til direkte brug af RDF distiller:
- Extract the RDF with whitespace preservation and without warnings, serialized in Turtle:
http://www.w3.org/2012/pyRdfa/extract?uri=https://data.gov.dk/test/rdfa/RDFa2_basic-example1.html
- Extract the RDF with whitespace preservation and without warnings, serialized in RDF/XML:
http://www.w3.org/2012/pyRdfa/extract?format=xml&uri=https://data.gov.dk/test/rdfa/RDFa2_basic-example1.html
- Extract the RDF from  with whitespace preservation and including warnings, serialized in Turtle:
http://www.w3.org/2012/pyRdfa/extract?graph=default,processor&uri=https://data.gov.dk/test/rdfa/RDFa2_basic-example1.html
- Use a fixed, pseudo URI to extract the RDF from the current page without specifying its URI (with default options); this can be used, say, as a link for a button on the page: http://www.w3.org/2012/pyRdfa/extract?uri=referer


<!DOCTYPE html>
<html lang="en" prefix="dct: http://purl.org/dc/terms/
              rdf: http://www.w3.org/1999/02/22-rdf-syntax-ns#
              dcat: http://www.w3.org/ns/dcat#
              foaf: http://xmlns.com/foaf/0.1/">
    <head>
        <title>basic-example1 in RDFa</title>
    </head>
 <body>
<article about="https://dcat.example.org/dataset-001" typeof="dcat:Dataset">
<h1>Dataset 001</h1> 
	<table class="table">
    <tr><td>Title:</td><td property="dc:title">Dataset 001</td></tr>
    <tr><td>Description:</td> <td property="dc:description">A description of Dataset 001</td></tr>
    <tr><td>Langauge:</td> <td property="dc:language" resource="http://publications.europa.eu/resource/dataset/language/DAN">DAN</td></tr>
    <tr><td>Accrual Periodicity:</td> <td property="dcat:accrualPeriodicity" resource="http://publications.europa.eu/resource/authority/frequency/ANNUAL">ANNUAL</td>	  </tr>
    <tr><td>Identifier:</td> <td property="dc:identifier" resource="https://dcat.example.org/dataset-001">https://dcat.example.org/dataset-001</td></tr>
    <tr><td>Publisher:</td> <td property="dc:publisher" resource="https://dcat.example.org/agent-001">Agent-001</td></tr>	  
    <tr><td class="field-label">Distributioner:</td>
	<td>	
		<!-- DATASET DISTRIBUTIONS --> 	  
		<table class="table">
			<tr property="dcat:distribution" typeof="dcat:Distribution" resource="https://dcat.example.org/dataset-001.csv">
				<td property="dct:title">dataset-001.csv</td>
				<td property="dcat:format" resource="http://publications.europa.eu/resource/authority/file-type/csv">CSV</td>
				<td property="dcat:byteSize" content="5120.0" datatype="xsd:decimal">5120.0 bytes</td>
				<td>
				<a property="dcat:accessURL" class="btn btn-primary" href="https://dcat.example.org/dataset-001.csv">Download</a>
				</td>
			</tr>
			<tr property="dcat:distribution" typeof="dcat:Distribution" resource="https://dcat.example.org/dataset-001.xml">
				<td property="dct:title">dataset-001.xml</td>
				<td property="dcat:format" resource="http://publications.europa.eu/resource/authority/file-type/xml">XML</td>
				<td property="dcat:byteSize" content="6120.0" datatype="xsd:decimal">6120.0 bytes</td>
				<td>
				<a property="dcat:accessURL" class="btn btn-primary" href="https://dcat.example.org/dataset-001.xml">Download</a>
				</td>
			</tr>
			</table>
	</td>
	</table>
  </article>
  </body>
</html>
