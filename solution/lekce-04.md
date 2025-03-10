## Cvičení - cykly 
---

## 1 - Seznam hodnocení

Mějme seznam hodnocení divadelní hry Plyšáci na útěku , který vypadá takto: 

```python
hodnoceni = [7, 9, 6, 7, 9, 8]
```

- Vytvořte program, který projde tento seznam a vypíše každé hodnocení na nový řádek.
- Upravte program tak, aby vypisoval výstup v tomto formátu

```python
7/10
9/10
6/10
7/10
9/10
8/10
```

<details>
<summary><b>Řešení</b></summary>

```python
for h in hodnoceni:
    print(f"{h}/10")
```

</details>

## 2 - Procházení seznamu
Založte si program **hesla.py** a na jeho začátek vložte následující kód obsahující seznam hesel pro přihlášení do nějakého systému

```python
hesla = [
    "xyz101",
    "punťa",
    "razor-blade",
    "1234",
    "12011986",
    "martin111",
    "trhnisi",
    "hokuspokus",
    "jeník15",
    "kristus-te-spasi",
    "beruška",
    "strčprstskrzkrk",
]
```

- Pomocí cyklu vypište všechny hesla na obrazovku, každé na jeden řádek.
- Upravte váš program tak, aby vypisoval jen bezpečná hesla, tedy taková, jež jsou delší než 8 znaků.

<details>
<summary><b>Řešení</b></summary>

```python
for heslo in hesla:
    print(heslo)

for heslo in hesla:
    if len(heslo) > 8:
        print(heslo)
```

</details>

## 3 - Složitější seznam
Založte si program **cykly02.py** a použijte v něm následující seznam měsíců v roce, Všimněte si, že je to seznam seznamů.

```python
mesice = [
    ["leden", 31],
    ["únor", 28],
    ["březen", 31],
    ["duben", 30],
    ["květen", 31],
    ["červen", 30],
    ["červenec", 31],
    ["srpen", 31],
    ["září", 30],
    ["říjen", 31],
    ["listopad", 30],
    ["prosinec", 31],
]
```

- Pomocí cyklu projděte tento seznam a vypište na výstup názvy jednotlivých měsíců.
- Pomocí dalšího cyklu vypište na výstup počty dní v jednotlivých měsících.

<details>
<summary><b>Řešení</b></summary>

```python
for mesic in mesice:
    print(mesic[0])

for mesic in mesice:
    print(mesic[1])
```

</details>

## 4 - Průměr
Napište cyklus, který projde zadaný seznam desetinných čísel a spočítá jejich průměr. Seznam čísel si vytvořte na začátku programu.

<details>
<summary><b>Řešení</b></summary>

```python
soucet = sum(cisla)
pocet = len(cisla)
prumer = soucet / pocet
print(f"Průměr: {prumer}")
```

</details>

## 5 - Hry
Následující seznam obsahuje seznam všech divadelních her, které se hrají v divadle Pěst na oko. Každá hra má svůj název a trvání v minutách.

```python
hry = [
    ["Ňadro na ňadru na nádru", 180],
    ["Útok plyšových krokodýlů", 95],
    ["Cesta do říše zelí", 128],
    ["Romance na zdymadle", 144],
    ["Zátiší s mimozemšťanem", 135],
    ["Čtyři facky a dortík", 100],
    ["Motorová okurka", 165],
    ["Johnny Noir", 140],
    ["Pražská kavárna vrací úder", 130],
    ["Pět sester ve vratech", 111],
    ["Stařec a krajta", 187],
    ["Růžová nemoc", 210],
    ["Smrt v přímém přenosu", 265],
]
```

- Pomocí cyklu projděte tento seznam a vypište na výstup názvy všech her.
- Vypište na výstup názvy všech her, které trvají více než 120 minut.
- Vypište na výstup názvy všech her spolu s jejich trváním v hodinách a minutách.

<details>
<summary><b>Řešení</b></summary>

```python
for hra in hry:
    print(hra[0])

for hra in hry:
    if hra[1] > 120:
        print(hra[0])

for hra in hry:
    hodiny = hra[1] // 60
    minuty = hra[1] % 60
    print(f"{hra[0]} trvá {hodiny} hodin a {minuty} minut")
```

</details>
