# Likningssystemer med programmering

:::::{admonition} Læringsmål
---
class: tip
---
* Forstå hvordan nestede `for`{l=python}-løkker fungerer
* Kunne bruke programmering til å løse likningssystemer med to ukjente
* Kunne bruke `and`{l=python} for å sjekke flere betingelser samtidig
* Kunne systematisk finne alle heltallsløsninger i et likningssystem
:::::

Et likningssystem har ofte to ukjente, $x$ og $y$. I programmering kan vi løse slike systemer ved å teste alle mulige par $(x, y)$ i et område og sjekke hvilke som oppfyller begge likningene samtidig.

## Nestede `for`{l=python}-løkker

For å teste alle par $(x, y)$ bruker vi to `for`{l=python}-løkker: en for $x$ og en for $y$. Den ene løkken nøstes (plasseres) inne i den andre.

:::::::::::::::{summary} Nestede `for`{l=python}-løkker
For å teste alle par $(x, y)$ bruker vi to `for`{l=python}-løkker:

:::{code-block} python
---
linenos:
---
for x in range(start, slutt):
    for y in range(start, slutt):
        # Kode som kjøres for hver kombinasjon av x og y
:::

Den ytre løkken itererer over $x$, og for hver $x$ itererer den indre løkken over alle $y$-verdier.
:::::::::::::::

:::::::::::::::{explore} Utforsk 1
La oss utforske hvordan nestede `for`{l=python}-løkker fungerer.

::::::::::::::{tab-set}
---
class: tabs-parts
---
:::::::::::::{tab-item} a
Hva tror du programmet skriver ut?

:::{interactive-code}
---
predict:
---
for x in range(1, 3):
    for y in range(1, 3):
        print((x, y))
:::
:::::::::::::

:::::::::::::{tab-item} b
Hva tror du programmet skriver ut?

:::{interactive-code}
---
predict:
---
for x in range(1, 4):
    for y in range(1, 3):
        print((x, y))
:::
:::::::::::::

:::::::::::::{tab-item} c
Hva tror du programmet skriver ut?

:::{interactive-code}
---
predict:
---
for x in range(0, 2):
    for y in range(0, 3):
        print((x, y))
:::
:::::::::::::

::::::::::::::

:::::::::::::::

---

## Sjekke flere betingelser samtidig

For å løse et likningssystem må begge likningene være oppfylt samtidig. Vi bruker `and`{l=python} for å sjekke flere betingelser i samme `if`{l=python}-setning.

:::::::::::::::{summary} `and`{l=python} - flere betingelser
Vi bruker `and`{l=python} når både betingelse 1 OG betingelse 2 må være sann:

:::{code-block} python
---
linenos:
---
if <betingelse_1> and <betingelse_2>:
    # Kode som kjøres hvis BEGGE betingelsene er sanne
:::

Hvis bare en av betingelsene er usann, kjøres koden ikke.
:::::::::::::::

:::::::::::::::{explore} Utforsk 2
La oss utforske hvordan `and`{l=python} fungerer når vi sjekker to betingelser.

::::::::::::::{tab-set}
---
class: tabs-parts
---
:::::::::::::{tab-item} a
Hva tror du programmet skriver ut når vi tester $(x, y) = (3, 2)$ mot systemet $x + y = 5$ og $x - y = 1$?

:::{interactive-code}
---
predict:
---
x = 3
y = 2
if x + y == 5 and x - y == 1:
    print("(", x, ",", y, ") er en løsning!")
:::
:::::::::::::

:::::::::::::{tab-item} b
Hva tror du programmet skriver ut når vi tester $(x, y) = (2, 2)$ mot systemet $x + y = 5$ og $x - y = 1$?

:::{interactive-code}
---
predict:
---
x = 2
y = 2
if x + y == 5 and x - y == 1:
    print("(", x, ",", y, ") er en løsning!")
:::
:::::::::::::

:::::::::::::{tab-item} c
Hva tror du programmet skriver ut når vi tester $(x, y) = (4, 2)$ mot systemet $x + y = 5$ og $x - y = 1$?

:::{interactive-code}
---
predict:
---
x = 4
y = 2
if x + y == 5 and x - y == 1:
    print("(", x, ",", y, ") er en løsning!")
:::
:::::::::::::

::::::::::::::

:::::::::::::::

---

## Løse likningssystemer

Nå kombinerer vi nestede `for`{l=python}-løkker og `and`{l=python} for å finne alle løsninger på et likningssystem.

:::::::::::::::{summary} Slik løser vi likningssystemer
For å finne løsninger på et likningssystem tester vi alle par $(x, y)$ i et område:

