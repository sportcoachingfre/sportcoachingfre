# Website beheren

De website gebruikt Astro. Start lokaal met `npm install` en `npm run dev`.
`npm test` controleert de echte website op desktop- en gsm-formaat met Playwright.
Installeer daarvoor eerst Chromium met `npx playwright install chromium`.
`npm run build` maakt de publicatie in `dist/`.

## Formulier

Stel `PUBLIC_FORM_ENDPOINT` in als GitHub Actions-secret met een FormSubmit-URL.
De bestemming staat zo niet in de bronbestanden, maar de gebouwde formulieractie is zichtbaar voor bezoekers. Een door FormSubmit uitgegeven ondoorzichtige identificatie kan later de mailadres-URL vervangen.
Zonder bestemming is de verzendknop uitgeschakeld en staat er een duidelijke melding.

Bij het eerste gebruik stuurt FormSubmit een activatiemail naar de ontvanger. De eigenaar moet die bevestigen voordat aanvragen bezorgd kunnen worden. Doe vervolgens zelf een proefaanvraag en controleer de ontvangst, ook in de spammap. Browsertests versturen geen echte aanvragen. De externe dienst beheert zijn eigen bevestigingspagina en eventuele captcha.

## Publicatie

GitHub Pages moet op GitHub Actions als publicatiebron staan. De workflow controleert elke pull request en publiceert na een geslaagde controle op `main`.
Er worden geen eigen database, analytics of betaalfuncties gebruikt.
