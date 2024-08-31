# beamerUNAM
Tema de beamer para las presentaciones para los videos.

## Instalación
Para encontrar el directorio donde se instalan los archivos locales usar:

```
$ kpsewhich -var-value TEXMFLOCAL
```

Por ejemplo, en ubuntu 20.04 obtuve:

```
/usr/local/share/texmf
```

Si aún no existe, crear desde ahí el siguiente directorio:

```
cd `kpsewhich -var-value TEXMFLOCAL`
sudo mkdir -p tex/latex/beamer/
```

Copiar ahí los archivos `.sty` que se encuentran dentro del directorio `theme`.  Por ejemplo con:

```
$ sudo cp theme/*.sty /usr/local/share/texmf/tex/latex/beamer/
```

Finalmente, para actualizar la base de datos de latex, ejecutar:

```
$ sudo texhash
```
