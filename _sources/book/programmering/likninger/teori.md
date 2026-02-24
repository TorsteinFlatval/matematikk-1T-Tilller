# Likninger med programmering


:::{goals} Læringsmål
* Forstå hvordan for-løkker fungerer i Python
* Kunne bruke programmering til å løse likninger
* Kunne systematisk teste ulike verdier i en likning
:::

I dette kapittelet skal vi lære å løse likninger ved hjelp av programmering. Vi starter helt fra scratch og bygger opp forståelsen steg for steg.


## Introduksjon til for-løkker

En for-løkke i Python lar oss gjenta en handling flere ganger. Dette er veldig nyttig når vi skal teste mange verdier.

La oss se på et enkelt eksempel:

:::::::::::::::{example} Eksempel 1
Programmet nedenfor viser en for-løkke fra 0 til 4.

:::{interactive-code}
for x in range(5):
    print(x)
:::

::::{solution}
---
dropdown: 0
---

Programmet bruker en for-løkke som går gjennom tallene fra 0 til 4 (totalt 5 tall). For hver verdi av `x` skriver programmet ut verdien.

Utskriften blir:

:::{code-block} console
0
1
2
3
4
:::

Legg merke til at `range(5)` gir oss tallene fra 0 til 4, ikke til og med 5!

::::

:::::::::::::::

---

:::::::::::::::{example} Eksempel 2
Programmet nedenfor viser en for-løkke fra 1 til 4.

:::{interactive-code}
for x in range(1, 5):
    print(x)
:::

::::{solution}
---
dropdown: 0
---

Nå starter vi på 1 og slutter på 5 (ikke inkludert). For-løkken går altså gjennom tallene 1, 2, 3, 4.

Utskriften blir:

:::{code-block} console
1
2
3
4
:::

::::

:::::::::::::::

---

:::::::::::::::{exercise} Underveisoppgave 1
Hva skriver programmet nedenfor ut?

:::{interactive-code}
for x in range(-2, 3):
    print(x)
:::

::::{answer}
:::{code-block} console
-2
-1
0
1
2
:::
::::

::::{solution}
For-løkken går gjennom tallene fra -2 til 2 (ikke inkludert 3).

Utskriften blir:

:::{code-block} console
-2
-1
0
1
2
:::
::::

:::::::::::::::


## Teste verdier i en likning

Nå som vi kan lage for-løkker, kan vi bruke dem til å teste om ulike verdier oppfyller en likning.

La oss si at vi vil løse likningen $2x + 3 = 11$.

Vi kan teste om en $x$-verdi er løsning ved å sjekke om venstresiden blir lik høyresiden.

:::::::::::::::{example} Eksempel 3
Programmet nedenfor tester om $x = 4$ er løsning på likningen $2x + 3 = 11$.

:::{interactive-code}
x = 4
if 2*x + 3 == 11:
    print("x =", x, "er en løsning!")
:::

::::{solution}
---
dropdown: 0
---

Vi setter `x = 4` og regner ut venstresiden: `2*x + 3 = 2*4 + 3 = 11`.

Siden venstresiden er lik 11 (som er høyresiden), er betingelsen `2*x + 3 == 11` sann.

Derfor skrives meldingen ut:

:::{code-block} console
x = 4 er en løsning!
:::

::::

:::::::::::::::

---

Legg merke til at vi bruker to likhetstegn `==` for å sjekke om to verdier er like. Ett likhetstegn `=` brukes for å sette en verdi.

:::::::::::::::{example} Eksempel 4
Programmet nedenfor tester om $x = 3$ er en løsning på likningen $2x + 3 = 11$.

:::{interactive-code}
x = 3
if 2*x + 3 == 11:
    print("x =", x, "er en løsning!")
:::

::::{solution}
---
dropdown: 0
---

Nå tester vi $x = 3$: `2*3 + 3 = 9`, som ikke er lik 11.

Derfor skjer ingenting - programmet skriver ikke ut noe.

Utskriften:
:::{code-block} console

:::

(tomt)

::::

:::::::::::::::

---

:::::::::::::::{exercise} Underveisoppgave 2
Endre programmet nedenfor slik at det tester om $x = 5$ er en løsning på likningen $3x - 2 = 13$.

:::{interactive-code}
x = 4
if 2*x + 3 == 11:
    print("x =", x, "er en løsning!")
:::

::::{answer}
:::{code-block} console
x = 5 er en løsning!
:::
::::

::::{solution}
Vi endrer verdien av `x` til 5 og bruker likningen $3x - 2 = 13$:

:::{code-block} python
x = 5
if 3*x - 2 == 13:
    print("x =", x, "er en løsning!")
:::

Siden $3 \cdot 5 - 2 = 15 - 2 = 13$, er $x = 5$ en løsning.

::::

:::::::::::::::


## Løse likninger ved å teste verdier

Nå kombinerer vi for-løkker og if-setninger for å finne løsninger på likninger!

:::::::::::::::{example} Eksempel 5
Programmet nedenfor finner løsningen på likningen $2x + 3 = 11$ ved å teste alle verdiene fra 0 til 10.

:::{interactive-code}
for x in range(11):
    if 2*x + 3 == 11:
        print("x =", x, "er en løsning!")
:::

::::{solution}
---
dropdown: 0
---

For-løkken går gjennom alle verdiene fra 0 til 10. For hver verdi sjekker vi om den oppfyller likningen.

