
# Areal


## Oversikt over områdeformler

Her er en oversikt over områdeformlene for de vanligste geometriske figurene:

:::::{grid} 1 1 2 2
---
gutter: 1
---

::::{grid-item-card}
:header: Rektangel
:class-header: sd-card-header
:class-body: sd-card-body
:class: summary-card

Arealet av et rektangel med bredde $b$ og høyde $h$:

$$A = b \cdot h$$

```{plot}
width: 90%
class: no-click, adaptive-figure
axis: off, equal
xmin: 0
xmax: 6
ymin: 0
ymax: 4
fontsize: 24
fill-polygon: (1,1), (5,1), (5,3), (1,3), #0072b2, 0.1
line-segment: (1,1), (5,1), solid, black, 2.5
line-segment: (5,1), (5,3), solid, black, 2.5
line-segment: (5,3), (1,3), solid, black, 2.5
line-segment: (1,3), (1,1), solid, black, 2.5
line-segment: (1,0.5), (5,0.5), solid, #0072b2, 1.5
text: 3, 0.15, "$b$", center
line-segment: (5.3,1), (5.3,3), solid, #0072b2, 1.5
text: 5.55, 2, "$h$", center
```

::::

::::{grid-item-card}
:header: Kvadrat
:class-header: sd-card-header
:class-body: sd-card-body
:class: summary-card

Arealet av et kvadrat med sidelengde $s$:

$$A = s^2$$

```{plot}
width: 90%
class: no-click, adaptive-figure
axis: off, equal
xmin: 0
xmax: 5
ymin: 0
ymax: 5
fontsize: 24
fill-polygon: (1,1), (4,1), (4,4), (1,4), #0072b2, 0.1
line-segment: (1,1), (4,1), solid, black, 2.5
line-segment: (4,1), (4,4), solid, black, 2.5
line-segment: (4,4), (1,4), solid, black, 2.5
line-segment: (1,4), (1,1), solid, black, 2.5
line-segment: (1,0.5), (4,0.5), solid, #0072b2, 1.5
text: 2.5, 0.15, "$s$", center
line-segment: (4.35,1), (4.35,4), solid, #0072b2, 1.5
text: 4.65, 2.5, "$s$", center
```

::::

::::

::::::

:::::::::::::::{admonition} Underveisoppgave 1
---
class: check
---

Et kvadrat har sidelengde $6$ cm.

Regn ut arealet av kvadratet og forklar hvordan vi får $\text{cm}^2$ som enhet når vi regner ut arealet. Figuren viser kvadratet delt inn i 36 små kvadrater, ett for hver kvadratcentimeter.

```{plot}
width: 50%
class: no-click, adaptive-figure
axis: off, equal
xmin: 0
xmax: 5
ymin: 0
ymax: 5
fontsize: 24
fill-polygon: (1,1), (4,1), (4,4), (1,4), #0072b2, 0.1
line-segment: (1,1), (4,1), solid, black, 2.5
line-segment: (4,1), (4,4), solid, black, 2.5
line-segment: (4,4), (1,4), solid, black, 2.5
line-segment: (1,4), (1,1), solid, black, 2.5
line-segment: (1.5,1), (1.5,4), solid, black, 1
line-segment: (2,1), (2,4), solid, black, 1
line-segment: (2.5,1), (2.5,4), solid, black, 1
line-segment: (3,1), (3,4), solid, black, 1
line-segment: (3.5,1), (3.5,4), solid, black, 1
line-segment: (1,1.5), (4,1.5), solid, black, 1
line-segment: (1,2), (4,2), solid, black, 1
line-segment: (1,2.5), (4,2.5), solid, black, 1
line-segment: (1,3), (4,3), solid, black, 1
line-segment: (1,3.5), (4,3.5), solid, black, 1
fill-polygon: (1,1), (1.5,1), (1.5,1.5), (1,1.5), #0072b2, 0.3
line-segment: (0.85,1), (0.85,1.5), solid, #0072b2, 2
text: 0.2, 1.4, "$1$ cm", center, fontsize: 10
line-segment: (1,0.85), (1.5,0.85), solid, #0072b2, 2
text: 0.95, 0.8, "$1$ cm", center, fontsize: 10
text: 0.0, 2.5, "$s = 6$ cm", center, fontsize: 12
text: 2.0, 0.8, "$s = 6$ cm", center, fontsize: 12
text: 0.93, 1.4, "$1$cm$^2$", center, fontsize: 5
```

:::::::::::::::

::::{admonition} Løsning
---
class: solution
---

**Bruk av figuren:**
Figuren viser hvordan kvadratet med sidelengde 6 cm er delt inn i 36 små kvadrater. Hvert lite kvadrat representerer 1 cm² (1 kvadratcentimeter), slik figuren viser med den blåe firkanten.

- Siden kvadratet har **6 cm i lengden** (horisontalt), får vi **6 små kvadrater på tvers**
- Siden kvadratet har **6 cm i høyden** (vertikalt), får vi **6 små kvadrater opp**
- Totalt: **6 $\cdot$ 6 = 36 små kvadrater** = **36 cm²**

**Formelen og beregningen:**
Vi bruker formelen for arealet av et kvadrat:

$$
A = s \cdot s = s^2
$$

Når vi setter inn sidelengden $s = 6$ cm, får vi:

$$
A = 6 \text{ cm} \cdot 6 \text{ cm} = 36 \text{ cm}^2
$$

