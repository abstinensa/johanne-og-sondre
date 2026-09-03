# Johanne og Sondre — bryllaupsside

Bryllaupsnettsida til Johanne og Sondre, hosta på GitHub Pages med eige
domene ([www.johanneogsondre.no](https://www.johanneogsondre.no)). Sida er
éi fil: `index.html`. Bryllaupsdatoen er **29. mai**.

## Filer

- `index.html` — heile sida (struktur, styling og skript i éi fil).
- `CNAME` — **må aldri slettast eller endrast**. Krevst for det eigne
  domenet på GitHub Pages.
- `README.md`

## Reglar for endringar

- Innhaldet på sida skal vere på **bokmål**.
- Behald design, fargar og tone som dei er — ikkje gjer om på layout,
  fargepalett (`--plomme`, `--solnedgang`, `--fersken`, `--krem`,
  `--oliven`, `--sennep`, `--rosa`) eller skrifttypar utan at det er
  eksplisitt bedt om.
- Ikkje rør `CNAME`.
- Gjer berre dei endringane som er eksplisitt bedt om — ikkje "forbetre"
  eller endre anna innhald på eiga hand.
- Passordgata (`#gate`, `const PASSORD` nedst i skriptet) er berre
  klientside-fnising, ikkje reell sikkerheit — den held nysgjerrige ute,
  ikkje motiverte personar.

## Kontaktinfo / sensitive verdiar i sida

Desse felta inneheld verdiar som må haldast oppdaterte og kan endre seg:

- **Toastmaster-e-post** — `mailto:`-lenke i info-kortet "Toastmaster".
- **RSVP-e-post** — `mailto:`-lenke (med subject) i RSVP-seksjonen,
  same adresse kan òg stå som synleg tekst.
- **Vipps-nummer** — i info-kortet "Ønskeliste: Kjøp oss festivalbillett".
- **Passord** — `const PASSORD` nedst i `<script>`.

Status per no: e-post-adressene (toastmaster + RSVP) og Vipps-nummeret er
**enno ikkje mottatt** frå brudeparet ("kommer" i påvente av svar) og står
difor framleis som placeholder (`toastmaster@epost.no`,
`johanneogsondre@epost.no`, `000 00 000`) i fila. Desse må oppdaterast med
ekte verdiar så snart dei ligg føre — dei skal **aldri** fyllast ut med
oppdikta/gjetta verdiar sidan sida er live og brukt av ekte gjester til
RSVP og betaling.

Passordet er sett til **`29mai`** (matcher bryllaupsdatoen).
