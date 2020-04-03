Comprimir archivos pdf command linux

```
gs -sDEVICE=pdfwrite -dCompatibilityLevel=1.4 -dPDFSETTINGS=/screen -dNOPAUSE -dQUIET -dBATCH -sOutputFile=destino.pdf origen.pdf

```

Opciones:

Introduciendo diferentes valores  para dPDFSETTINGS modificamos la calidad, tamaño y resolución del archivo de salida ejemplos:

```
dPDFSETTINGS=/screen (72 dpi, peor calidad)
dPDFSETTINGS=/ebook (150 dpi, calidad media)
dPDFSETTINGS=/printer (300 dpi, alta calidad)
dPDFSETTINGS=/prepress (300 dpi, alta calidad preservando el color)
dPDFSETTINGS=/default ( idéntico a screen )
```