:::{code-block} python
---
linenos:
---
for x in range(start, slutt):
    for y in range(start, slutt):
        if <likning_1> and <likning_2>:
            print((x, y))
:::

Alle par som gjør begge likningene sanne blir skrevet ut.
:::::::::::::::

:::::::::::::::{example} Eksempel 1
La oss løse likningssystemet

$$\begin{align}
x + y &= 5 \\
x - y &= 1
\end{align}$$

ved å teste alle heltallsverdier fra -10 til 10.

:::{interactive-code}
for x in range(-10, 11):
    for y in range(-10, 11):
        if x + y == 5 and x - y == 1:
            print((x, y))
:::

::::{solution}
---
dropdown: 0
---

Vi tester alle par $(x, y)$. For hver kombinasjon sjekker vi om både $x + y = 5$ og $x - y = 1$ er sanne.

Bare paret $(3, 2)$ oppfyller begge likningene:
- $3 + 2 = 5$ ✓
- $3 - 2 = 1$ ✓

Utskriften blir:

:::{code-block} console
(3, 2)
:::

Løsningen er:

$$\mathcal{L} = \{(3, 2)\}$$

::::

:::::::::::::::

---

:::::::::::::::{example} Eksempel 2
La oss løse likningssystemet

$$\begin{align}
x^2 + y &= 7 \\
x - y &= -1
\end{align}$$

ved å teste alle heltallsverdier fra -10 til 10.

:::{interactive-code}
for x in range(-10, 11):
    for y in range(-10, 11):
        if x**2 + y == 7 and x - y == -1:
            print((x, y))
:::

::::{solution}
---
dropdown: 0
---

Fra likning 2: $y = x + 1$

Setter vi dette inn i likning 1: $x^2 + (x + 1) = 7$, som gir $x^2 + x - 6 = 0$.

Løsningen er $(2, 3)$:
- $2^2 + 3 = 4 + 3 = 7$ ✓
- $2 - 3 = -1$ ✓

Utskriften blir:

:::{code-block} console
(2, 3)
:::

Løsningen er:

$$\mathcal{L} = \{(2, 3)\}$$

::::

:::::::::::::::

---

:::::::::::::::{exercise} Underveisoppgave 1
Løs likningssystemet ved å teste verdier fra -10 til 10:

$$\begin{align}
x + 2y &= 4 \\
x - y &= 1
\end{align}$$

:::{interactive-code}
# Skriv koden din her
:::

::::{answer}
$$\mathcal{L} = \{(2, 1)\}$$
::::

::::{solution}
Vi tester alle par og skriver ut dem som passer:

:::{code-block} python
for x in range(-10, 11):
    for y in range(-10, 11):
        if x + 2*y == 4 and x - y == 1:
            print((x, y))
:::

Paret $(2, 1)$ oppfyller begge likningene:
- $2 + 2 \cdot 1 = 4$ ✓
- $2 - 1 = 1$ ✓

Utskriften blir:

:::{code-block} console
(2, 1)
:::

Løsningen er:

$$\mathcal{L} = \{(2, 1)\}$$

::::

:::::::::::::::

---

:::::::::::::::{exercise} Underveisoppgave 2
Løs likningssystemet ved å teste verdier fra -10 til 10:

$$\begin{align}
x + y &= 2 \\
x - y &= 6
\end{align}$$

:::{interactive-code}
# Skriv koden din her
:::

::::{answer}
$$\mathcal{L} = \{(4, -2)\}$$
::::

::::{solution}
Vi bruker nestede `for`{l=python}-løkker:

:::{code-block} python
for x in range(-10, 11):
    for y in range(-10, 11):
        if x + y == 2 and x - y == 6:
            print((x, y))
:::

Utskriften blir:

:::{code-block} console
(4, -2)
:::

Løsningen er:

$$\mathcal{L} = \{(4, -2)\}$$

::::

:::::::::::::::

---

:::::::::::::::{exercise} Underveisoppgave 3
Løs likningssystemet ved å teste verdier fra -10 til 10:

$$\begin{align}
x^2 + y &= 9 \\
x + y &= 3
\end{align}$$

:::{interactive-code}
# Skriv koden din her
:::

::::{answer}
$$\mathcal{L} = \{(2, 1), (-3, 6)\}$$
::::

::::{solution}
Vi tester begge likningene samtidig:

:::{code-block} python
for x in range(-10, 11):
    for y in range(-10, 11):
        if x**2 + y == 9 and x + y == 3:
            print((x, y))
:::

Utskriften blir:

:::{code-block} console
(2, 1)
(-3, 6)
:::

Løsningene er:

$$\mathcal{L} = \{(2, 1), (-3, 6)\}$$

::::

:::::::::::::::

---