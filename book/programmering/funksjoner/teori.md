# Funksjoner med programmering


:::{goals} Læringsmål
* Forstå hva en funksjon er og hvorfor vi bruker funksjoner
* Kunne definere egne funksjoner med `def`{l=python}
* Forstå hvordan vi bruker parametere til å gi funksjoner ulike verdier
* Forstå forskjellen på `print`{l=python} og `return`{l=python}
:::

I dette kapittelet skal vi lære å samle kode i funksjoner. En funksjon er en navngitt kodeblokk som utfører en bestemt oppgave. Dette er veldig nyttig når vi skal gjøre samme operasjon flere ganger.

## Definere en funksjon

Vi bruker nøkkelordet `def`{l=python} for å lage (definere) en funksjon i Python. 

:::::::::::::::{summary} Definere en funksjon
Vi definerer en funksjon slik:

:::{code-block} python
---
linenos:
---
def funksjonsnavn():
    # Kode som skal utføres
:::

For å bruke (kalle) funksjonen senere i programmet, skriver vi navnet etterfulgt av parenteser: `funksjonsnavn()`{l=python}.
:::::::::::::::

:::::::::::::::{example} Eksempel 1
Programmet nedenfor viser en enkel funksjon som skriver ut en hilsen.

:::{interactive-code}
def hils():
    print("Hei på deg!")

hils()
hils()
:::

::::{solution}
---
dropdown: 0
---

Programmet definerer først funksjonen `hils()`{l=python}. Deretter kaller vi funksjonen to ganger.

Utskriften blir:

:::{code-block} console
Hei på deg!
Hei på deg!
:::

::::

:::::::::::::::

---

:::::::::::::::{explore} Utforsk 1
Nedenfor vises et program som definerer og bruker en funksjon i en løkke.

::::::::::::::{tab-set}
---
class: tabs-parts
---
:::::::::::::{tab-item} a
Les programmet nedenfor og prøv å forutsi hva programmet skriver ut.

Skriv inn gjetningen din nedenfor og sjekk svaret ditt!

:::{interactive-code}
---
predict:
---
def si_hurra():
    print("Hurra!")

for i in range(3):
    si_hurra()
:::
:::::::::::::
::::::::::::::

:::::::::::::::

---

## Funksjoner med parametere

Ofte vil vi at funksjonen skal bruke noen verdier vi sender til den. Vi kaller disse verdiene for **parametere** eller **argumenter**.

:::::::::::::::{example} Eksempel 2
Programmet nedenfor viser en funksjon som tar imot et tall som parameter (argument) og regner ut arealet av et kvadrat.

:::{interactive-code}
def regn_ut_areal(side):
    areal = side * side
    print("Arealet er", areal)

regn_ut_areal(3)
regn_ut_areal(5)
:::

::::{solution}
---
dropdown: 0
---

Funksjonen `regn_ut_areal`{l=python} tar imot variabelen `side`{l=python}. Første gang kaller vi den med tallet `3`, og programmet hopper ned i funksjonen med `side = 3`. Andre gang er `side = 5`.

Utskriften blir:

:::{code-block} console
Arealet er 9
Arealet er 25
:::

::::

:::::::::::::::

---

## Returnere en verdi

Hittil har funksjonene våre bare brukt `print`{l=python} for å skrive ut tekst på skjermen. Ofte vil vi heller at funksjonen skal regne ut et svar og **sende svaret tilbake** til oss slik at vi kan bruke det videre i programmet. Da bruker vi nøkkelordet `return`{l=python}.

:::::::::::::::{summary} `return`{l=python}
En funksjon avsluttes når den kommer til en `return`{l=python}-setning. Verdien bak `return`{l=python} sendes tilbake til der funksjonen ble kalt.

:::{code-block} python
---
linenos:
---
def kvadrat(x):
    return x**2
    
svar = kvadrat(3) # svar får verdien 9
:::
:::::::::::::::

:::::::::::::::{explore} Utforsk 2
Prøv koden nedenfor! 
Hva skjer hvis du bytter ut `return areal` med `print(areal)` inne i funksjonen?
Når vi vil bruke svaret fra en funksjon videre (som å legge det sammen med noe annet), holder det ikke at funksjonen bare *printer* svaret. Funksjonen må **returnere** verdien til oss.


