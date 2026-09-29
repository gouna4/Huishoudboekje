# Huishoudboek · v16

Je vaste lasten en uitgaven bijhouden, zien waar je geld heen gaat, en tips
krijgen waar je kunt besparen. Broertje van het telefoonboek en het klusboek.

**Geen server, geen account, geen internet nodig.** Wat je invult blijft in de
opslag van de browser op je eigen toestel en wordt nergens naartoe gestuurd.
Deze bestanden zijn leeg: wie de site opent, krijgt een leeg boek.

## Wat het doet

- **Vaste lasten** met een eigen rondje per soort, zoals in de bankapp: huur,
  energie, water, internet, mobiel, verzekeringen, belastingen, boodschappen,
  streaming, sport, auto, kinderen, huis & klussen, moskee en goede doelen,
  sparen en meer (28 soorten)
- Per week, per 2 of 4 weken, per maand, kwartaal, half jaar of jaar. De app
  rekent alles om naar per maand, per jaar en per week
- **Alleen in sommige maanden**, voor bijvoorbeeld gemeentebelasting in tien
  termijnen
- Typ je een naam als "Essent" of "Netflix", dan kiest de app zelf de soort
- **Prijs door de tijd**: pas je een bedrag aan, dan onthoudt de app de oude
  prijs. Duurder geworden staat in het rood met een ▲
- Opgezegd zetten in plaats van verwijderen, dan kloppen oude maanden nog
- Contract loopt af: twee maanden van tevoren een waarschuwing
- **Losse uitgaven** zoals boodschappen en tanken, met maandoverzicht en een
  grafiek van zes maanden
- **Opruimen**: prullenbak bij Vaste lasten, met ongedaan maken
- **Huishouden**: aantal volwassenen en kinderen, huur of koop, netto inkomen
- **Besparen**: de app vergelijkt wat je betaalt met ruwe richtwaarden voor
  een huishouden van jouw grootte, en kijkt naar prijsstijgingen, aflopende
  contracten, dure telefoonabonnementen, toeslagen en het overstapseizoen van
  de zorgverzekering
- **Thuis** (het huisje linksboven, daar start de app): je vult je netto
  inkomen in en de app verdeelt het over vier pilaren, elk met een cirkel die
  laat zien hoe ver je deze maand bent: vaste lasten, uitgaven, vervoer (10%)
  en sparen (5 tot 20%, zelf te kiezen). Geef je bij uitgaven of vervoer te
  veel uit, dan gaat het eerst van wat er bij de ander over is en daarna van
  sparen, nooit van de vaste lasten. Tik op een cirkel voor alles wat erin zit
- **Van salaris tot salaris**: een periode heet naar de maand waarin je het
  geld uitgeeft ("September" = salaris van 25 aug, 25 aug – 24 sep). Het huisje rekent per periode vanaf je
  betaaldag (standaard de 25e, in het weekend de vrijdag ervoor), met pijltjes
  om terug te kijken naar vorige periodes
- **Al afgeschreven**: bij elke vaste last geef je aan op welke dag hij echt
  afging, en eventueel dat hij voortaan op die dag komt. Valt een vaste last in
  het weekend, dan rekent de app met de vrijdag ervoor (instelbaar)
- **Afschrijvingen per vaste last**: de laatste vier en de volgende, elk met
  de periode waarin hij valt. Wat je bevestigt krijgt ✓ en gaat mee in de back-up
- **Vaste lasten per periode**: bij Vaste lasten wissel je tussen de hele lijst
  en wat er per salarisperiode is afgeschreven
- **Hoort bij**: per vaste last zelf kiezen in welke cirkel hij meetelt
- **Tijdelijk**: een vaste last die na een aantal keer vanzelf stopt
- **Inkomen per periode**: tik op het huisje op Inkomen ✎ en vul in wat je die
  periode kreeg; eventueel ook als standaard. Het inkomen blijft op het toestel
  en gaat niet mee in de back-up
- **Spaarrekening**: tik op de cirkel Sparen. Saldo één keer invullen, dan
  rekent de app verder. Erop gezet en noodgreep (geld eraf naar je
  betaalrekening) vul je in; vaste spaaropdrachten tellen vanzelf mee. Een
  noodgreep is geen inkomen: hij maakt je budget niet groter en blijft staan
  als "nog terug te zetten" tot je weer iets terugzet
- **Voorgeschoten**: geld dat je voorschiet voor klussen of telefoons telt niet
  mee bij je uitgaven. Terug gekregen (contant of via de bank) vul je in; het
  huisje laat zien wat je per soort nog terugkrijgt
- **Eigen soorten**: onder "Eigen soort" maak je een soort met naam en
  icoontje; bij voorgeschoten zet je met "+ Eigen" iets bij (klussen, telefoons,
  vlees en iets anders staan er al). Weghalen kan bij het tandwiel
- **Tanken**: eigen tabblad en eigen cirkel voor tanken, laden, parkeren,
  autowas en ov. Wegenbelasting, autoverzekering en ANWB zijn vaste lasten
- **Vaste lasten één keer per maand**: wat vanaf je betaaldag gepland staat,
  telt voor de maand die dan begint; zo heeft elke maand precies één Essent
- **Bewust zo ingesteld**: vinkje per vaste last, dan geeft de app er geen tips over
- **Jaaroverzicht**: per maand, per soort en per vaste last; afdrukken of
  opslaan als PDF
- **Pincode** van vier cijfers; op slot bij openen en na drie minuten weg
- **Het oogje** bovenin verbergt alleen je inkomen (en wat je daaruit kunt
  terugrekenen); alle bedragen verbergen kan bij de instellingen
- **Overal dezelfde periode**: huisje, vaste lasten, uitgaven en vervoer bladeren
  samen van salaris tot salaris
- Back-up sturen, opslaan of kopiëren; terugzetten uit een bestand of geplakte
  tekst; vijf herstelpunten op het toestel zelf; een melding als je twee
  weken geen back-up maakte

## Bestanden

    index.html        de hele app: opmaak en code in één bestand
    sw.js             offline werken; eerst het netwerk, dan de eigen kopie
    manifest.json     maakt hem installeerbaar op je beginscherm
    icon-192.png      pictogram
    icon-512.png      pictogram
    .gitignore        houdt back-upbestanden buiten GitHub

## Een nieuwe versie uitbrengen

Verhoog het nummer op twee plekken, anders zie je je eigen wijziging niet:

1. `index.html` — `var VERSIE='16'` bovenaan het script
2. `sw.js` — `huishoudboek-v16`

## Nooit in deze repo

Het back-upbestand (`huishoudboek-JJJJ-MM-DD-uummss.json`). Daarin staan je
bedragen, leveranciers en klantnummers. Je inkomen staat er niet in: dat
blijft op het toestel en verandert niet als je een back-up terugzet. `.gitignore` houdt ze
tegen, maar kijk voor het uploaden of er niets tussen zit.

## Let op

De gegevens hangen aan het webadres. Verhuis je de app naar een ander adres,
maak dan eerst een back-up en zet die daarna terug via de instellingen.
