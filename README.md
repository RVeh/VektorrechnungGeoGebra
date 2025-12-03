# Vektorrechnung mit GeoGebra  
## Schnitt zweier Ebenen – strukturiert, verständlich, unterrichtstauglich

Dieses Repository enthält Material für den Unterricht (Sek II) zum Thema  
**Schnitt zweier Ebenen in Parameterform** mit **GeoGebra**.

Der Fokus liegt auf einem **didaktisch sauberen**, **strukturierten** Vorgehen,
das Schüler*innen wirklich verstehen lässt, wie Geraden und Ebenen aufgebaut
sind – und wie man zuverlässig die **Schnittgerade** bestimmt.

Alle Dateien sind sofort einsatzbereit.

---

## 🎯 Ziel des Materials

- Schüler*innen sollen Ebenen **korrekt und strukturiert** in GeoGebra eingeben.
- Die Schnittgerade wird **nicht** über Spezialbefehle erzeugt,  
  sondern über ein **LGS und die Parametergleichung**.
- Lehrkräfte erhalten ein Materialpaket, das **funktioniert**,  
  **Verständnis aufbaut** und **Fehler verhindert**.

---

## 📂 Inhalte des Repositories

### ✔ 1. GeoGebra-Datei (`.ggb`)
**`Ebenen_Schnitt_Parameterform.ggb`**

- Zwei Ebenen in Parameterform (Stützvektor + Spannvektoren)  
- Visualisierung der Ebenen im Raum  
- LGS wird im CAS-Fenster gelöst  
- Schnittgerade wird sichtbar und parametrisiert

Die Datei ist so aufgebaut, dass SuS  
➡️ zuerst **strukturiert eingeben**,  
➡️ dann **LGS lösen**,  
➡️ danach **die Gerade interpretieren** können.

---

### ✔ 2. Aufgabenblatt / Aufgabenfolie (PDF)

Enthält:

- Aufgabenstellung  
- saubere Notation  
- Parameterformen der Ebenen  
- Platz für eigene Notizen der Schüler*innen

---

### ✔ 3. Lehrer-Folien (PDF, später vollständig)
Mit folgendem Aufbau:

1. **Problemstellung** (Was soll bestimmt werden?)  
2. **Eingabe der Ebenen**  
   - Stützvektor + Spannvektoren  
   - Struktur sichtbar machen  
3. **LGS für den Schnitt**  
   → Solve (kein Intersect!)  
4. **Parametrische Darstellung der Schnittgeraden**  
5. **Fehlervermeidung**:  
   - `A + u` nicht verwenden  
   - `Plane(A,u,v)` nicht verwenden  
   - `Intersect(E1,E2)` liefert oft falsche Objekte  
6. **Tiefbohrung**: Vergleich PMF vs. Ebenengleichung

Diese Folien entsprechen einem **strukturorientierten Mathematikunterricht**.

---

## 💡 Didaktischer Hintergrund

GeoGebra implementiert die volle affine Geometrie –  
die Schulmathematik jedoch nicht.

Um Missverständnisse zu vermeiden, nutzen wir **nur Befehle**, die:

- mathematisch korrekt im Unterrichtskontext sind  
- transparente Strukturen zeigen  
- im Algebrafenster und CAS konsistent funktionieren  
- Blackbox-Effekte vermeiden  

Das bedeutet konkret:

### ✔ Diese Befehle verwenden wir:
```geogebra
Vector(A,B)
Line(A,B)
Plane(A,B,C)
Solve(...)