**Hvorfor blir enheten cm²:**
Når vi ganger en lengde målt i centimeter med en annen lengde målt i centimeter, får vi et areal målt i kvadratcentimeter. Vi ganger både **tallene** ($6 \cdot 6 = 36$) og **enhetene** ($\text{cm} \cdot \text{cm} = \text{cm}^2$).
::::

---

:::::{grid} 1 1 2 2
---
gutter: 1
---

::::{grid-item-card}
:header: Trekant
:class-header: sd-card-header
:class-body: sd-card-body
:class: summary-card

Arealet av en trekant med grunnflate $g$ og høyde $h$:

$$A = \frac{1}{2} \cdot g \cdot h$$

```{plot}
width: 90%
class: no-click, adaptive-figure
axis: off, equal
xmin: 0
xmax: 6
ymin: 0
ymax: 5
fontsize: 24
fill-polygon: (1,1), (5,1), (3,3.8), #0072b2, 0.1
line-segment: (1,1), (5,1), solid, black, 2.5
line-segment: (5,1), (3,3.8), solid, black, 2.5
line-segment: (3,3.8), (1,1), solid, black, 2.5
line-segment: (1,0.5), (5,0.5), solid, #0072b2, 1.5
text: 3, 0.15, "$g$", center
line-segment: (3,1), (3,3.8), dashed, #0072b2, 1.5
text: 2.5, 2.4, "$h$", center
```

::::

::::{grid-item-card}
:header: Parallellogram
:class-header: sd-card-header
:class-body: sd-card-body
:class: summary-card

Arealet av et parallellogram med grunnflate $g$ og høyde $h$:

$$A = g \cdot h$$

```{plot}
width: 90%
class: no-click, adaptive-figure
axis: off, equal
xmin: 0
xmax: 7
ymin: 0
ymax: 4
fontsize: 24
fill-polygon: (1,1), (5,1), (6,3), (2,3), #0072b2, 0.1
line-segment: (1,1), (5,1), solid, black, 2.5
line-segment: (5,1), (6,3), solid, black, 2.5
line-segment: (6,3), (2,3), solid, black, 2.5
line-segment: (2,3), (1,1), solid, black, 2.5
line-segment: (1,0.5), (5,0.5), solid, #0072b2, 1.5
text: 3, 0.15, "$g$", center
line-segment: (2,1), (2,3), dashed, #0072b2, 1.5
text: 1.5, 2, "$h$", center
```

::::

::::{grid-item-card}
:header: Trapes
:class-header: sd-card-header
:class-body: sd-card-body
:class: summary-card

Arealet av et trapes med parallelle sider $a$ og $b$, og høyde $h$:

$$A = \frac{a + b}{2} \cdot h$$

```{plot}
width: 90%
class: no-click, adaptive-figure
axis: off, equal
xmin: 0
xmax: 6
ymin: 0
ymax: 4.5
fontsize: 24
fill-polygon: (1,1), (5,1), (4,3), (2,3), #0072b2, 0.1
line-segment: (1,1), (5,1), solid, black, 2.5
line-segment: (5,1), (4,3), solid, black, 2.5
line-segment: (4,3), (2,3), solid, black, 2.5
line-segment: (2,3), (1,1), solid, black, 2.5
line-segment: (1,0.5), (5,0.5), solid, #0072b2, 1.5
text: 3, 0.15, "$b$", center
line-segment: (2,3.35), (4,3.35), solid, #0072b2, 1.5
text: 3, 3.9, "$a$", center
line-segment: (5.3,1), (5.3,3), solid, #0072b2, 1.5
text: 5.55, 2, "$h$", center
```

::::

::::{grid-item-card}
:header: Sirkel
:class-header: sd-card-header
:class-body: sd-card-body
:class: summary-card

Arealet av en sirkel med radius $r$:

$$A = \pi r^2$$

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
text: 3.75, 2.1, "$r$", #0072b2
```

::::

::::::

:::{explore} Fra sirkel til rektangel
Undersøk hvordan en sirkel kan omformes til et rektangel ved å dele sirkelens areal i flere og flere biter.

:::{raw} html
---
file: ./koder/areal_sirkel.html
---
:::
:::

::::{solution} Hvorfor er arealet av en sirkel πr²?

Når vi deler sirkelen i flere og flere biter og omformer dem, nærmer formen seg et rektangel. La oss forstå hvorfor dette gir oss formelen for arealet av en sirkel: $A = \pi r^2$.

**Omkrets av en sirkel:**
Omkretsen av en sirkel med radius $r$ er $O = 2\pi r$.

**Når vi deler sirkelen i mange biter:**
Hvis vi deler sirkelen i $n$ biter og legger dem ved siden av hverandre i en linje, blir den totale lengden av den øvre og nedre kanten sammen lik omkretsen:

$$\text{Bredde av rektangel} \approx \frac{O}{2} = \frac{2\pi r}{2} = \pi r$$

**Høyden av rektangelet:**
Når bitene står vertikalt fra en linje, strekker de seg fra sentrum av sirkelen til kanten, som er en lengde på $r$:

$$\text{Høyde av rektangel} = r$$

**Arealet av rektangelet:**
Siden arealet av et rektangel er bredde ganger høyde, får vi:

$$A = \text{bredde} \times \text{høyde} = \pi r \times r = \pi r^2$$

Når vi deler sirkelen i flere og flere biter (lar $n \to \infty$), blir omformingen eksakt, og vi får den nøyaktige formelen for arealet av en sirkel:

$$\boxed{A = \pi r^2}$$

::::

