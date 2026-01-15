# Grafisk profil

Det här är en sida du kan använda för att testa och dokumentera den grafiska profilen för ditt företag eller projekt. Den innehåller riktlinjer för logotypanvändning, färger, typografi och andra visuella element.

Arbeta med varje del tills du är nöjd med hur den ser ut och fungerar. Anpassa innehållet efter dina behov och se till att allt följer din grafiska profil.

## Hur använder du mallen

Mallen finns på den här sidan i mappen `docs/index.html`. Du kan redigera HTML-koden direkt för att ändra innehållet och strukturen på sidan. Stilar och layout styrs av CSS-filen i `docs/styles.css`, så du kan också göra ändringar där för att anpassa utseendet.

De flesta ändringarna görs i CSS-filen, där du kan justera färger, typsnitt, marginaler och andra visuella element för att matcha din grafiska profil.
Detta styrs av CSS-variabler högst upp i filen, så det är enkelt att hitta och ändra dem.

CSS-variabler skrivs med två bindestreck före namnet, till exempel `--primary-color`. För att använda en variabel i CSS-koden så skriver du `var(--variabel-namn)`. Om du vill kan du ange ett standardvärde som används om variabeln inte är definierad, till exempel `var(--variabel-namn, #000)`.

Variablerna finns i `:root`-sektionen i CSS-filen och inkluderar färger, typsnitt, storlekar och andra designparametrar.

Om du vill skapa egna storleksvariabler för typsnitt och avstånd så kan du göra det med [utopia](https://utopia.fyi/).

```css
:root {
    /* Relativa storlekar för tyografik och avstånd. */
    /* Variabler för färger */
    --primary-color: #3498db;
    --secondary-color: #2ecc71;
    --color-dark: #333;
    --color-ligth: #f9f9f9;

    /* Variabler för typografi */
    --type-heading: sans-serif;
    --type-body: serif;
    --line-height-body: 1.6;
    --line-height-heading: 1.1;

    /* Avstånd för innehåll */
    --gutter: var(--space-m);
    --wrapper-max-width: 65rem;
}
```

## Innehåll

- [Logotyp](#logotyp)
- [Typografi](#typografi)
- [Färger](#färger)
- [Övrigt](#extra)

## Logotyp

Beskriv hur logotypen ska användas, inklusive storlek, placering och skyddszon.
Du kan skapa en logotyp i ett ritprogram och exportera den som en bildfil för att inkludera här.
Om du vill så går det även att skapa logotypen med AI. Du kan då använda en prompt som beskriver hur logotypen ska se ut. Det är då viktigt att du specifierar bildtypen, transparent bakgrund osv. samt att du vill att den ska generera en symbol och en version med text.

> I need you to generate 1 example logotype. I want you to produce the logotype in 2 different images, one with just the icon and one with the icon and text...

## Typografi

Beskriv de typsnitt som används i den grafiska profilen, inklusive rubriker, brödtext och eventuella specialtecken.
Ange storlekar, vikter och andra stilistiska riktlinjer för att säker

Ett tips här är att kolla på [Google Fonts](https://fonts.google.com/) för att hitta typsnitt som passar ditt företag. Du kan även läsa lite om olika typsnitt och dess användning på denna [Font guide](https://www.kolenda.io/guides/fonts). Pairings kan du kolla på [Font Pair](https://fontpair.co/) eller [Fontjoy](https://fontjoy.com/).

## Färger

Beskriv färgpaletten som används i den grafiska profilen, inklusive primära och sekundära färger samt eventuella accentfärger.
Ange färgkoder (hex, RGB, CMYK) och riktlinjer för hur färgerna ska användas tillsammans. 

Här är det viktigt att du testar de olika färgerna med text för att det ska gå att läsa. Om du behöver så kopiera color-swatch delen i HTML filen och skapa egna konfigurationer för att testa.

Testa sedan detta med hjälpa av [WAVE](https://wave.webaim.org/) verktyget för att se till att du har tillräcklig kontrast mellan text och bakgrundsfärger. Ett tips är att installera [browser-tillägget](https://wave.webaim.org/extension/) för WAVE. Du kan också använda [Contrast Checker](https://contrastchecker.com/) för att verifiera att dina färgval uppfyller tillgänglighetsstandarder.

## Övrigt

Beskriv andra viktiga visuella element i den grafiska profilen, såsom ikoner, bildstil eller layoutprinciper. Du kan kolla i brand-dokumentet på classroom för inspiration.

Inkludera riktlinjer för hur dessa element ska användas för att säkerställa en konsekvent visuell identitet. Det kan vara sådant som knappar, kanter, skuggor med mera.