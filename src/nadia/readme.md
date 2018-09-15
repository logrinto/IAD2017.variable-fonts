# Variable-Fonts der IAD2017

Um die Fonts zu generieren werden folgende Tools benötigt:

* [fontmake](https://github.com/googlei18n/fontmake)
  * `pip install fontmake`

## ToDo
* [UFO-Dateien](http://unifiedfontobject.org/) erstelle: ([Konverter ab OTF](https://everythingfonts.com/otf-to-ufo))
* UFO-Dateien unter `./src/{{name}}/ufo/{{dateiname.ufo}}` speichern
* [Designspace-File](https://github.com/LettError/designSpaceDocument) aufgrund von `./src/_example/scaler.designspace` in `./src/{{name}}/{{dateiname.designspace}}` erstellen
* Mit `fontmake` Variable Font erstellen. Befehl: `fontmake -o variable -m ./src/{{name}}/{{dateiname.designspace}}`
* Den erstelten Variable Font in ein [WOFF](https://everythingfonts.com/ttf-to-woff) & [WOFF2](https://everythingfonts.com/ttf-to-woff2) konvertieren.
* WOFF-Dateien in `./docs/fonts/{{name}}/` kopieren
* CSS in `./docs/fonts/styles.css/` erstellen. Siehe `./src/_example/styles.css`
* HTML in `./docs/index.html` anpassen.

## Weitere Infos
* [I Can Variable Font](https://github.com/scribbletone/i-can-variable-font)
