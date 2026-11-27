# oida-wuerfel

Ein kleines Paket für die Programmiersprache [OIDA](https://github.com/lelewithheart/oida-lang):
Würfeln und Münze werfen. Es ist vor allem dazu da, `oida hol` auszuprobieren.

## Holen

Im Ordner des eigenen Programms:

```
oida hol lelewithheart/oida-wuerfel
```

Das Paket liegt dann in `pakete/oida-wuerfel` und steht in `pakete.txt`.

## Verwenden

```
BRAUCH "oida-wuerfel" OIS w OIDA

SCHREIB(w.wuaf()) OIDA             # 1 bis 6
SCHREIB(w.wuaf_mit(20)) OIDA       # 1 bis 20
SCHREIB(w.mehrmois(3)) OIDA        # zum Beispiel [4, 1, 6]
SCHREIB(w.summe_von(2)) OIDA       # zwei Würfel zusammen: 2 bis 12
SCHREIB(w.münze()) OIDA            # Kopf oder Zoi
```

## Was drin ist

| Funktion | Ergebnis |
|---|---|
| `wuaf()` | ein Wurf mit einem gewöhnlichen Würfel |
| `wuaf_mit(seitn)` | ein Wurf mit einem Würfel mit so vielen Seiten |
| `mehrmois(wia_oft)` | mehrere Würfe als `LISTN VON ZOI` |
| `summe_von(wia_oft)` | die Summe von mehreren Würfen |
| `münze()` | `"Kopf"` oder `"Zoi"` |

Ein Paket für OIDA ist ein Ordner mit einer Datei `paket.oida` (hier) oder einer Datei, die so
heißt wie das Paket. Weitere Dateien holt sie selbst mit `BRAUCH` dazu (hier `teile/zöhn.oida`).
