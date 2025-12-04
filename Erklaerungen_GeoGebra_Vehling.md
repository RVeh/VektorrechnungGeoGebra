# 📄 Bemerkungen zur Schnittgerade zweier Ebenen in Parameterform (PMF)

## 1. Parameterform und LGS – was steckt dahinter?

Eine Ebene in Parameterform  
$$ 
E(s,t)= a + s\,u + t\,v 
$$
ist mathematisch gesehen nichts anderes als eine **Lösung eines linearen Gleichungssystems (LGS)**:

- 3 Gleichungen (für x, y, z)  
- 4 Unbekannte $(s,t,p,q)$, weil zwei Ebenen jeweils zwei Parameter besitzen.

---

## 2. Was passiert beim Schnitt zweier Ebenen?

Für zwei Ebenen $E_1(s,t)$ und $E_2(p,q)$ gilt:

$$ E_1(s,t) = E_2(p,q) $$

Daraus entstehen drei Gleichungen:

| Gleichung                     | Bedeutung                 |
|------------------------------|---------------------------|
| $x(E_1) = x(E_2)$          | Vergleich der x-Koordinate |
| $(y(E_1) = y(E_2)$         | Vergleich der y-Koordinate |
| $z(E_1) = z(E_2)$          | Vergleich der z-Koordinate |

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

Damit formulieren wir das LGS:

```ggb
gl1 := x(E1(s,t)) = x(E2(p,q))
gl2 := y(E1(s,t)) = y(E2(p,q))
gl3 := z(E1(s,t)) = z(E2(p,q))
