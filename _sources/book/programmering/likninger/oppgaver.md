# Oppgaver

## Oppgave 1
Hva skriver programmet nedenfor ut?

:::{interactive-code}
---
predict:
---
for x in range(3, 8):
    print(x)

::::

::::{answer}
:::{code-block} console
3
4
5
6
7
:::
::::

::::{solution}
For-løkken går gjennom tallene fra 3 til 7 (ikke inkludert 8).

Utskriften blir:

:::{code-block} console
3
4
5
6
7
:::
::::

---

## Oppgave 2
Skriv et program som tester om $x = 7$ er en løsning på likningen $4x - 5 = 23$.

:::{interactive-code}
# Skriv koden din her
:::

::::{answer}
:::{code-block} console
x = 7 er en løsning!
:::
::::

::::{solution}
Vi setter `x = 7` og sjekker om $4x - 5 = 23$:

:::{code-block} python
x = 7
if 4*x - 5 == 23:
    print("x =", x, "er en løsning!")
:::

Siden $4 \cdot 7 - 5 = 28 - 5 = 23$, er $x = 7$ en løsning.

::::

---

## Oppgave 3
Finn løsningen på likningen $5x - 3 = 17$ ved å teste verdier fra 0 til 10.

:::{interactive-code}
# Skriv koden din her
:::

::::{answer}
$$
\mathcal{L} = \{4\}
$$
::::

::::{solution}
Vi bruker en for-løkke som tester verdier fra 0 til 10:

:::{code-block} python
for x in range(11):
    if 5*x - 3 == 17:
        print("x =", x, "er en løsning!")
:::

Utskriften blir:

:::{code-block} console
x = 4 er en løsning!
:::

Løsningen er $x = 4$ fordi $5 \cdot 4 - 3 = 20 - 3 = 17$.

$$
\mathcal{L} = \{4\}
$$

::::

---

## Oppgave 4
Finn alle løsninger på likningen $x^2 - 9 = 0$ ved å teste verdier fra -10 til 10.

:::{interactive-code}
# Skriv koden din her
:::

::::{answer}
$$
\mathcal{L} = \{-3, 3\}
$$
::::

::::{solution}
Vi bruker en for-løkke som tester verdier fra -10 til 10:

:::{code-block} python
for x in range(-10, 11):
    if x**2 - 9 == 0:
        print("x =", x, "er en løsning!")
:::

Utskriften blir:

:::{code-block} console
x = -3 er en løsning!
x = 3 er en løsning!
:::

Løsningen av likningen er derfor:

$$
\mathcal{L} = \{-3, 3\}
$$

Vi kan sjekke: $(-3)^2 - 9 = 9 - 9 = 0$ ✓ og $3^2 - 9 = 9 - 9 = 0$ ✓

::::

---

## Oppgave 5
Finn alle løsninger på likningen $x^2 + 2x - 8 = 0$ ved å teste verdier fra -10 til 10.

:::{interactive-code}
# Skriv koden din her
:::

::::{answer}
$$
\mathcal{L} = \{-4, 2\}
$$
::::

::::{solution}
Vi bruker en for-løkke som tester verdier fra -10 til 10:

:::{code-block} python
for x in range(-10, 11):
    if x**2 + 2*x - 8 == 0:
        print("x =", x, "er en løsning!")
:::

Utskriften blir:

:::{code-block} console
x = -4 er en løsning!
x = 2 er en løsning!
:::

Løsningen av likningen er derfor:

$$
\mathcal{L} = \{-4, 2\}
$$

Vi kan sjekke:
- For $x = -4$: $(-4)^2 + 2(-4) - 8 = 16 - 8 - 8 = 0$ ✓
- For $x = 2$: $2^2 + 2(2) - 8 = 4 + 4 - 8 = 0$ ✓

::::

---

## Oppgave 6
Finn alle løsninger på likningen $x^2 - 4x + 3 = 0$ og lagre dem i en liste.

:::{interactive-code}
# Skriv koden din her
:::

::::{answer}
$$
\mathcal{L} = \{1, 3\}
$$
::::

::::{solution}
Vi lager en tom liste og legger til løsninger vi finner:

:::{code-block} python
løsninger = []

for x in range(-10, 11):
    if x**2 - 4*x + 3 == 0:
        løsninger.append(x)

print("Løsningene er:", løsninger)
:::

Utskriften blir:

:::{code-block} console
Løsningene er: [1, 3]
:::

Løsningen av likningen er derfor:

$$
\mathcal{L} = \{1, 3\}
$$

::::

---

## Oppgave 7
Finn alle løsninger på likningen $2x^2 - 8 = 0$ ved å teste verdier fra -5 til 5.

:::{interactive-code}
# Skriv koden din her
:::

::::{answer}
$$
\mathcal{L} = \{-2, 2\}
$$
::::

::::{solution}
Vi bruker en for-løkke som tester verdier fra -5 til 5:

:::{code-block} python
for x in range(-5, 6):
    if 2*x**2 - 8 == 0:
        print("x =", x, "er en løsning!")
:::

Utskriften blir:

:::{code-block} console
x = -2 er en løsning!
x = 2 er en løsning!
:::

Løsningen av likningen er derfor:

$$
\mathcal{L} = \{-2, 2\}
$$

::::

---

## Oppgave 8
Finn alle løsninger på likningen $x^3 - 8 = 0$ ved å teste verdier fra -5 til 5.

:::{interactive-code}
# Skriv koden din her
:::

::::{answer}
$$
\mathcal{L} = \{2\}
$$
::::

::::{solution}
Vi bruker en for-løkke som tester verdier fra -5 til 5:

:::{code-block} python
for x in range(-5, 6):
    if x**3 - 8 == 0:
        print("x =", x, "er en løsning!")
:::

Utskriften blir:

:::{code-block} console
x = 2 er en løsning!
:::

Løsningen av likningen er derfor:

$$
\mathcal{L} = \{2\}
$$

Fordi $2^3 = 8$.

::::

---

## Oppgave 9
Finn alle løsninger på likningen $x^2 + 3x - 18 = 0$ og lagre dem i en liste.

:::{interactive-code}
# Skriv koden din her
:::

::::{answer}
$$
\mathcal{L} = \{-6, 3\}
$$
::::

::::{solution}
Vi lager en tom liste og legger til løsninger vi finner:

:::{code-block} python
løsninger = []

for x in range(-10, 11):
    if x**2 + 3*x - 18 == 0:
        løsninger.append(x)

print("Løsningene er:", løsninger)
:::

Utskriften blir:

:::{code-block} console
Løsningene er: [-6, 3]
:::

Løsningen av likningen er derfor:

$$
\mathcal{L} = \{-6, 3\}
$$

::::

---

## Oppgave 10
Noen likninger har ingen heltallsløsninger. Hva blir utskriften av programmet nedenfor?

:::{interactive-code}
---
predict:
---
for x in range(-10, 11):
    if x**2 + 1 == 0:
        print("x =", x, "er en løsning!")
:::

::::{answer}
:::{code-block} console

:::

(tomt - ingen løsninger funnet)

::::

::::{solution}
Likningen $x^2 + 1 = 0$ har ingen reelle løsninger, siden $x^2$ alltid er positiv eller null.

Derfor vil programmet ikke finne noen løsning:

:::{code-block} console

:::

(tomt - ingen løsninger funnet)

::::
