# Selektorių specifiškumas

Specifiškumas nustato, kurią CSS taisyklę pagal prioritetą taiko naršyklė HTML elementams selektoriuse. Paprastai tariant, specifiškumas yra taisyklių rinkinis, nusakantis prioritetą stiliaus atributams taikytį.

Tarkime turime tokį HTML kodą:

```html
<div id="someID">
  <label>Input name</label>
  <input class="classname" type="text"/>
</div>
```

Pagal nutylėjimą elemento specifiškumas yra (0, 0, 0, 0)

---

Rašant selektorių pagal elemento pavadinimą (input):

```css
input {
    color: red;
}
```

specifiškumas yra (0, 0, 0, 1)

---

Rašant selektorių pagal elemento pavadinimą (input) ir klasės atributą (class):

```css
input.classname {
    color: blue;
}
```

specifiškumas yra (0, 0, 1, 1)

---

Rašant selektorių pagal elemento ID (id) ir klasės atributą (class):

```css

#someID .classname {
    color: yellow;
}
```

specifiškumas yra (0, 1, 1, 0)

---

Rašant selektorių pagal elemento pavadinima, ID (id) ir klasės atributą (class):

```css
div#someID input.classname {
    color: blue;
}
```

specifiškumas yra (0, 1, 1, 2)

---

Yra taip pat specifinis raktažodis `!important`, kuri naudojant su stiliaus atributu, galima padidiną specifiškumą (1, 0, 0, 0) reikšme.

```css

input.classname {
    color: green
}
```

Specifiškumas čia bus (1, 0, 1, 1)

P.S.
```
*Pseudo-class selectors (for example, :hover) and attribute selectors (for example, [type="input"]) each have the same specificity as a class selector. The universal selector (*) and combinators (>, +, ~) have no effect on specificity.*
```
