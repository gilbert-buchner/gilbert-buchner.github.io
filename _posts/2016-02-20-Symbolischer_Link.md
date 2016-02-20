---
layout: post
title: Symbolischen Link erstellen (Windows)
---
<p>
cmd als Admin ausführen</p> 
<p>
<code>
mklink /D linkname verzeichnisname
</code></p>
<p>
praktisches Beispiel:
</p>
<code>
C:\xamp\htdocs>mklink /D projekta "c:\meine_projekte\projekta"
</code>

symbolische Verknüpfung erstellt für projekta <<===>> c:\meine_projekte\projekta
