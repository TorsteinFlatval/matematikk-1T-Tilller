# Oppgaver


:::::::::::::::{admonition} Oppgave 1
---
class: check
---
Et kvadrat har sidelengde $6$ m.

Forklar hvordan vi får $\text{m}^2$ som enhet når vi regner ut arealet.

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
text: 2.5, 0.5, "$s = 6$ m", center
text: 3.5, 2.5, "$s = 6$ m", center
```

::::{admonition} Fasit
---
class: answer, dropdown
---
$$
A = 36 \text{ m}^2
$$
::::

::::{admonition} Løsning
---
class: solution, dropdown
---
Vi bruker formelen for arealet av et kvadrat:

$$
A = s \cdot s = s^2
$$

Når vi setter inn sidelengden $s = 6$ m, får vi:

$$
A = 6 \text{ m} \cdot 6 \text{ m} = 36 \text{ m} \cdot \text{m} = 36 \text{ m}^2
$$

Når vi ganger en lengde målt i meter med en annen lengde målt i meter, får vi et areal målt i kvadratmeter ($\text{m}^2$). Dette er fordi vi ganger både tallene ($6 \cdot 6 = 36$) og enhetene ($\text{m} \cdot \text{m} = \text{m}^2$).
::::

:::::::::::::::

:::::::::::::::{admonition} Oppgave 2
---
class: check
---
Et rektangel har bredde $8$ cm og høyde $5$ cm. 

Hva er arealet av rektangelet?

```{plot}
width: 50%
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
text: 3, 0.5, "$b = 8$ cm", center
text: 5.8, 2, "$h = 5$ cm", center
```

::::{admonition} Fasit
---
class: answer, dropdown
---
$$
A = 40 \text{ cm}^2
$$
::::

::::{admonition} Løsning
---
class: solution, dropdown
---
Vi bruker formelen for arealet av et rektangel:

$$
A = b \cdot h = 8 \cdot 5 = 40 \text{ cm}^2
$$
::::

:::::::::::::::

:::::::::::::::{admonition} Underveisoppgave 3
---
class: check
---
En trekant har grunnflate $12$ m og høyde $7$ m.

Hva er arealet av trekanten?

```{plot}
width: 60%
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
line-segment: (3,1), (3,3.8), dashed, black, 1.5
text: 3, 0.5, "$g = 12$ m", center
text: 2.1, 2.4, "$h = 7$ m", center
```

::::{admonition} Fasit
---
class: answer, dropdown
---
$$
A = 42 \text{ m}^2
$$
::::

::::{admonition} Løsning
---
class: solution, dropdown
---
Vi bruker formelen for arealet av en trekant:

$$
A = \frac{1}{2} \cdot g \cdot h = \frac{1}{2} \cdot 12 \cdot 7 = 42 \text{ m}^2
$$
::::

:::::::::::::::

:::::::::::::::{admonition} Oppgave 3
---
class: check
---
En sirkel har radius $4$ cm.

Hva er arealet av sirkelen? Bruk $\pi \approx 3{,}14$.

```{plot}
width: 50%
class: no-click, adaptive-figure
axis: off, equal
xmin: 0.5
xmax: 5.5
ymin: 0.5
ymax: 4.5
fontsize: 24
circle: (3,2.5), 1.5, solid, black, 2.5
line-segment: (3,2.5), (4.5,2.5), dashed, black, 1.5
text: 3.75, 2.8, "$r = 4$ cm", center
```

::::{admonition} Fasit
---
class: answer, dropdown
---
$$
A = 16\pi \approx 50{,}24 \text{ cm}^2
$$
::::

::::{admonition} Løsning
---
class: solution, dropdown
---
Vi bruker formelen for arealet av en sirkel:

$$
A = \pi r^2 = \pi \cdot 4^2 = 16\pi \approx 50{,}24 \text{ cm}^2
$$
::::

:::::::::::::::

:::::::::::::::{admonition} Underveisoppgave 5
---
class: check
---
Et trapes har parallelle sider $a = 6$ cm og $b = 10$ cm, og høyde $h = 4$ cm.

Hva er arealet av trapeset?

```{plot}
width: 60%
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
line-segment: (3,1), (3,3), dashed, black, 1.5
text: 3, 0.5, "$b = 10$ cm", center
text: 3, 3.5, "$a = 6$ cm", center
text: 3.5, 2, "$h = 4$ cm", center
```

::::{admonition} Fasit
---
class: answer, dropdown
---
$$
A = 32 \text{ cm}^2
$$
::::

::::{admonition} Løsning
---
class: solution, dropdown
---
Vi bruker formelen for arealet av et trapes:

$$
A = \frac{a + b}{2} \cdot h = \frac{6 + 10}{2} \cdot 4 = \frac{16}{2} \cdot 4 = 8 \cdot 4 = 32 \text{ cm}^2
$$
::::

:::::::::::::::
