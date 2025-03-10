## Cvičení - funkce 
---

## 1 - Násobení
Napiš funkci mult, která bude mít dva číselné parametry. Funkce oba parametry vynásobí a vrátí výsledek.

<details>
<summary><b>Řešení</b></summary>

```python
def mult(a, b):
    return a * b

vysledek = mult(4, 5)
print(vysledek)
```

</details>

## 2 - Hotel
Napiš funkci total_price, která vypočte cenu noci v hotelu. Funkce bude mít dva parametry - persons a breakfast. Cena za noc za osobu je 850 Kč a cena za snídani za osobu je 125 Kč. Funkce vrátí výslednou cenu. Parametr breakfast je nepovinný a výchozí hodnota je False.

Funkci vyzkoušej se zadáním dvou i jedné hodnoty, např. total_price(3), total_price(2, True).

<details>
<summary><b>Řešení</b></summary>

```python
def total_price(persons, breakfast=False):
    cena = persons * 850
    if breakfast:
        cena += persons * 125
    return cena

print(total_price(3))
print(total_price(2, True))
```

</details>

## 3 - Faktoriál
Vytvoř program, který obsahuje funkci pro výpočet libovolného faktoriál. (https://cs.wikipedia.org/wiki/Faktori%C3%A1l) 

Využij funkci z matematického modulu.

<details>
<summary><b>Řešení</b></summary>

```python
import math

def faktorial(n):
    return math.factorial(n)

print(faktorial(5))
```

</details>

## 4 - Rámeček
Napiš funkci, která jako parametr převezme řetězec a vytiskne jej obalen hvězdičkami.

```
Zadej slovo: ahoj
********
* ahoj *
********
```

Nápověda: 8 * '*' == '********'

Bonus: Znak, kterým se má text obalit, bude zadán také jako parametr.

<details>
<summary><b>Řešení</b></summary>

```python
def ramecek(text, znak='*'):
    delka = len(text) + 4
    print(znak * delka)
    print(f"{znak} {text} {znak}")
    print(znak * delka)

ramecek("ahoj")
ramecek("ahoj", "#")
```

</details>