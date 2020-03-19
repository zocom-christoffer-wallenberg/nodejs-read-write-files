## Installation

Vi kommer börja med att installera Node.js. Du kan ladda ner det [här](https://nodejs.org/en/download/). Sedan installera det på datorn. Med Node.js installeras också NPM som är en pakethanterare för Node.

När installationen är klar kan du testa att all fungerar genom att öppna terminalen i ditt operativsystem. På Mac är det terminal och på Windows kan man använda sig av Powershell.

Skriv i terminalen:
```
node -v -> Om allt är korrekt bör det stå ex. v12.13.1
npm -v -> Om allt är korrekt bör det stå ex. 6.12.1
```

## Ditt övningsrepo

När du startade denna kurs installerades det ett övningsrepo på ditt konto som du kan hitta [här]({{ repoUrl }}).

Klona ner detta repo genom att trycka på **Clone and download** och sedan **Open in Github desktop**.

I detta repo kan du se att det ligger en fil som heter app.js som du kommer att jobba i.

## Hello World

I filen **app.js** skriv ```console.log('Hello World!')```och spara. Öppna upp en terminal och navigera dig med kommando **cd** till repot på din dator och skriv sedan:
```node app.js```för att köra ditt Node.js program.

Tips! I VS Code kan du öppna ett terminal direkt i ditt repo och köra ditt node program.

I terminalen bör du nu se texten **Hello World!**.

När du är klar tryck på knappen **Close issue** för att fortsätta!