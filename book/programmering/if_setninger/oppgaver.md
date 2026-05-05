# Oppgaver: if - else setninger

:::::::::::::::{exercise} Oppgave 1
---
level: 1
---
Ta quizen! 

:::{quiz}
Q: Hva blir skrevet ut av programmet? <pre><code class="python">x = 10\nif x > 5:\n    print("x er større enn 5")\nelse:\n    print("x er ikke større enn 5")</code></pre>
+ x er større enn 5
- x er ikke større enn 5
- Begge blir skrevet ut
- Ingenting blir skrevet ut

Q: Hva blir skrevet ut av programmet? <pre><code class="python">x = 3\nif x > 5:\n    print("x er større enn 5")\nelse:\n    print("x er ikke større enn 5")</code></pre>
+ x er ikke større enn 5
- x er større enn 5
- Begge blir skrevet ut
- Ingenting blir skrevet ut

Q: Hva blir skrevet ut av programmet? <pre><code class="python">tall = 7\nif tall == 7:\n    print("Tallet er 7")\nelse:\n    print("Tallet er ikke 7")</code></pre>
+ Tallet er 7
- Tallet er ikke 7
- Begge blir skrevet ut
- Ingenting blir skrevet ut

Q: Hva blir skrevet ut av programmet? <pre><code class="python">alder = 16\nif alder >= 18:\n    print("Du er myndig")\nelse:\n    print("Du er ikke myndig")</code></pre>
+ Du er ikke myndig
- Du er myndig
- Begge blir skrevet ut
- Ingenting blir skrevet ut

Q: Hva blir skrevet ut av programmet? <pre><code class="python">x = 5\nif x != 5:\n    print("x er ikke 5")\nelse:\n    print("x er 5")</code></pre>
+ x er 5
- x er ikke 5
- Begge blir skrevet ut
- Ingenting blir skrevet ut

Q: Hva blir skrevet ut av programmet? <pre><code class="python">tall = -3\nif tall < 0:\n    print("Tallet er negativt")\nelse:\n    print("Tallet er ikke negativt")</code></pre>
+ Tallet er negativt
- Tallet er ikke negativt
- Begge blir skrevet ut
- Ingenting blir skrevet ut
:::
:::::::::::::::

---

:::::::::::::::{exercise} Oppgave 2
---
level: 1
---
Nedenfor vises noen programkoder med if-else-setninger. Les programmene og prøv å forutsi hva som blir skrevet ut. 

Skriv inn gjetningen din og sjekk svaret ditt for hvert av programmene.

::::::::::::::{tab-set}
---
class: tabs-parts
---
:::::::::::::{tab-item} a

:::{interactive-code}
---
predict:
---
x = 8
if x > 10:
    print("x er større enn 10")
else:
    print("x er ikke større enn 10")
:::

:::::::::::::

:::::::::::::{tab-item} b

:::{interactive-code}
---
predict:
---
navn = "Alice"
if navn == "Bob":
    print("Hallo Bob")
else:
    print("Du er ikke Bob")
:::

:::::::::::::

:::::::::::::{tab-item} c

:::{interactive-code}
---
predict:
---
tall = 15
if tall <= 10:
    print("Tallet er 10 eller mindre")
else:
    print("Tallet er større enn 10")
:::

:::::::::::::

:::::::::::::{tab-item} d

:::{interactive-code}
---
predict:
---
alder = 25
if alder < 18:
    print("Du er barn")
else:
    print("Du er voksen")
:::

:::::::::::::

::::::::::::::

:::::::::::::::

---

:::::::::::::::{exercise} Oppgave 3
---
level: 1
---
::::::::::::::{tab-set}
---
class: tabs-parts
---
:::::::::::::{tab-item} a
Fyll ut programmet nedenfor slik at det skriver ut "Tallet er positivt" dersom `x` er større enn 0, ellers skal det skrive ut "Tallet er ikke positivt".

:::{interactive-code}
x = 5
if ????:  # FYLL INN: bytt ut ????
    print("Tallet er positivt")
else:
    print("Tallet er ikke positivt")
:::

::::{answer}
Utskrift:

```text
Tallet er positivt
```
::::

::::{solution}
:::{code-block} python
---
linenos:
---
x = 5
if x > 0:
    print("Tallet er positivt")
