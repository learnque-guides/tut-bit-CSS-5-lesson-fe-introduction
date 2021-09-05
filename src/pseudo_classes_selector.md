# Pseudo klasės selektoriai

CSS pseudo klasė yra raktinis žodis pridedamas prie selektoriaus pabaigos, prieš jį rašant dvitaškį (:), kuris naudojamas norint nurodyti, kad norite stilizuoti pasirinktą elementą, bet tik tada, kai jis yra tam tikroje būsenoje.

---

```css
selector:pseudo-class {
    property: value;
}
```

---

Pavyzdžiai:

```css
a:hover, a:focus {
    color: darkred;
    text-decoration: none;
}

button:hover {
    color: blue;
}

div:first-child {
    color: blue;
}

div:last-child {
    color: blue;
}

li:nth-child(2) {
    color: lime;
}

:nth-child(4n) {
    color: lime;
}

p:last-of-type {
    color: red;
    font-style: italic;
}

/* and more */
```

Daugiau informacijos apie pseudo klases: [Pseudo classes](https://developer.mozilla.org/en-US/docs/Web/CSS/Pseudo-classes)
