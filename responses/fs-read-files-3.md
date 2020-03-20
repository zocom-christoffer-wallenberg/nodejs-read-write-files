## Läsa från en textfil

I detta steg ska vi läsa från en textfil på datorn och skriva ut innehållet i terminalen. Till hjälp ska vi använda oss av den inbyggda modulen ```fs``` (en inbyggd modul behöver vi inte installera med npm).

Först behöver vi ladda in modulen ```fs``` med hjälp av ```require```.

Skriv nedanstående i **app.js**.

```
const fs = require('fs');
```

Nu kan vi anväda oss av variabeln fs och alla funktioner som finns i den modulen. I detta steg ska vi använda oss av ```readFile```för att läsa in innehållet.

I din **app.js** skriv in nedanstående kod:

```
fs.readFile('quote.txt', 'utf8', (error, contents) => {
    console.log(contents);
});
```

Kör ditt program nu i terminalen med kommandot ```node app.js```.
Nu bör du se texten **You can never be overdressed or overeducated** skrivas ut i terminalen.

Vad är det som händer måntro?

```readFile``` tar tre parametrar. Den första är sökvägen till textfilen, den andra är teckenkodningen och den sista är en callback-funktion som ska köras när inläsningen av filen är klar.

Har allt gått bra som finns innehållet i **contents** annars finns det ett felmeddelande i **error**.

I Github desktop lägg till app.js och commita den, sedan pusha till Github. När du har gjort det kommer nästa steg att visas.