else:
    print("Tallet er ikke positivt")
:::
::::

:::::::::::::

:::::::::::::{tab-item} b
Fyll ut programmet nedenfor slik at det skriver ut "Du kan stemme" dersom alderen er 18 eller mer, ellers skal det skrive ut "Du kan ikke stemme".

:::{interactive-code}
alder = 20
if ????:  # FYLL INN: bytt ut ????
    print("Du kan stemme")
else:
    print("Du kan ikke stemme")
:::

::::{answer}
Utskrift:

```text
Du kan stemme
```
::::

::::{solution}
:::{code-block} python
---
linenos:
---
alder = 20
if alder >= 18:
    print("Du kan stemme")
else:
    print("Du kan ikke stemme")
:::
::::

:::::::::::::

:::::::::::::{tab-item} c
Fyll ut programmet nedenfor slik at det sjekker om tallet er partall eller oddetall.

:::{interactive-code}
tall = 4
if ????:  # FYLL INN: bytt ut ????
    print("Tallet er partall")
else:
    print("Tallet er oddetall")
:::

::::{answer}
Utskrift:

```text
Tallet er partall
```
::::

::::{solution}
:::{code-block} python
---
linenos:
---
tall = 4
if tall % 2 == 0:
    print("Tallet er partall")
else:
    print("Tallet er oddetall")
:::
::::

:::::::::::::

:::::::::::::{tab-item} d
Fyll ut programmet nedenfor slik at det sjekker om ordet er "Python", og skriver ut riktig melding.

:::{interactive-code}
ord = "Python"
if ????:  # FYLL INN: bytt ut ????
    print("Det er Python!")
else:
    print("Det er ikke Python")
:::

::::{answer}
Utskrift:

```text
Det er Python!
```
::::

::::{solution}
:::{code-block} python
---
linenos:
---
ord = "Python"
if ord == "Python":
    print("Det er Python!")
else:
    print("Det er ikke Python")
:::
::::

:::::::::::::

::::::::::::::

:::::::::::::::

---

:::::::::::::::{exercise} Oppgave 4
---
level: 2
---
::::::::::::::{tab-set}
---
class: tabs-parts
---
:::::::::::::{tab-item} a
Skriv et fullstendig program som sjekker om et tall `x` er mindre enn 100. Dersom det er det, skal det skrive ut "Tallet er mindre enn 100", ellers "Tallet er 100 eller større".

:::{interactive-code}
x = 50
# FYLL INN: skriv hele programmet
:::

:::::{answer}
Utskrift:

```text
Tallet er mindre enn 100
```
:::::

:::::{solution}
:::{code-block} python
---
linenos:
---
x = 50
if x < 100:
    print("Tallet er mindre enn 100")
else:
    print("Tallet er 100 eller større")
:::
:::::

:::::::::::::

:::::::::::::{tab-item} b
Skriv et program som sjekker om lengden av strengen `tekst` er større enn 5 tegn. Hvis den er lengre, skal det skrive ut "Teksten er lang", ellers "Teksten er kort".

:::{interactive-code}
tekst = "Hello"
# FYLL INN: skriv hele programmet
:::

:::::{answer}
Utskrift:

```text
Teksten er kort
```
:::::

:::::{solution}
:::{code-block} python
---
linenos:
---
tekst = "Hello"
if len(tekst) > 5:
    print("Teksten er lang")
else:
    print("Teksten er kort")
:::
:::::

:::::::::::::

:::::::::::::{tab-item} c
Skriv et program som sjekker om tallet `x` ligger mellom 0 og 10 (inkludert). Hvis det gjør det, skal det skrive ut "Tallet er mellom 0 og 10", ellers "Tallet er ikke mellom 0 og 10".

**Hint:** Du trenger å sjekke to betingelser med `and`.

:::{interactive-code}
x = 7
# FYLL INN: skriv hele programmet
:::

:::::{answer}
Utskrift:

```text
Tallet er mellom 0 og 10
```
:::::

:::::{solution}
:::{code-block} python
---
linenos:
---
x = 7
if x >= 0 and x <= 10:
    print("Tallet er mellom 0 og 10")
else:
    print("Tallet er ikke mellom 0 og 10")
:::
:::::

:::::::::::::

::::::::::::::

:::::::::::::::

