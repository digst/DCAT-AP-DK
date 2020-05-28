<!DOCTYPE html>
<html prefix="dct: http://purl.org/dc/terms/
              rdf: http://www.w3.org/1999/02/22-rdf-syntax-ns#
              dcat: http://www.w3.org/ns/dcat#
              foaf: http://xmlns.com/foaf/0.1/">
<body>
<h1>Indlejring af eksisterende DCAT-metadata med RDFa</h1>

<p>DCAT-metadata kan indlejres i eksisterende opmærkning vha. JSON-LD eller RFDa. </p>

<p>RDFa er en W3C-anbefaling der tilføjer et sæt attributniveauudvidelser til HTML, XHTML og forskellige XML-baserede dokumenttyper til indlejring af metadata i webdokumenter, https://en.wikipedia.org/wiki/RDFa</p>
<p>
Læs mere om RFDa i disse vejledninger :
<ol><li>https://theodi.org/article/marking-up-your-dataset-with-dcat/</li>
<li>https://developers.google.com/search/docs/data-types/dataset</li>
</ol>


</p>

<p>Og se et lille eksempel her:</p>
<!-- A DATASET --> 
<article about="https://dcat.example.org/dataset-001" typeof="dcat:Dataset">
  <table class="table">
    <tr><td>Title:</td><td property="dc:title">Dataset 001</td></tr>
    <tr><td>Description:</td> <td property="dc:description">A description of Dataset 001</td></tr>
    <tr><td>Langauge:</td> <td property="dc:language" resource="http://publications.europa.eu/resource/dataset/language/DAN">DAN</td></tr>
    <tr><td>Accrual Periodicity:</td> <td property="dcat:accrualPeriodicity" resource="http://publications.europa.eu/resource/authority/frequency/ANNUAL">ANNUAL</td>	  </tr>
    <tr><td>Identifier:</td> <td property="dc:identifier" resource="https://dcat.example.org/dataset-001">https://dcat.example.org/dataset-001</td></tr>
    <tr><td>Publisher:</td> <td property="dc:publisher" resource="https://dcat.example.org/agent-001">Agent-001</td></tr>	  
    <tr><td class="field-label">Distributioner:</td>
	<td><!-- DATASET DISTRIBUTIONS --> 	  
		<table class="table">
			<tr property="dcat:distribution" typeof="dcat:Distribution" resource="https://dcat.example.org/dataset-001.csv">
				<td property="dct:title">dataset-001.csv</td>
				<td property="dcat:format" resource="http://publications.europa.eu/resource/authority/file-type/csv">CSV</td>
				<td property="dcat:byteSize" content="5120.0" datatype="xsd:decimal">5120.0 bytes</td>
				<td><a property="dcat:accessURL" class="btn btn-primary" href="https://dcat.example.org/dataset-001.csv">Download</a>
				</td>
			</tr>
			<tr property="dcat:distribution" typeof="dcat:Distribution" resource="https://dcat.example.org/dataset-001.xml">
				<td property="dct:title">dataset-001.xml</td>
				<td property="dcat:format" resource="http://publications.europa.eu/resource/authority/file-type/xml">XML</td>
				<td property="dcat:byteSize" content="6120.0" datatype="xsd:decimal">6120.0 bytes</td>
				<td><a property="dcat:accessURL" class="btn btn-primary" href="https://dcat.example.org/dataset-001.xml">Download</a>
				</td>
			</tr>
			</table>
			</td>
		</table>
    </dl>
  </article>
  </body>
</html>
