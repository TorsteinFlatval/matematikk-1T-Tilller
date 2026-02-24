
# Volum

## Oversikt over volum-formler

Her er en oversikt over volumformlene for de vanligste geometriske figurene:

:::::{grid} 1 1 2 2
---
gutter: 1
---

::::{grid-item-card}
:header: Rektangulær prisme
:class-header: sd-card-header
:class-body: sd-card-body
:class: summary-card

Volumet av et rektangulært prisme med lengde $l$, bredde $b$ og høyde $h$:

$$V = l \cdot b \cdot h$$

```{plot}
width: 90%
class: no-click, adaptive-figure
axis: off, equal
xmin: 0
xmax: 7
ymin: 0
ymax: 6
fontsize: 24
line-segment: (1,2), (4,2), solid, black, 2
line-segment: (4,2), (5,1), solid, black, 2
line-segment: (5,1), (2,1), solid, black, 2
line-segment: (2,1), (1,2), solid, black, 2
line-segment: (1,2), (1,5), solid, black, 2
line-segment: (4,2), (4,5), solid, black, 2
line-segment: (5,1), (5,4), solid, black, 2
line-segment: (2,1), (2,4), solid, black, 2
line-segment: (1,5), (4,5), solid, black, 2
line-segment: (4,5), (5,4), solid, black, 2
line-segment: (5,4), (2,4), solid, black, 2
line-segment: (2,4), (1,5), solid, black, 2
line-segment: (1,0.6), (4,0.6), solid, #0072b2, 1.5
text: 2.5, 0.2, "$l$", center
line-segment: (4.3,2), (4.3,5), solid, #0072b2, 1.5
text: 4.7, 3.5, "$h$", center
line-segment: (4.2,1.8), (5,1), solid, #0072b2, 1.5
text: 4.8, 1.3, "$b$", center
```

::::

::::{grid-item-card}
:header: Kube
:class-header: sd-card-header
:class-body: sd-card-body
:class: summary-card

Volumet av en kube med sidelengde $s$:

$$V = s^3$$

```{plot}
width: 90%
class: no-click, adaptive-figure
axis: off, equal
xmin: 0
xmax: 7
ymin: 0
ymax: 6
fontsize: 24
line-segment: (1,2), (4,2), solid, black, 2
line-segment: (4,2), (5,1), solid, black, 2
line-segment: (5,1), (2,1), solid, black, 2
line-segment: (2,1), (1,2), solid, black, 2
line-segment: (1,2), (1,5), solid, black, 2
line-segment: (4,2), (4,5), solid, black, 2
line-segment: (5,1), (5,4), solid, black, 2
line-segment: (2,1), (2,4), solid, black, 2
line-segment: (1,5), (4,5), solid, black, 2
line-segment: (4,5), (5,4), solid, black, 2
line-segment: (5,4), (2,4), solid, black, 2
line-segment: (2,4), (1,5), solid, black, 2
line-segment: (1,0.6), (4,0.6), solid, #0072b2, 1.5
text: 2.5, 0.2, "$s$", center
line-segment: (4.3,2), (4.3,5), solid, #0072b2, 1.5
text: 4.7, 3.5, "$s$", center
line-segment: (4.2,1.8), (5,1), solid, #0072b2, 1.5
text: 4.8, 1.3, "$s$", center
```

::::

::::{grid-item-card}
:header: Sylinder
:class-header: sd-card-header
:class-body: sd-card-body
:class: summary-card

Volumet av en sylinder med radius $r$ og høyde $h$:

$$V = \pi r^2 h$$

```{plot}
width: 90%
class: no-click, adaptive-figure
axis: off, equal
xmin: 0
xmax: 6
ymin: 0
ymax: 6
fontsize: 24
ellipse: (3,1.5), 1.2, 0.3, solid, black, 2, 0
line-segment: (1.8,1.5), (1.8,4.5), solid, black, 2
line-segment: (4.2,1.5), (4.2,4.5), solid, black, 2
ellipse: (3,4.5), 1.2, 0.3, solid, black, 2, 0
line-segment: (3,1.2), (3,4.5), solid, #0072b2, 1.5
text: 2.5, 2.8, "$h$", center
line-segment: (3,1.5), (4.2,1.5), solid, #0072b2, 1.5
text: 3.6, 1.1, "$r$", center
```

::::

::::{grid-item-card}
:header: Pyramide
:class-header: sd-card-header
:class-body: sd-card-body
:class: summary-card

Volumet av en pyramide med grunnflate $G$ og høyde $h$:

$$V = \frac{1}{3} \cdot G \cdot h$$

```{plot}
width: 90%
class: no-click, adaptive-figure
axis: off, equal
xmin: 0
xmax: 6
ymin: 0
ymax: 6
fontsize: 24
line-segment: (1,1), (4,1), solid, black, 2
line-segment: (4,1), (5,0.5), solid, black, 2
line-segment: (5,0.5), (2,0.5), solid, black, 2
line-segment: (2,0.5), (1,1), solid, black, 2
line-segment: (1,1), (3,5), solid, black, 2
line-segment: (4,1), (3,5), solid, black, 2
line-segment: (5,0.5), (3,5), solid, black, 2
line-segment: (2,0.5), (3,5), solid, black, 2
line-segment: (3,1), (3,5), dashed, #0072b2, 1.5
text: 2.5, 2.5, "$h$", center
line-segment: (1,0.8), (4,0.8), solid, #0072b2, 1.5
text: 2.5, 0.4, "$G$", center
```

