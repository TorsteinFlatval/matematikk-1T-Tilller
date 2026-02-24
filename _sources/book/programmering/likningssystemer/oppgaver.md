# Oppgaver

## Oppgave 1
Bruk to for-løkker til å finne alle heltallsløsninger i intervallet [-10, 10] for systemet

\begin{align*}
    x + y &= 2 \\
    x - y &= 6
\end{align*}

:::{interactive-code}
# Skriv koden din her
:::

::::{answer}
$$
\mathcal{L} = \{(4, -2)\}
$$
::::

::::{solution}
Vi tester alle punkt i intervallet og skriver ut løsningene:

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

Dermed er løsningen

$$
\mathcal{L} = \{(4, -2)\}
$$

::::

---

## Oppgave 2
Finn alle heltallsløsninger i intervallet [-10, 10] for systemet

\begin{align*}
    x^2 + y &= 9 \\
    x + y &= 3
\end{align*}

:::{interactive-code}
# Skriv koden din her
:::

::::{answer}
$$
\mathcal{L} = \{(2, 1), (-3, 6)\}
$$
::::

::::{solution}
Vi bruker to for-løkker og tester begge likningene samtidig:

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

Dermed er løsningene

$$
\mathcal{L} = \{(2, 1), (-3, 6)\}
$$

::::

---

## Oppgave 3
Finn alle heltallsløsninger i intervallet [-15, 15] for systemet

\begin{align*}
    2x - y &= 1 \\
    x^2 + y &= 5
\end{align*}

:::{interactive-code}
# Skriv koden din her
:::

::::{answer}
$$
\mathcal{L} = \{(2, 3), (-1, -3)\}
$$
::::

::::{solution}
Vi tester alle punkt og skriver ut de som passer:

:::{code-block} python
for x in range(-15, 16):
    for y in range(-15, 16):
        if 2*x - y == 1 and x**2 + y == 5:
            print((x, y))
:::

Utskriften blir:

:::{code-block} console
(2, 3)
(-1, -3)
:::

Dermed er løsningene

$$
\mathcal{L} = \{(2, 3), (-1, -3)\}
$$

::::

---

## Oppgave 4
Lag et program som finner alle heltallsløsninger i intervallet [-20, 20] for systemet

\begin{align*}
    x^2 - y^2 &= 9 \\
    x + y &= 3
\end{align*}

:::{interactive-code}
# Skriv koden din her
:::

::::{answer}
$$
\mathcal{L} = \{(3, 0), (0, 3)\}
$$
::::

::::{solution}
Vi tester alle punkt og skriver ut løsningene:

:::{code-block} python
for x in range(-20, 21):
    for y in range(-20, 21):
        if x**2 - y**2 == 9 and x + y == 3:
            print((x, y))
:::

Utskriften blir:

:::{code-block} console
(3, 0)
(0, 3)
:::

Dermed er løsningene

$$
\mathcal{L} = \{(3, 0), (0, 3)\}
$$

::::
