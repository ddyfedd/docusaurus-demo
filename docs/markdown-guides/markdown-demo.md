---
title: Markdown Formázási Példák
description: Bemutató a Docusaurusban használható Markdown formázásokról.
toc_max_heading_level: 5
sidebar_position: 1
draft: true
---

# Címsor 1 (H1)

Ez egy bevezető bekezdés. A Markdown egy egyszerű jelölőnyelv, amelyet könnyű olvasni és írni. A Docusaurus ezt használja a dokumentációs oldalak tartalmának létrehozásához.

[Belso hivatkozas](#inline-kód)

## Címsor 2 (H2)

Ez egy alcím. Itt bemutatjuk a különböző formázási lehetőségeket.

### Címsor 3 (H3)

Még mélyebb szintű címsor.

#### Címsor 4 (H4)

És így tovább...

##### Címsor 5 (H5)

###### Címsor 6 (H6)

---

## Szövegformázás

Ez **vastagított szöveg**.
Ez *dőlt szöveg*.
Ez _szintén dőlt szöveg_.
Ez ***vastagított és dőlt szöveg***.
Ez `kiemelt (inline) kód`.
Ez ~~áthúzott szöveg~~.

---

## Listák

### Számozatlan lista (Unordered List)

- Első elem
- Második elem
  - Beágyazott elem 1
  - Beágyazott elem 2
- Harmadik elem

### Számozott lista (Ordered List)

1.  Első pont
2.  Második pont
    1.  Alpont A
    2.  Alpont B
3.  Harmadik pont

### Feladatlista (Task List)

- [x] Befejezett feladat
- [ ] Befejezetlen feladat
- [ ] Még egy befejezetlen feladat

---

## Kódblokkok

### Inline kód

Ahogy fentebb láttuk, az `inline kódot` backtick-ek közé írjuk. Például: \`const valtozo = "érték";\`.

### Kódblokk (Code Block)

A kódblokkokat három backtick (```) közé zárjuk. Megadhatjuk a programozási nyelvet is a szintaxiskiemeléshez.

```javascript title="javascript.js"
// JavaScript példakód
function helloWorld(name) {
  console.log(`Helló, ${name}!`);
}

// highlight-next-line
helloWorld("Docusaurus");
```python
# Python példakód
def greet(name):
  print(f"Szia, {name}!")

greet("Felhasználó")
```html
<div>
  <h1>Ez egy HTML címsor</h1>
  <p>Ez egy HTML bekezdés.</p>
</div>
```

---

## Idézet (Blockquote)

> Ez egy idézet.
> Több soros idézet is lehetséges.
>
> > Beágyazott idézet.

---

## Vízszintes vonal (Horizontal Rule)

Három vagy több kötőjel, csillag vagy aláhúzás hoz létre egy vízszintes vonalat.

---

***

___

---

## Linkek (Links)

Ez egy link a [Docusaurus hivatalos oldalára](https://docusaurus.io/).
Ez egy relatív link egy [másik dokumentációs oldalra](./masik-oldal.md) (feltéve, hogy létezik).
Link hivatkozással:
[Google][google-link]

[google-link]: https://www.google.com

---

## Képek (Images)

![Docusaurus Logó](https://docusaurus.io/img/docusaurus.svg "Docusaurus Logó")

Képek is lehetnek linkek:
[![Docusaurus Logó mint Link](https://docusaurus.io/img/docusaurus.svg "Kattints ide a Docusaurus oldalához")](https://docusaurus.io/)

*Megjegyzés: A kép elérési útját és az alternatív szöveget helyesen kell megadni.*

---

## Táblázatok (Tables)

| Fejléc 1 | Fejléc 2 | Fejléc 3 |
| :------- | :------: | -------: |
| Balra    | Középre  | Jobbra   |
| cella    | cella    | cella    |
| cella    | cella    | cella    |

A `:` jelöli az igazítást:
- `:---` balra igazítás (alapértelmezett)
- `:--:` középre igazítás
- `---:` jobbra igazítás

---

## Docusaurus Admonitions (Figyelmeztetések/Megjegyzések)

Ezek speciális blokkok, amelyek kiemelik a fontos információkat.

:::note
Ez egy **megjegyzés** (note).
Hasznos általános információk közlésére.
:::

:::tip
Ez egy **tipp** (tip).
Javaslatokat, trükköket oszthatsz meg itt.
:::

:::info
Ez egy **információ** (info) blokk.
Fontos tudnivalókhoz.
:::

:::caution
Ez egy **figyelmeztetés** (caution) blokk.
Potenciális problémákra vagy mellékhatásokra hívja fel a figyelmet.
:::

:::danger
Ez egy **veszély** (danger) blokk.
Kritikus információkhoz, amelyek figyelmen kívül hagyása komoly következményekkel járhat.
:::

### Admonition egyedi címmel

:::note[Egyedi Cím Itt]
Ez egy megjegyzés egyedi címmel.
:::