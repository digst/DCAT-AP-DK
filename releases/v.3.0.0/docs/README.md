
HTML-indholdet er udstillet som GitHub Pages[1] her: https://digst.github.io/DCAT-AP-DK/releases/v.3.0.1/docs/

Her ligger følgende filer:
- README.md - Denne fil
- index.md - Mastertekst i Markdown-format  [2] [3]
- index.html - Mastertekst konverteret til html

[1] Udstilling via GitHub Pages kan aktiveres via repositoriets 'Settings' (scroll ned til GitHub Pages)

[2] Konvertering kan fx ske via Bikeshed's webformular: https://api.csswg.org/bikeshed/

[3] Word (docx) filer kan konverteres til Markdown via fx: https://euangoddard.github.io/clipboard2markdown/

Indsæt følgende script nederst i body i index.html filen, for at tilføje tabindex i indholdsfortegnelse:

<script>
    /*Set attribute tabindex on all elements in TOC*/
    var toc =  document.querySelectorAll("#toc .content");
    for (var i = 0; i < toc.length; i++) {
      if (!toc[i].hasAttribute("tabindex")){
        var att = document.createAttribute("tabindex");
        att.value = "0";
        toc[i].setAttributeNode(att);
      }
    }
    /*Set lang attribute value to "da" in html tag*/
    document.getElementsByTagName("html")[0].setAttribute("lang", "da");
</script>
