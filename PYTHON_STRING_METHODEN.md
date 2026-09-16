# Wichtige String-Befehle in Python

| Befehl / Methode | Zweck | Beispiel |
| --- | --- | --- |
| `len(text)` | Länge eines Strings | `len("Hallo")  # 5` |
| `str(wert)` | Wert in einen String umwandeln | `str(42)  # "42"` |
| `text.lower()` | In Kleinbuchstaben umwandeln | `"Hallo".lower()  # "hallo"` |
| `text.upper()` | In Großbuchstaben umwandeln | `"Hallo".upper()  # "HALLO"` |
| `text.capitalize()` | Ersten Buchstaben groß schreiben | `"hallo welt".capitalize()  # "Hallo welt"` |
| `text.title()` | Jedes Wort groß schreiben | `"hallo welt".title()  # "Hallo Welt"` |
| `text.strip()` | Leerzeichen außen entfernen | `"  Hallo  ".strip()  # "Hallo"` |
| `text.lstrip()` / `text.rstrip()` | Links / rechts Leerzeichen entfernen | `"  Hallo ".lstrip()` |
| `text.replace(alt, neu)` | Text ersetzen | `"Hallo".replace("a", "e")  # "Hello"` |
| `text.split(trenner)` | String in Liste aufteilen | `"a,b,c".split(",")  # ["a", "b", "c"]` |
| `trenner.join(liste)` | Liste zu String verbinden | `", ".join(["a", "b", "c"])  # "a, b, c"` |
| `text.find(suche)` | Position finden, sonst `-1` | `"Python".find("th")  # 2` |
| `text.index(suche)` | Position finden, Fehler wenn nicht vorhanden | `"Python".index("th")  # 2` |
| `text.count(suche)` | Häufigkeit zählen | `"Banane".count("a")  # 3` |
| `text.startswith(prefix)` | Prüft den Anfang | `"datei.txt".startswith("datei")  # True` |
| `text.endswith(suffix)` | Prüft das Ende | `"datei.txt".endswith(".txt")  # True` |
| `text.isalpha()` | Nur Buchstaben? | `"Hallo".isalpha()  # True` |
| `text.isdigit()` | Nur Ziffern? | `"123".isdigit()  # True` |
| `text.isalnum()` | Nur Buchstaben und Ziffern? | `"abc123".isalnum()  # True` |
| `text.isspace()` | Nur Leerraumzeichen? | `" \t".isspace()  # True` |
| `text.center(breite, zeichen)` | Text zentrieren | `"Hi".center(8, "-")  # "---Hi---"` |
| `text.zfill(breite)` | Mit führenden Nullen auffüllen | `"42".zfill(5)  # "00042"` |
| `text.format(...)` | Platzhalter ersetzen | `"Name: {}".format("Anna")` |
| f-Strings | Moderne String-Formatierung | `f"Name: {name}, Alter: {alter}"` |
| `text[0]` / `text[-1]` | Erstes / letztes Zeichen | `"Python"[0]  # "P"` |
| `text[start:ende]` | Teilstring ausschneiden | `"Python"[0:3]  # "Pyt"` |
| `text[::-1]` | String umdrehen | `"Python"[::-1]  # "nohtyP"` |

## Wichtig

Strings sind in Python unveränderlich. Methoden wie `replace()` oder `upper()`
ändern den ursprünglichen Text nicht, sondern liefern einen neuen String:

```python
text = "hallo"
text = text.upper()
print(text)  # HALLO
```
