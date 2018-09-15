# Variable-Fonts der IAD2017

Um die Fonts zu generieren werden folgende Tools benötigt:

* [fontmake](https://github.com/googlei18n/fontmake)
  * `pip install fontmake`

## ToDo
1. [UFO-Dateien](http://unifiedfontobject.org/) erstelle: ([Konverter ab OTF](https://everythingfonts.com/otf-to-ufo))
2. UFO-Dateien unter `./src/{{name}}/ufo/{{dateiname.ufo}}` speichern
3. [Designspace-File](https://github.com/LettError/designSpaceDocument) aufgrund von `./src/_example/scaler.designspace` in `./src/{{name}}/{{dateiname.designspace}}` erstellen
4. Mit `fontmake` Variable Font erstellen. Befehl: `fontmake -o variable -m ./src/{{name}}/{{dateiname.designspace}}`
5. Den erstelten Variable Font in ein [WOFF](https://everythingfonts.com/ttf-to-woff) & [WOFF2](https://everythingfonts.com/ttf-to-woff2) konvertieren.
6. WOFF-Dateien in `./docs/fonts/{{name}}/` kopieren
7. CSS in `./docs/fonts/styles.css/` erstellen. Siehe `./src/_example/styles.css`
8. HTML in `./docs/index.html` anpassen.

## Weitere Infos
* [I Can Variable Font](https://github.com/scribbletone/i-can-variable-font)
