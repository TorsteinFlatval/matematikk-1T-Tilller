# Oppgaver: Likningssystemer med programmering


:::::::::::::::{exercise} Oppgave 1
---
level: 1
---
Fyll inn koden slik at programmet finner løsningen på likningssystemet $x + y = 5$ og $x - y = 1$.

:::{interactive-code}
for x in range(-10, 11):
    for y in range(-10, 11):
        if ?????? and ??????:
            print((x, y))
:::

::::{answer}
Utskrift:

```text
(3, 2)
```
::::

::::{solution}
:::{code-block} python
for x in range(-10, 11):
    for y in range(-10, 11):
        if x + y == 5 and x - y == 1:
            print((x, y))
:::

Løsningen er $(x, y) = (3, 2)$.
::::
:::::::::::::::


:::::::::::::::{exercise} Oppgave 2
---
level: 1
---
Løs følgende likningssystemer ved å teste alle heltallsverdier:

::::::::::::::{tab-set}
---
class: tabs-parts
---
:::::::::::::{tab-item} a
Finn alle heltallsløsninger i intervallet [-10, 10] for systemet:

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
:::{code-block} python
for x in range(-10, 11):
    for y in range(-10, 11):
        if x + y == 2 and x - y == 6:
            print((x, y))
:::

Løsningen er $(4, -2)$.
::::
:::::::::::::

:::::::::::::{tab-item} b
Finn alle heltallsløsninger i intervallet [-10, 10] for systemet:

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
:::{code-block} python
for x in range(-10, 11):
    for y in range(-10, 11):
        if x**2 + y == 9 and x + y == 3:
            print((x, y))
:::

Løsningene er $(2, 1)$ og $(-3, 6)$.
::::
:::::::::::::

:::::::::::::{tab-item} c
Finn alle heltallsløsninger i intervallet [-15, 15] for systemet:

$$\begin{align}
2x - y &= 1 \\
x^2 + y &= 5
\end{align}$$

:::{interactive-code}
# Skriv koden din her
:::

::::{answer}
$$\mathcal{L} = \{(2, 3), (-1, -3)\}$$
::::

::::{solution}
:::{code-block} python
for x in range(-15, 16):
    for y in range(-15, 16):
        if 2*x - y == 1 and x**2 + y == 5:
            print((x, y))
:::

Løsningene er $(2, 3)$ og $(-1, -3)$.
::::
:::::::::::::

::::::::::::::

::::::::::::::::


:::::::::::::::{exercise} Oppgave 3
---
level: 2
---

::::::::::::::{tab-set}
---
class: tabs-parts
---
:::::::::::::{tab-item} a
La $f(x) = x$ og $g(x) = 2x - 3$. Finn alle løsninger der $f(x) = g(x)$ ved å teste verdier fra -10 til 10.

:::{interactive-code}
# Definer funksjonene og finn løsningene
:::

::::{answer}
$$\mathcal{L} = \{3\}$$
::::

::::{solution}
:::{code-block} python
def f(x):
    return x

def g(x):
    return 2*x - 3

for x in range(-10, 11):
    if f(x) == g(x):
        print(f"x = {x}: f({x}) = g({x}) = {f(x)}")
:::

Løsningen er $x = 3$ fordi $f(3) = 3$ og $g(3) = 2(3) - 3 = 3$.
::::
:::::::::::::

:::::::::::::{tab-item} b
La $f(x) = x^2$ og $g(x) = 2x$. Finn alle heltallsløsninger der $f(x) = g(x)$ ved å teste verdier fra -5 til 5.

:::{interactive-code}
# Definer funksjonene og finn løsningene
:::

::::{answer}
$$\mathcal{L} = \{0, 2\}$$
::::

::::{solution}
:::{code-block} python
def f(x):
    return x**2

def g(x):
    return 2*x

for x in range(-5, 6):
    if f(x) == g(x):
        print(f"x = {x}: f({x}) = g({x}) = {f(x)}")
:::

Løsningene er $x = 0$ og $x = 2$.
- For $x = 0$: $0^2 = 0$ og $2(0) = 0$
- For $x = 2$: $2^2 = 4$ og $2(2) = 4$
::::
:::::::::::::

:::::::::::::{tab-item} c
La $f(x) = x^2 + 1$ og $g(x) = 5$. Finn alle heltallsløsninger der $f(x) = g(x)$ ved å teste verdier fra -5 til 5.

:::{interactive-code}
# Definer funksjonene og finn løsningene
:::

::::{answer}
$$\mathcal{L} = \{-2, 2\}$$
::::

::::{solution}
:::{code-block} python
def f(x):
    return x**2 + 1

def g(x):
    return 5

for x in range(-5, 6):
    if f(x) == g(x):
        print(f"x = {x}: f({x}) = g({x}) = {f(x)}")
:::

Løsningene oppfyller $x^2 + 1 = 5$, som gir $x^2 = 4$. Løsningene er $x = -2$ og $x = 2$.
::::
:::::::::::::

::::::::::::::

::::::::::::::


:::::::::::::::{exercise} Oppgave 4
---
level: 2
---
Avanserte oppgaver med likningssystemer:

::::::::::::::{tab-set}
---
class: tabs-parts
---
:::::::::::::{tab-item} a
Finn alle heltallsløsninger i intervallet [-20, 20] for systemet:

$$\begin{align}
x^2 - y^2 &= 9 \\
x + y &= 3
\end{align}$$

:::{interactive-code}
# Skriv koden din her
:::

::::{answer}
$$\mathcal{L} = \{(3, 0), (0, 3)\}$$
::::

::::{solution}
:::{code-block} python
for x in range(-20, 21):
    for y in range(-20, 21):
        if x**2 - y**2 == 9 and x + y == 3:
            print((x, y))
:::

Løsningene er $(3, 0)$ og $(0, 3)$.
::::
:::::::::::::

:::::::::::::{tab-item} b
La $f(x) = x^3$ og $g(x) = 4x$. Finn alle heltallsløsninger der $f(x) = g(x)$ ved å teste verdier fra -3 til 3.

:::{interactive-code}
# Definer funksjonene og finn løsningene
:::

::::{answer}
$$\mathcal{L} = \{-2, 0, 2\}$$
::::

::::{solution}
:::{code-block} python
def f(x):
    return x**3

def g(x):
    return 4*x

for x in range(-3, 4):
    if f(x) == g(x):
        print(f"x = {x}: f({x}) = g({x}) = {f(x)}")
:::

Løsningene oppfyller $x^3 = 4x$, som gir $x^3 - 4x = 0$ eller $x(x^2 - 4) = 0$.
Løsningene er $x = -2$, $x = 0$, og $x = 2$.
::::
:::::::::::::

:::::::::::::{tab-item} c
La $f(x) = x^2 - 3$ og $g(x) = x$. Finn alle løsninger der $f(x) = g(x)$ ved å teste verdier fra -5 til 5.

:::{interactive-code}
# Definer funksjonene og finn løsningene
:::

::::{answer}
$$\mathcal{L} = \{-1, 3\}$$
::::

::::{solution}
:::{code-block} python
def f(x):
    return x**2 - 3

def g(x):
    return x

for x in range(-5, 6):
    if f(x) == g(x):
        print(f"x = {x}: f({x}) = g({x}) = {f(x)}")
:::

Løsningene oppfyller $x^2 - 3 = x$, som gir $x^2 - x - 3 = 0$. Med heltallstesting finner vi $x = -1$ og $x = 3$.
::::
:::::::::::::

::::::::::::::
