# Pseudo elementų selektoriai

Pseudo elementų selektoriai yra panašus į pseudo klases. Pseudo elementai yra raktinis žodis pridedamas prie selektoriaus pabaigos, prieš jį rašant dvigubą dvitaškį (::). Jo paskirtis pritaikyti stiliaus atributus prie tam tikros elemento dalies, pavyzdžiui, galo (after), pirmos teksto eilutės ir t.t.

---

```css
a::after { 
    content: '⤴';
}

p::first-line {
    color: blue;
}
```

---

Sintaksė:

```css
selector::pseudo-element {
    property: value;
}
```
