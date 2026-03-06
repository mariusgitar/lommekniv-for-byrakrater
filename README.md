# Byråkratens lommekniv

Byråkratens lommekniv er en enkel, statisk portal som samler lenker til småverktøy for dokumenthåndtering og digitalt kontorarbeid.

Portalen inneholder ikke selve verktøyene. Den fungerer som en ryddig startside som peker videre til eksisterende GitHub Pages-apper.

## Hva prosjektet inneholder

- En rolig og responsiv forside med tre verktøykort
- Illustrert bakgrunnsbilde for en tydelig, men dempet profil
- Klare lenker videre til:
  - PDF-sammenslåer
  - QR-kodefabrikk
  - PII-scrubber
- En liten bunnseksjon som sier at flere verktøy kommer
- En kontaktlinje for forslag til nye verktøy

## Endre lenker til verktøyene

Åpne `index.html` og oppdater `href` i hvert verktøykort:

- `https://BRUKERNAVN.github.io/pdf-sammenslaaer/`
- `https://BRUKERNAVN.github.io/qr-kodefabrikk/`
- `https://BRUKERNAVN.github.io/pii-scrubber/`

Bytt `BRUKERNAVN` med faktisk GitHub-brukernavn.

## Publisere med GitHub Pages

1. Push prosjektet til ønsket GitHub-repo.
2. Gå til **Settings → Pages** i repoet.
3. Velg deploy-kilde: **Deploy from a branch**.
4. Velg branch (typisk `main`) og mappe (`/root`).
5. Lagre. GitHub publiserer siden automatisk.

## Feilsøking ved publisering

Hvis GitHub Actions ikke starter som forventet etter en endring, kan en ny commit og push ofte trigge kjøringen på nytt. Sjekk også at Actions er aktivert i repo-innstillingene.

## Viktige filer

- `index.html` – innhold og struktur for portalen
- `styles.css` – all visuell stil og responsiv layout
- `README.md` – kort dokumentasjon og sjekkliste
- Bakgrunnsillustrasjonen er lagt inn direkte i `styles.css` (tekstformat) for å unngå binærfil i repoet

> Sist oppdatert: liten dokumentasjonsendring for å trigge ny CI/Actions-kjøring.

## Manuell testliste

- [ ] Siden laster lokalt i nettleser (åpne `index.html`).
- [ ] Tittel og intro vises riktig.
- [ ] Alle tre verktøykort vises med navn, beskrivelse og knappelenke.
- [ ] Lenkene peker til riktige plassholder-URL-er.
- [ ] Layout fungerer på smal skjermbredde.
- [ ] Hover- og fokus-state er tydelig på lenkene.
- [ ] Kontaktlinje med e-post vises i bunnseksjonen og e-postlenken fungerer.
- [ ] Kontrast og lesbarhet er god på lys bakgrunn.
