## Skriva till en fil

I detta sista av ska vi skriva till en fil.

Eftersom vi i föregående steg läste in modulen ```fs``` med ```require``` behöver vi inte göra det igen. Utan vi kan hoppa
direkt till skriv till en fil.

Först skapar vi en variabel med en sträng som vi vill spara.

```
let quote = 'Be yourself. Everyone else is already taken.'
```

För att sedan skriva till en textfil använder vi oss av funktionen ```writeFile```. Skriv in nedan kod i **app.js**.

```
fs.writeFile('OscarWilde.txt', quote, (err) => {
   console.log('Quote saved!');
});
```

Kör ditt program nu i terminalen med kommandot ```node app.js```.
Nu bör du se texten **Quote saved!** skrivas ut i terminalen. Sedan bör du hitta en texfil i samma map som heter **OscarWilde.txt** och i den
ska det står  **Be yourself. Everyone else is already taken.**.

Denna första parametern är textfilens namn och om den inte finns kommer Node.js att skapa den på din dator. Den är andra parametern är texten som
ska skrivas till textfilen. Sista parametern är en callback-funktion som körs när det är klart.

Vi kan använda oss av strömmar för att kontinuerligt skriva till en fil. Testa och skriv nedanstående kod och kör den sedan.

```
const file = fs.createWriteStream('OscarWilde.txt');

for(let i=0; i < 5; i++) {
 file.write('You can never be overdressed or overeducated.\n');
}

file.end();
```
Du bör nu se texten **You can never be overdressed or overeducated.** fem gånger i textfilen **OscarWilde.txt**.

## Övning
Nu ska vi öva på att kombinera ```readFile``` och ```writeFile```.

Lägg in texten i textfilen **quote.txt** genom att första läsa in innehållet med ```readFile``` och sedan lägga på texten
```Be yourself. Everyone else is already taken.``` och skriva båda meningarna till **quote.txt**.

I Github desktop lägg till alla ändrade filer och commita, sedan pusha till Github. När du har gjort det är du klar och kommer få lite
instruktioner på övningar att träna på.