:::{interactive-code}
def areal_kvadrat(side):
    areal = side * side
    return areal

# Nå kan vi lagre svarene i variabler og bruke dem videre!
areal1 = areal_kvadrat(3)
areal2 = areal_kvadrat(4)

totalt_areal = areal1 + areal2
print("Det totale arealet er", totalt_areal)
:::

::::{solution}
---
dropdown: 0
---

I stedet for `print`{l=python} bruker funksjonen `return`{l=python}. Det gjør at vi kan lagre resultatet som kommer fra funksjonen, for eksempel i variablene `areal1`{l=python} og `areal2`{l=python}. Etterpå kan vi regne videre med dem!

Utskriften blir:

:::{code-block} console
Det totale arealet er 25
:::

::::

:::::::::::::::

---

:::{margin} `print`{l=python} med f-strenger
I koden bruker vi `f"f({x}) = {f_verdi}"`{l=python}. Dette kalles en **f-streng**. F-strengen lar oss sette verdier inn i teksten ved å bruke `{}`{l=python} for å erstate variabelverdier.
:::

:::::::::::::::{example} Eksempel 4
La oss lage en lineær funksjon $f(x) = 2x + 1$ og en kvadratisk funksjon $g(x) = x^2 - 3$. Så finner vi noen funksjonsværdier.

:::{interactive-code}
def f(x):
    return 2*x + 1

def g(x):
    return x**2 - 3

# Finn funksjonsværdier
x = 4
f_verdi = f(x)
g_verdi = g(x)

print(f"f({x}) = {f_verdi}")
print(f"g({x}) = {g_verdi}")
:::

::::{solution}
---
dropdown: 0
---

Vi definerer to funksjoner: `f(x)`{l=python} som representerer den lineære funksjonen $f(x) = 2x + 1$, og `g(x)`{l=python} som representerer den andregradsfunksjonen $g(x) = x^2 - 3$.

Deretter finner vi funksjonsverdiene for $x = 4$.

Utskriften blir:

:::{code-block} console
f(4) = 9
g(4) = 13
:::

::::

:::::::::::::::

---

:::::::::::::::{exercise} Underveisoppgave 1
Hva skriver programmet ut?

:::{interactive-code}
def f(x):
    return 2*x + 1

print(f(5))
:::

::::{answer}
:::{code-block} console
11
:::
::::

::::{solution}
Funksjonen `f(x)`{l=python} tar inn verdien `5` som `x` og regner ut `2 * 5 + 1`, som er 11. Dette returneres og blir deretter skrevet ut av `print`{l=python}.

Utskriften blir:

:::{code-block} console
11
:::
::::

:::::::::::::::

---

:::::::::::::::{exercise} Underveisoppgave 2
Lag en funksjon `g(x)`{l=python} som tilsvarer det matematiske uttrykket $g(x) = x^2 - 3$.
Bruk funksjonen til å regne ut og skrive ut oppgitt svar for $g(4)$.

:::{interactive-code}
# Skriv koden din her
:::

::::{answer}
Utskriften blir:

:::{code-block} console
13
:::
::::

::::{solution}
:::{code-block} python
---
linenos:
---
def g(x):
    return x**2 - 3

print(g(4))
:::
::::

:::::::::::::::

---

:::::::::::::::{exercise} Underveisoppgave 3
Ta quizen!

:::{quiz}
Q: Løs oppgaven ved å velge det riktige alternativet: Hvilken kodelinje kaller funksjonen riktig? <pre><code class="python">def min_funksjon(tall):\n    return tall * 2</code></pre>
+ `svar = min_funksjon(4)`
- `svar = min_funksjon[4]`
- `min_funksjon = 4`
- `def min_funksjon(4)`


Q: Hva er den viktigste forskjellen på `print` og `return`?
+ `return` sender et resultat tilbake til programmet slik at det kan lagres, mens `print` bare viser teksten på skjermen.
- De betyr akkurat det samme i Python.
- `return` kan bare brukes for tall, mens `print` bare er for tekstbeter.
- `print` avslutter funksjonen slik at den stopper.

:::
:::::::::::::::
