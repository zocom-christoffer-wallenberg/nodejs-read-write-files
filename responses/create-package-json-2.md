## Skapa en package.json

En package.json är som en settingsfil för ditt projekt. Den innehåller information om vem som är skaparen, hur ditt program startas,
vilka moduler (dependecies) som behövs installeras. En package.json är unik för varje projekt man har och gör det enkelt för en annan utvecklare att klona ner ditt repo och köra igång.

För att skapa en package.json, börja med att öppna upp din terminal och navigera till övningsrepot på din dator (använder du VS Code kan du öppna upp en terminalfönster i VS Code).

Tips! Glöm inte bort att samtidigt kolla i presentationen på Learnpoint för hjälp.

I terminalen skriv:

```npm init````

Då kommer att få lite frågor att svara på och efter det kommer en package.json att skapas. Du borde efter det se en package.json fil i ditt repo.

För att installera en **dependecy** i din package.json skriver du:

```npm install express --save```

```--save``` betyder att din installerade **dependecy** kommer att sparas i din package.json. 

I Github desktop lägg till din skapade package.json och commita den och sedan pusha till Github. När du har gjort det kommer nästa steg att visas.