Kun når $x = 4$ er venstresiden lik høyresiden, så programmet skriver ut:

:::{code-block} console
x = 4 er en løsning!
:::

::::

:::::::::::::::

---

:::::::::::::::{example} Eksempel 6
Programmet nedenfor løser likningen $x^2 = 16$ ved å teste verdier fra -10 til 10.

:::{interactive-code}
for x in range(-10, 11):
    if x**2 == 16:
        print("x =", x, "er en løsning!")
:::

::::{solution}
---
dropdown: 0
---

For-løkken tester alle verdiene fra -10 til 10. Likningen $x^2 = 16$ har to løsninger: $x = -4$ og $x = 4$.

Utskriften blir:

:::{code-block} console
x = -4 er en løsning!
x = 4 er en løsning!
:::

::::

:::::::::::::::

---

:::::::::::::::{exercise} Underveisoppgave 3
Finn løsningen på likningen $3x - 5 = 10$ ved å teste verdier fra 0 til 10.

:::{interactive-code}
# Skriv koden din her
:::

::::{answer}
:::{code-block} console
x = 5 er en løsning!
:::
::::

::::{solution}
Vi bruker en for-løkke som tester verdier fra 0 til 10:

:::{code-block} python
for x in range(11):
    if 3*x - 5 == 10:
        print("x =", x, "er en løsning!")
:::

Løsningen er $x = 5$ fordi $3 \cdot 5 - 5 = 15 - 5 = 10$.

::::

:::::::::::::::


## Ikke-lineære likninger

Metoden fungerer også for mer komplekse likninger!

:::::::::::::::{example} Eksempel 7
Programmet nedenfor løser likningen $x^2 - 3x - 10 = 0$ ved å teste verdier fra -10 til 10.

:::{interactive-code}
for x in range(-10, 11):
    if x**2 - 3*x - 10 == 0:
        print("x =", x, "er en løsning!")
:::

::::{solution}
---
dropdown: 0
---

For-løkken tester alle verdiene fra -10 til 10. Likningen har to løsninger: $x = -2$ og $x = 5$.

La oss sjekke:
- For $x = -2$: $(-2)^2 - 3(-2) - 10 = 4 + 6 - 10 = 0$ ✓
- For $x = 5$: $5^2 - 3(5) - 10 = 25 - 15 - 10 = 0$ ✓

Utskriften blir:

:::{code-block} console
x = -2 er en løsning!
x = 5 er en løsning!
:::

::::

:::::::::::::::

---

:::::::::::::::{example} Eksempel 8
Noen likninger har ingen løsninger blant heltallene. Programmet nedenfor tester likningen $2x - 1 = 0$.

:::{interactive-code}
for x in range(-10, 11):
    if 2*x - 1 == 0:
        print("x =", x, "er en løsning!")
:::

Vi kan i stedet teste desimalverdier ved å gå i steg på 0.1. Dette er samme idé som `for x in range(-10, 10, 0.1)`, men `range` tar bare heltall, så vi skalerer først og deler etterpå:

:::{code-block} python
for i in range(-100, 101):
    x = i / 10
    if 2*x - 1 == 0:
        print("x =", x, "er en løsning!")
:::

Utskriften blir:

:::{code-block} console
x = 0.5 er en løsning!
:::

::::{solution}
---
dropdown: 0
---

Likningen $2x - 1 = 0$ har løsningen $x = \frac{1}{2}$, som ikke er et heltall.

Derfor vil programmet ikke finne noen løsning når vi bare tester heltall:

:::{code-block} console

:::

(tomt - ingen løsninger funnet)

::::

:::::::::::::::

---

:::::::::::::::{exercise} Underveisoppgave 4
Løs likningen $x^2 + x - 12 = 0$ ved å teste verdier fra -10 til 10.

:::{interactive-code}
# Skriv koden din her
:::

::::{answer}
$$
\mathcal{L} = \{-4, 3\}
$$
::::

::::{solution}
Vi bruker en for-løkke som tester verdier fra -10 til 10:

:::{code-block} python
for x in range(-10, 11):
    if x**2 + x - 12 == 0:
        print("x =", x, "er en løsning!")
:::

Utskriften blir:

:::{code-block} console
x = -4 er en løsning!
x = 3 er en løsning!
:::

Løsningen av likningen er derfor:

$$
\mathcal{L} = \{-4, 3\}
$$

Vi kan sjekke:
- For $x = -4$: $(-4)^2 + (-4) - 12 = 16 - 4 - 12 = 0$ ✓
- For $x = 3$: $3^2 + 3 - 12 = 9 + 3 - 12 = 0$ ✓

::::

:::::::::::::::



## Oppsummering

I dette kapittelet har vi lært:

1. **For-løkker**: Hvordan vi kan gjenta en handling flere ganger
   - `range(5)` gir tallene 0, 1, 2, 3, 4
   - `range(1, 5)` gir tallene 1, 2, 3, 4
   - `range(-2, 3)` gir tallene -2, -1, 0, 1, 2

2. **If-setninger**: Hvordan vi kan sjekke om noe er sant
   - `==` brukes for å sjekke om to verdier er like
   - `=` brukes for å sette en verdi

3. **Løse likninger**: Kombinere for-løkker og if-setninger
   - Teste systematisk ulike verdier
   - Finne alle løsninger i et gitt intervall


Denne metoden fungerer best når vi leter etter heltallsløsninger. For mer presise løsninger kan vi bruke andre metoder som CAS eller algebraiske metoder.