::::

::::{grid-item-card}
:header: Kule
:class-header: sd-card-header
:class-body: sd-card-body
:class: summary-card

Volumet av en kule med radius $r$:

$$V = \frac{4}{3} \pi r^3$$

```{plot}
width: 90%
class: no-click, adaptive-figure
axis: off, equal
xmin: 0.5
xmax: 5.5
ymin: 0.5
ymax: 4.5
fontsize: 24
circle: (3,2.5), 1.5, solid, black, 2.5
line-segment: (3,2.5), (4.5,2.5), solid, #0072b2, 2
text: 3.75, 2.1, "$r$", center
```

::::

::::::

---

:::::::::::::::{admonition} Underveisoppgave 1
---
class: check
---

En kube har sidelengde $2$ cm.

Regn ut volumet av kuben og forklar hvordan vi får $\text{cm}^3$ som enhet når vi regner ut volumet. Figuren viser kuben delt inn i 8 små kuber, ett for hver kubikkcentimeter.

```{plot}
width: 50%
class: no-click, adaptive-figure
axis: off, equal
xmin: 0
xmax: 7
ymin: 0
ymax: 6
fontsize: 18
line-segment: (1,2), (4,2), solid, black, 2
line-segment: (4,2), (5,1), solid, black, 2
line-segment: (5,1), (2,1), solid, black, 2
line-segment: (2,1), (1,2), solid, black, 2
line-segment: (1,2), (1,5), solid, black, 2
line-segment: (4,2), (4,5), solid, black, 2
line-segment: (5,1), (5,4), solid, black, 2
line-segment: (2,1), (2,4), solid, black, 2
line-segment: (1,5), (4,5), solid, black, 2
line-segment: (4,5), (5,4), solid, black, 2
line-segment: (5,4), (2,4), solid, black, 2
line-segment: (2,4), (1,5), solid, black, 2
line-segment: (2.5,2), (2.5,5), solid, black, 1
line-segment: (1,3.5), (4,3.5), solid, black, 1
line-segment: (2.5,1), (3.5,0.5), solid, black, 1
line-segment: (2.5,4), (3.5,3.5), solid, black, 1
line-segment: (3.5,0.5), (3.5,3.5), solid, black, 1
line-segment: (1,2), (2,1.5), solid, black, 1
line-segment: (1,5), (2,4.5), solid, black, 1
line-segment: (2,4.5), (3,4), solid, black, 1
line-segment: (2,1.5), (3,1), solid, black, 1
line-segment: (4,2), (5,1.5), solid, black, 1
line-segment: (4,5), (5,4.5), solid, black, 1
fill-polygon: (1,2), (1,3.5), (2.5,3.5), (2.5,2), #0072b2, 0.3
line-segment: (0.8,2), (0.8,3.5), solid, #0072b2, 2
text: 0.3, 2.7, "$2$ cm", center, fontsize: 10
line-segment: (1,1.85), (2.5,1.85), solid, #0072b2, 2
text: 1.75, 1.6, "$2$ cm", center, fontsize: 10
line-segment: (0.8,3.5), (1.3,3.2), solid, #0072b2, 2
text: 0.2, 3.5, "$2$ cm", center, fontsize: 10
text: 1.75, 2.7, "$1$cm$^3$", center, fontsize: 8
text: 0.0, 0.5, "$s = 2$ cm", center, fontsize: 12
```

:::::::::::::::

::::{admonition} Løsning
---
class: solution
---

**Bruk av figuren:**
Figuren viser hvordan kuben med sidelengde 2 cm er delt inn i 8 små kuber. Hvert lite kube representerer 1 cm³ (1 kubikkcentimeter), slik figuren viser med den blåe kuben.

- Siden kuben har **2 cm i lengden**, får vi **2 små kuber langs lengden**
- Siden kuben har **2 cm i bredden**, får vi **2 små kuber langs bredden**
- Siden kuben har **2 cm i høyden**, får vi **2 små kuber langs høyden**
- Totalt: **2 · 2 · 2 = 8 små kuber** = **8 cm³**

**Formelen og beregningen:**
Vi bruker formelen for volumet av en kube:

$$
V = s \cdot s \cdot s = s^3
$$

Når vi setter inn sidelengden $s = 2$ cm, får vi:

$$
V = 2 \text{ cm} \cdot 2 \text{ cm} \cdot 2 \text{ cm} = 8 \text{ cm}^3
$$

**Hvorfor blir enheten cm³:**
Når vi ganger en lengde målt i centimeter med to andre lengder målt i centimeter, får vi et volum målt i kubikkcentimeter. Vi ganger både **tallene** ($2 \cdot 2 \cdot 2 = 8$) og **enhetene** ($\text{cm} \cdot \text{cm} \cdot \text{cm} = \text{cm}^3$).
::::
