# Hópverkefni 1 - Lausn


## Hvernig skal keyra verkefnið

Til þess að keyra verkefnið í fyrsta sinn þarf að sækja node.js og keyra skipunina npm install inn í aðalmöppu.
Við það eru allir nauðsynlegir pakkar settir upp. Síðan þarf að keyra skipunina node run sass til þess að þýða
SCSS skrár yfir í CSS skrá sem stýrir útliti síða.

Til þess að keyra verkefnið má svo nota eftirfarandi skipanir:
* Til þess að þýða scss skrár yfir í styles.css: npm run sass
* Til þess að skoða síður á eigin netþjóni: npm run browser-sync
* Til þess að skoða síður á eigin netþjóni og þýða jafnóðum allar breytingar á þeim með sass: npm run dev
* Til þess að fara yfir allar skrár og athuga hvort málfræðin í þeim sé í samræmi við staðla verkefnsins: npm run lint

## Uppsetning verkefnis
Verkefnið er sett upp á eftirfarani máta:

### HTML skjöl fyrir siður
Heimasíðan er í skjalinu index.html sem er geymt í rót verkefnisins. HTML skjöl fyrir aðrar síður eru í möppunni ./pages

### SCSS og CSS skrár
Allt CSS útlit er unnið í SCSS skrám í möppunni ./styles. Node-sass er svo notað til þess að þýða SCSS skránnna styles.scss 
sem inniheldur import köll á allar hinar SCSS skrárnar. Skráin er þýddi yfir í skránna styles.css sem öll öll HTML skjölin
nota til þess að útfæra CSS útlitslýsingu sína. Skráin styles.scss er geymd í rót verkefnis og skráin styles.css er einnig
skrifuð í rótina.

Þegar SCSS skrár eru þýddar þýðir Node-sass skránna 

Í möppunni ./styles er einnig að finna möppuna ./pages, þar eru scss skrár sem stýra útliti sem er takmarkað við ákveðnar
síður geymdar. Í heildina inniheldur verkefnið eftirfarandi SCSS skrár (í þeirri röð sem styles.scss sækir þær):
* config : skrá sem sækir letur og skilgreinir leturstærð, nöfn lita og hámarks breidd síðu.
* grid : skrá sem skilgreinir grind sem síðum er raðar eftir
* global : skrá sem skilgreinir útlit almennra eiginda
* header : skrá sem skilgreinir útlit eiginda sem birt eru í header
* hovercards : skrá sem skilgreinir útlit og eigindi korta (hover cards) sem sýna uppskriftir
* recipe : skrá sem skilgreinir útlit uppskrifta (texta og lista af hráefnum).
* homePage : skrá sem skilgreinir útlit eiginda sem aðeins birtast á index.html
* latestRecipesPage : skrá sem skilgreinir útlit eiginda sem aðeins birtast á latestrecipes.html
* recipePage : skrá sem skilgreinir útlit eiginda sem aðeins birtast á recipe.html
* videoRecipePage : skrá sem skilgreinir útlit eiginda sem aðeins birtast á videorecipe.html
* footer : skrá sem skilgreinir útlit eiginda sem birt eru í footer

## Hópur

Jón Guðjónsson (einn í hóp) 
HÍ-notendanafn: jog35
Github-notendanafn: JonGudjonsson

