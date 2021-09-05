# Užduotis 3

Tarkime turite tokį HTML kodą:

```html
<div id="someID">
    <label>Input name</label>
    <input class="classname" type="text"/>
</div>
```

Paskaičiuokite koks specifiškumas yra paskaičiuotas selektoriams?

```css
#someID input.classname {
    color: red;
}

label + input.classname[type="text"] {
    color: black;
}
```

Galite pasinaudoti specifiškumo [kalkuliatorium :D](https://specificity.keegan.st/)
