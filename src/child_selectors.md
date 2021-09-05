# Child (vaiko :D) selektorius

* `>` simbolis leidžia mums pritaikyti stilius elementams kurie yra tiesioginiai vaikiniai elementai tėviniam elementui :D

```html
<!DOCTYPE html>
<html>

<head>
  <style>
    .my-element > div {
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

![Child selektorius](image/child_selector.png)
