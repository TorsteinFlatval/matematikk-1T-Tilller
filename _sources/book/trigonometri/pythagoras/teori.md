# Pytagoras' setning

En **rettvinklet** trekant er en trekant der én av vinklene er $90 \degree$.
Pytagoras' setning er en setning som forteller oss hvordan sidene i en rettvinklet trekant henger sammen. 

:::::::::::::::{admonition} Pytagoras' setning
---
class: summary
---
For en rettvinklet trekant gjelder

$$
(\mathrm{hypotenus})^2 = (\mathrm{katet}_1)^2 + (\mathrm{katet}_2)^2
$$

Se figuren til venstre nedenfor.

:::{figure} ./figurer/teori/merged_figure.svg
---
width: 100%
class: no-click, adaptive-figure
---
:::

Typisk navnsettes sidene i en rettvinklet trekant slik at den motstående siden til hjørne $A$ kalles for $a$, den motstående siden til hjørne $B$ kalles for $b$ og den motstående siden til $C$ kalles for $c$. Se figuren til høyre ovenfor. 

Da kan vi skrive ned Pytagoras' setning ved

$$
a^2 = b^2 + c^2
$$

:::::::::::::::

---


:::::::::::::::{admonition} Underveisoppgave 1
---
class: check
---

Nedenfor vises en rettvinklet trekant der den ene kateten har lengde 4 og den andre kateten er 3.

:::{plot}
width: 45%
class: no-click, adaptive-figure
axis: off, equal
xmin: -0.8
xmax: 3.8
ymin: -0.8
ymax: 4.8
figsize: (5, 6)
fontsize: 24
fill-polygon: (0, 0), (3, 0), (0, 4), 0072b2, 0.1
line-segment: (0, 0), (3, 0), solid, black, 2
line-segment: (3, 0), (0, 4), solid, black, 2
line-segment: (0, 4), (0, 0), solid, black, 2
vline: 0.3, 0, 0.3, solid, black, 2
hline: 0.3, 0, 0.3, solid, black, 2
text: -0.4, -0.15, "$A$", center
text: 3.15, -0.15, "$B$", center
text: -0.2, 4.5, "$C$", center
text: 1.3, -0.25, "$3$", center
text: -0.4, 2, "$4$", center
text: 1.6, 2.2, "$x$", center
:::

Bestem hypotenusen $x$.

::::{admonition} Løsning
---
class: solution
---

Vi bruker Pytagoras' læresetning $a^2 + b^2 = c^2$ der $a$ og $b$ er katetene og $c$ er hypotenusen.
Her er den ene kateten $a = 3$ og den andre kateten $b = 4$. Den ukjente siden $x$ er:

$$
\begin{aligned}
3^2 + 4^2 &= x^2 \\
9 + 16 &= x^2 \\
25 &= x^2 \\
x &= \sqrt{25} \\
x &=  5
\end{aligned}
$$

:::{admonition} NB!
---
class: remark
---
Matematisk sett er løsningen av likningen $x^2 = 25$ både $x = 5$ og $x = -5$, fordi begge verdiene oppfyller likningen siden $(-5)^2 = 25$ og $5^2 = 25$.

Men siden $x$ representerer en lengde i trekanten, kan vi ikke ha negativ lengde. Derfor velger vi bare den positive løsningen: $x = 5$.
:::

::::

:::::::::::::::

---


---

:::::::::::::::{admonition} Utforsk 1
---
class: explore
---

:::{figure} ./Videoer/Pythagoras_1.gif
---
class: no-click, adaptive-figure
width: 80%
style: "background-color: black;"
---
:::

<br>

Nedenfor vises et CAS-vindu som løser likningene

\begin{align*}
    3^2 + 4^2 = c^2 \\
    30^2 + b^2 = 50^2
\end{align*}

:::{ggb} 600 300
---
material_id: kwevpver
toolbar: "true"
---
:::

<br>

Fra utskriften i **celle 1** og **celle 2**, kan vi lese av at løsningene er:

$ c = 5 $ og $b = 40$. Her også forkaster vi de negative løsningene for $b$ og $c$.

:::::::::::::::



:::::{admonition} Utforsk 2
---
class: explore
name: programmering-if-else-utforsk-1
---
Under vises et kort interaktivt program. 

Utforsk og kjør programmet, og forklar hva programmet gjør.

:::{raw} html
---
file: ./python/utforsk/utforsk_1.html
---
:::

:::::::::::::::{admonition} Underveisoppgave 2
---
class: check
---

Sorter stegene i riktig rekkefølge for å lage et program som beregner hypotenusen i en rettvinklet trekant der katetene er $5$ og $12$.

:::{parsons-puzzle}
a = 5
b = 12
c = sqrt(a**2 + b**2)
print(c)
:::

:::::::::::::::



