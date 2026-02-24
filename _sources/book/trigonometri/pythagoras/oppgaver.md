# Oppgaver

## Pytagoras' setning

:::::::::::::::{exercise} Oppgave 1
---
level: 1
---

Bestem $x$ i trekanten nedenfor.

:::{figure} ./figurer/underveisoppgaver/figur.svg
---
width: 60%
class: no-click, adaptive-figure
---
:::

:::{answer}
$$
x = 6
$$
:::

::::{solution}

Vi bruker Pytagoras' setning:

$$
a^2 = b^2 + c^2
$$

Der $a$ er hypotenusen. Fra figuren kan vi se at vi har en rettvinklet trekant med kjente sidelengder.

**Algebraisk manipulasjon:**

Setter inn de kjente verdiene i Pytagoras' setning:

$$
x^2 = 3^2 + 4^2
$$

Beregner kvadratene:

$$
x^2 = 9 + 16
$$

Adderer på høyre side:

$$
x^2 = 25
$$

Tar kvadratroten av begge sider:

$$
x = \sqrt{25} = 6
$$

Løsningen er:

$$
x = 6
$$

::::

:::::::::::::::

---

:::::::::::::::{exercise} Oppgave 2
---
level: 1
---

Nedenfor vises en rettvinklet trekant.

:::{figure} ./figurer/oppgaver/oppgave_2/figur.svg
---
width: 70%
class: no-click, adaptive-figure
---
:::

::::::::::::::{tab-set}
---
class: tabs-parts
---
:::::::::::::{tab-item} a
Bestem $x$.

:::{answer}
$$
x = 5 \sqrt{3}.
$$
:::

::::{solution}
Metode 1:

Vi bruker Pytagoras' læresetning:
$$
a^2 + b^2 = c^2
$$

Metode 2:

I en $30^\circ-60^\circ-90^\circ$-trekant er hypotenusen dobbelt så lang som den korteste kateten. Siden den korteste kateten er $5$, må hypotenusen være $10$.
::::

:::::::::::::

:::::::::::::{tab-item} b
Bruk CAS-vinduet til å bestemme $x$.
:::{cas-popup} 400 500
:::

:::{answer}
$$
x = 5 \sqrt{3}.
$$
:::

::::{solution}
<!-- Løsning for b) is temporarily empty -->
::::

:::::::::::::

:::::::::::::::

---

:::::::::::::::{exercise} Oppgave 3
---
level: 1
---

En stige på 5 meter lener seg inntil et tre. Bunnen av stigen er plassert 1,5 meter fra trestammen på flat mark. Vi antar at treet står vinkelrett på bakken.

Se figuren nedenfor.

:::{figure} ./figurer/oppgaver/oppgave_3/figur.svg
---
width: 60%
class: no-click, adaptive-figure
---
:::

::::::::::::::{tab-set}
---
class: tabs-parts
---
:::::::::::::{tab-item} a
Hvor høyt opp på treet når stigen? Bestem høyden $h$.

:::{answer}
$$
h \approx 4,77 \text{ m}.
$$
:::

::::{solution}
Siden treet står vinkelrett på bakken, danner stigen, bakken og treet en rettvinklet trekant.
* Hypotenusen er stigen: $c = 5$ m.
* Den ene kateten er avstanden langs bakken: $a = 1,5$ m.
* Den andre kateten er høyden opp på treet: $b = h$.

Vi bruker Pytagoras' læresetning ($a^2 + b^2 = c^2$) og setter inn tallene:

$$
\begin{aligned}
1,5^2 + h^2 &= 5^2 \\
2,25 + h^2 &= 25 \\
h^2 &= 25 - 2,25 \\
h^2 &= 22,75 \\
h &= \sqrt{22,75} \\
h &\approx 4,77
\end{aligned}
$$

Siden høyden må være positiv, forkaster vi den negative løsningen.
Stigen når ca. 4,77 meter opp på treet.
::::

:::::::::::::

:::::::::::::{tab-item} b
Hvor høyt opp på treet når stigen? Bruk CAS til å bestemme høyden $h$.
:::{cas-popup} 400 500
:::

:::{answer}
$$
h \approx 4,77 \text{ m}.
$$
:::

::::{solution}
<!-- Løsning for b) is temporarily empty -->
::::

:::::::::::::

:::::::::::::::

---

