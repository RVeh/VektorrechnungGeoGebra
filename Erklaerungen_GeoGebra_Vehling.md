# 📄 Bemerkungen zur Schnittgerade zweier Ebenen in Parameterform (PMF)

## 1. Parameterform und LGS – was steckt dahinter?

Eine Ebene in Parameterform  $E(s,t)= \vec{a} + s\cdot \vec{u} + t\cdot \vec{v}$
ist mathematisch gesehen nichts anderes als  **ein lineares Gleichungssystems (LGS)**:

- 3 Gleichungen (für x, y, z)  
- 4 Unbekannte $(s,t,p,q)$, weil zwei Ebenen beteiligt sind und zwei Ebenen jeweils zwei Parameter besitzen.

Eigenlich müsste es $\vec{E}(s,t)$ heißen, aber Pfeile werden in GeoGebra nicht eingeben.

---

## 2. Was passiert beim Schnitt zweier Ebenen?

Für zwei Ebenen $E_1(s,t)$ und $E_2(p,q)$ gilt die Schnittbedingung:

$$ E_1(s,t) = E_2(p,q) $$

Daraus entstehen drei Gleichungen:

| Gleichung                     | Bedeutung                 |
|------------------------------|---------------------------|
| $x(E_1) = x(E_2)$          | x-Koordinaten: erste Zeile des LGS |
| $(y(E_1) = y(E_2)$         | y-Koordinaten: zweite Zeile des LGS  |
| $z(E_1) = z(E_2)$          | z-Koordinaten: dritte Zeile des LGS  |

Mögliche Fälle:

| Fall | Bedeutung |
|------|-----------|
| **1 freie Variable** | Ebenen schneiden sich in einer **Geraden** |
| **alle Variablen bestimmt** | Ebenen sind **identisch** |
| **keine Lösung** | Ebenen sind **parallel** |

**Merke:** Eine Schnittgerade entsteht genau dann, wenn **genau ein Parameter frei bleibt**.

---

## 3. Umsetzung in GeoGebra (CAS)

Zugriff auf Koordinaten:

- `x(.)`
- `y(.)`
- `z(.)`

Beispiele:

- \(x(P)=1\) für \(P(1,2,3)\)  
- \(x(E_1(s,t))\) liefert die x-Komponente der PMF

Damit formulieren wir das LGS:

```ggb
gl1 := x(E1(s,t)) = x(E2(p,q))
gl2 := y(E1(s,t)) = y(E2(p,q))
gl3 := z(E1(s,t)) = z(E2(p,q))
```
---
Jetzt wird das LGS gelösr:

g(q) := Löse({gl1, gl2, gl3}, {s, t, p})

Wir wählen **q als freien Parameter**
(Alternativ wären auch s, t oder p möglich.)

GeoGebra liefert dann eine Lösung in vektorieller Form.

## 4. Wie entsteht eine Geradengleichung?

Eine Geradengleichung hat die Form: $\vec{x}=\vec{a}+t \cdot \vec{r}$.

In GeoGebra-CAS sieht das so aus: $g(t):=\vec{a}+t \cdot \vec{r}$, aber als ein Vektor geschrieben (s. Datei).

Mit $g(0)$ erhält man einen Stützvektot und mit $g(1)-g(0)$ einen Richtungsvektor.

Warum steht dort zweimal *ein*? Es gibt unendlich viele Stützvektorn und unendlich viele linear abhängige Richtungsvektoren.

---

So sieht die Texteingabe (LaTeX anklicken) aus, damit im Textfenster die scböne Vektor-Darstellung entsteht.

<img width="400" height="600" alt="Texteingabe_LaTeX" src="https://github.com/user-attachments/assets/d636d94b-e124-442d-8a79-a6978882f46a" />

---


