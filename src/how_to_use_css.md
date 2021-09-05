# Kaip pritaikyti CSS HTML dokumente?

* CSS gali būti panaudotas HTML dokumente trimis būdais:
    * Naudojant nuoroda į išorinį .css dokumentą, naudojant HTML žymę (ang. tag) `<link>`.
    * Rašyti CSS dokumento skilties `<head>` žymoje (ang. tag) naudojant `<style>`,
    * Rašyti CSS naudojant bet kurios HTML žymos (ang. tag) stiliaus atributą (style).
* Geriausia praktika yra naudoti išorinį .css failą visiems stiliams išsaugoti.
* Keletas CSS savybių, kurios naudosime pavyzdžiuose (paskui panagrinėsim daugiau jų ir detaliau, kai išmoskime atrinkti HTML elementus, kuriems norėsime pritaikyti stiliaus atributus):
    * color (red, blue it t.t.) - spalvai nusakyti.
    * border (pvz., border: medium solid) - rėmialiui nusakyti.
    * background-color (green, magenta ir t.t.) - fono spalvai.
    * text-transform (uppercase, lowercase) - teksto transformacijai.
    * font-weight (500, 600) - teksto šrifto dydžiui pakeisti.

---

```html
<!DOCTYPE html>
<html>
    <head>
        <link rel="stylesheet" href="css/main.css" type="text/css">
        <style>
            h1 {
                color: orange;
            }
        </style>
    </head>
    <body>
        <main style="background-color: red">
            <h1>Hello from CSS !!!</h1>
            <div class="some"></div>
        </main>
    </body>
</html>
```
