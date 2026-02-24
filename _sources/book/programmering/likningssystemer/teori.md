# Likningssystemer med programmering


:::{goals} Læringsmål
* Forstå hvordan to for-løkker kan brukes til å teste punkt (x, y)
* Kunne bruke nestede for-løkker til å finne løsninger i et likningssystem
* Kunne avgrense søkeområdet for å finne alle heltallsløsninger
:::

## Dobbel for-løkke
Vi starter med en dobbel for-løkke som skriver ut alle punkt (x, y) i et lite område.

:::::::::::::::{example} Eksempel 0
Programmet nedenfor skriver ut alle par (x, y) der x går fra 1 til 3 og y går fra 1 til 2.

:::{interactive-code}
for x in range(1, 4):
    for y in range(1, 3):
        print((x, y))
:::

::::{solution}
---
dropdown: 0
---
Utskriften blir:

:::{code-block} console
(1, 1)
(1, 2)
(2, 1)
(2, 2)
(3, 1)
(3, 2)
:::

::::

:::::::::::::::

I dette kapittelet skal vi bruke programmering til å løse likningssystemer. Vi bruker to for-løkker, en for x og en for y, slik at vi kan teste mange punkt systematisk.

## Ideen
Et likningssystem har ofte to ukjente, x og y. Da kan vi teste alle heltallsverdier i et avgrenset område og sjekke om begge likningene er oppfylt samtidig.

:::::::::::::::{summary} Slik tester vi et punkt
Et punkt (x, y) er en løsning hvis både likning 1 og likning 2 er sanne.

:::{code-block} python
---
linenos:
---
for x in range(start, stopp):
    for y in range(start, stopp):
        if <likning_1> and <likning_2>:
            print((x, y))
:::
:::::::::::::::

## Eksempel 1
Vi løser systemet

\begin{align*}
    x + y &= 5 \\
    x - y &= 1
\end{align*}

:::::::::::::::{example} Eksempel 1
Programmet nedenfor tester alle heltallsverdier fra -10 til 10.

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
Vi tester alle punkt (x, y). Bare (3, 2) oppfyller begge likningene.

:::{code-block} console
(3, 2)
:::

Dermed er løsningen

$$
\mathcal{L} = \{(3, 2)\}
$$

::::

:::::::::::::::

---

## Eksempel 2
Vi løser systemet

\begin{align*}
    x^2 + y &= 7 \\
    x - y &= -1
\end{align*}

:::::::::::::::{example} Eksempel 2
Programmet nedenfor finner alle heltallsløsninger i intervallet [-10, 10].

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
Programmet finner punktet (2, 3).

:::{code-block} console
(2, 3)
:::

Dermed er løsningen

$$
\mathcal{L} = \{(2, 3)\}
$$

::::

:::::::::::::::

---

:::::::::::::::{exercise} Underveisoppgave 1
Bruk to for-løkker til å finne alle heltallsløsninger i intervallet [-10, 10] for systemet

\begin{align*}
    x + 2y &= 4 \\
    x - y &= 1
\end{align*}

:::{interactive-code}
# Skriv koden din her
:::

::::{answer}
$$
\mathcal{L} = \{(2, 1)\}
$$
::::

::::{solution}
Vi tester alle punkt og skriver ut dem som passer:

:::{code-block} python
for x in range(-10, 11):
    for y in range(-10, 11):
        if x + 2*y == 4 and x - y == 1:
            print((x, y))
:::

Utskriften blir:

:::{code-block} console
(2, 1)
:::

Dermed er løsningen

$$
\mathcal{L} = \{(2, 1)\}
$$

::::

:::::::::::::::

---

## Velg riktig søkeområde
Hvis vi velger for lite område, kan vi miste løsninger. Hvis vi velger for stort område, blir programmet tregere.

Et vanlig valg er fra -10 til 10, men du kan endre det hvis du forventer store tall.

:::::::::::::::{exercise} Underveisoppgave 2
Endre programmet slik at det søker i intervallet [-20, 20]. Finn alle heltallsløsninger til systemet

\begin{align*}
    x^2 - y &= 10 \\
    x + y &= 6
\end{align*}

:::{interactive-code}
# Skriv koden din her
:::

::::{answer}
$$
\mathcal{L} = \{(4, 2)\}
$$
::::

::::{solution}
Vi bruker to for-løkker og et større søkeområde:

:::{code-block} python
for x in range(-20, 21):
    for y in range(-20, 21):
        if x**2 - y == 10 and x + y == 6:
            print((x, y))
:::

Utskriften blir:

:::{code-block} console
(4, 2)
:::

Dermed er løsningen

$$
\mathcal{L} = \{(4, 2)\}
$$

::::

:::::::::::::::
