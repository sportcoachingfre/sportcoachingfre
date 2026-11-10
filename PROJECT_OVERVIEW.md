# Sportcoaching Fre

## Doel
Een website die het aanbod en de coach voorstelt. Bezoekers kunnen extra informatie aanvragen over personaltraining, bootcamps en zwemlessen. De coach neemt daarna persoonlijk contact op.

## Doelgroep
Volwassenen die interesse hebben in personaltraining of bootcamps, en ouders die zwemlessen zoeken voor kinderen vanaf 4 jaar.

## Eerste versie
- Duidelijke informatie over de coach als personal coach en zwemlesgever in het zwembad van Aarschot.
- Uitleg over personaltraining voor volwassenen, op afspraak.
- Uitleg over bootcamps op donderdagavond: 19.15–20.15 uur en 20.15–21.15 uur.
- Uitleg over zwemlessen voor kinderen vanaf 4 jaar, op vrijdag vanaf 16 uur.
- Een informatieformulier waarin bezoekers hun interesse aanduiden en een bericht kunnen sturen. Aanvragen worden per e-mail aan de coach bezorgd.
- Goed bruikbaar op gsm en computer.

## Nog niet
- Geen agenda, vrije tijdstippen kiezen of definitieve boekingen.
- Geen online betalingen of bezoekersaccounts.
- Geen eigen klantenbestand of beheerportaal.

## Platform
Een publiek toegankelijke website, zodat bezoekers het aanbod eenvoudig kunnen bekijken en delen.

## Frameworks en bouwstenen
Astro, omdat de website vooral bestaat uit informatiepagina's met een eenvoudig formulier. Voor het versturen van formulieren is een externe formulierdienst nodig, omdat GitHub Pages zelf geen e-mails verstuurt. De dienst en het ontvangstadres worden bij de uitwerking gekozen en ingesteld.

## Opslag
Geen eigen database. Informatieaanvragen worden via een formulierdienst naar de mailbox van de coach gestuurd. Bewaar contactgegevens en berichten niet in de publieke repository of op de publieke website, ook niet als voorbeeld. Vraag voor zwemlesinformatie alleen de noodzakelijke contactgegevens van een ouder of verantwoordelijke; geen kinddossier. De instellingen voor verwerking en bewaring bij de formulierdienst worden bij de uitwerking vastgelegd.

## Vormgeving
Gebruikt het design system in `design-system/` als vertrekpunt. Schoollogo's en AI-specifieke inhoud passen niet bij deze sportwebsite en worden niet als identiteit van de coach gebruikt. De gebruiker kan later een ander design laten ontwerpen en het huidige vervangen.

## Eisen
- Bezoekers moeten zich gewoon kunnen aanmelden voor extra informatie; ze moeten geen uren kunnen kiezen of vrij inplannen.
- Zwemlessen zijn bedoeld voor kinderen vanaf 4 jaar en starten vrijdag vanaf 16 uur.
- Personaltraining is bedoeld voor volwassenen.
- Bootcamps zijn donderdagavond van 19.15 tot 20.15 uur en van 20.15 tot 21.15 uur.

## Publicatie
GitHub Pages. Een publicatieworkflow wordt bij de bouw ingericht: elke merge naar de hoofdbranch `main` publiceert de site automatisch.
