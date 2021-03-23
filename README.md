# HTW | Playground: Fork Colors

Das Repository dient im Praktikum als Spielwiese, um **Fork** und **Pull-Request** kennenzulernen. Es ist eine kleine Webanwendung, welche über GitHub Page angezeigt wird und anhand einer JSON-Datei Farbkreise darstellt.

Link zur GitHub Page: https://tigion.github.io/htw-playground-fork-colors/

## Worum geht es?

Um einen Farbkreis in diesem Repository zu hinterlassen, muss ein Fork mit einem Pull-Request durchgeführt werden.

Dazu muss in einem Pull-Request die JSON-Datei _colors.json_ im Verzeichnis `/data` angepasst werden. Hier wird ein Eintrag mit dem GitHub-Account oder Namen bei `id:` und einer Farbe im rgb-Format bei `color:` hinerlassen.

## Aufbau der _/data/colors.json_ Datei

In der Datei *colors.json* befinden sich ein Array von Objekten bestehend aus eine ID (`id`) und einer Farbe (`color`):

```json
[
  {
    ...
  },
  {
    "id": "",
    "color": { "r": 255, "g": 255, "b": 255 }
  }
]
```

* `id:` ... GitHub-Account oder Name
* `color:`
  * `r:` ... Wert von **rot** zwischen `0` und `255`
  * `g:` ... Wert von **gelb** zwischen `0` und `255`
  * `b:` ... Wert von **blau** zwischen `0` und `255`

Achtet beim Hinzufügen eines neuen `{ id: ... colors: ... }`-Eintrages darauf, dass sich vor dem letzte Eintrag **ein Komma** und danach **keines** befindet.

## Vorgehen

1. Forke dieses Repository als Kopie in deinen Account.
2. Führe davon einen lokalen Clone auf deinen Rechner aus.
3. Erstelle dir einen neuen Branch und wechsle in diesen.
4. Füge der *colors.json* einen neuen Eintrag mit deinen Werten hinzu. Alternativ passt du einen Eintrag an, bei welchem die `id:` noch leer (`""`) ist.
5. Nim die Änderung als neuen Commit auf und pushe sie mit dem zugehörigen Branch in dein Repository.
6. Schlage mit jetzt die Änderung als Pull-Request vor.
7. Ich schaue mir - *undefinierte Verzögerung* - deinen Pull-Request an. Ist er okay, übernehme ich die Änderung und nach kurzer Zeit ist dein Farbkreis zu sehen. Ist er nicht okay hinterlasse ich einen Kommentar.
8. Ist der Pull-Request erfolgreich von mir übernommen, kann dein Fork (bei nicht gebrauch) gelöscht werden.