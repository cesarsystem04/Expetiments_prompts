
Convertir los archivos PDF en Markdown

uvx "markitdown[all]" "Estado de cuenta2026-10.pdf" -o  document.md 


`markitdown path-to-file.pdf > document.md`


`markitdown[all] "Estado de cuenta2026-10.pdf.pdf" > document.md`


Instalar python 



Comprobar cuantas paginas tiene el archivo

uvx --from pypdf python -c "from pypdf import PdfReader; r=PdfReader('Estado de cuenta2026-10.pdf'); print('Total de páginas:', len(r.pages))"


Comprobar cuanto contenido tiene el mardown 

(Get-Item ".\document.md").Length
