# Descendant (palikuonių :D) selektorius

* Stiliaus taisykles HTML elementams galima apibrėžti, naudojant selektorių kombinacijas.
* Pavyzdžiui, selektorius **my-element div** pritaikis CSS stiliaus taisykles visiems `<div>` elementams, kurie yra elemento su ID reiksme **#my-element** viduje. Šiuo atveju `<div>` elementai yra vadinami vaikiniais (children) elementais, o **#my-element** yra vadinamas tėviniu (ancestor)

```html
<!DOCTYPE html>
<html>

<head>
  <style>
    .my-element div {
      border: medium solid;
    }
  </style>
</head>

<body>
  <div class="my-element">
    <div>
      Tekstas 1
      <div>Tekstas 1.1</div>
      <hr />
      <div>Tekstas 1.2</div>
    </div>
    <hr />
    <div>Tekstas 2</div>
  </div>
  <hr />
  <div>Isorinis tekstas</div>
</body>

</html>
```

---

![Descendant selektorius](./image/descendant_selector.png)
