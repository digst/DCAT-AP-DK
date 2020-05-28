<!DOCTYPE html>
<html prefix="dct: http://purl.org/dc/terms/
              rdf: http://www.w3.org/1999/02/22-rdf-syntax-ns#
              dcat: http://www.w3.org/ns/dcat#
              foaf: http://xmlns.com/foaf/0.1/">
    <head>
        <title>basic-example1 in RDFa</title>
    </head>
 <body>
 
 
<!-- A DATASET --> 
<article about="/node/1234" typeof="dcat:Dataset">
    <dl>
      <dt>Title:</dt>      	<dd property="dc:title">Dataset 001</dd>
      <dt>Description:</dt> <dd property="dc:description">A description of Dataset 001</dd>
      <dt>Langauge:</dt> <dd property="dc:language">http://publications.europa.eu/resource/dataset/language/DAN</dd>
      <dt>Accrual Periodicity:</dt> <dd property="dcat:accrualPeriodicity">http://publications.europa.eu/resource/authority/frequency/ANNUAL</dd>	  
      <dt>Identifier:</dt> <dd property="dc:identifier">https://dcat.example.org/dataset-001</dd>
      <dt>Publisher:</dt> <dd property="dc:publisher">https://dcat.example.org/agent-001</dd>	  
      <dt class="field-label">Distributioner:</dt>
		<!-- DATASET DISTRIBUTIONS --> 	  
		<table class="table">
			<thead>
				<tr>
					<th>Title</th>
					<th>Format</th>
					<th>Byte size</th>
					<th>Download</th>
				</tr>
			</thead>
			<tbody typeof="dcat:Dataset" property="dcat:dataset" resource="https://dcat.example.org/dataset-001.csv">
				<tr property="dcat:distribution" typeof="dcat:Distribution">
					<td property="dct:title">dataset-001.csv</td>
					<td property="dcat:mediaType" content="https://www.iana.org/assignments/media-types/text/csv">CSV</td>
					<td property="dcat:byteSize" content="5120.0" datatype="xsd:decimal">5120.0</td>
					<td property="dct:type" resource=":indirect-access">
						<a property="dcat:accessURL" class="btn btn-primary" href="https://dcat.example.org/dataset-001.csv">Download</a>
					</td>
				</tr>
			</tbody>	 
			<tbody typeof="dcat:Dataset" property="dcat:dataset" resource="https://dcat.example.org/dataset-001.xml">
				<tr property="dcat:distribution" typeof="dcat:Distribution">
					<td property="dct:title">dataset-001.xml</td>
					<td property="dcat:mediaType" content="https://www.iana.org/assignments/media-types/text/xml">XML</td>
					<td property="dcat:byteSize" content="6120.0" datatype="xsd:decimal">6120.0</td>
					<td property="dct:type" resource=":indirect-access">
						<a property="dcat:accessURL" class="btn btn-primary" href="https://dcat.example.org/dataset-001.xml">Download</a>
					</td>
				</tr>
			</tbody>	
		</table>
    </dl>
  </article>
  
  
  </body>
</html>