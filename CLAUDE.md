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
**enno ikkje mottatt** frå brudeparet. På eksplisitt ønske frå brudeparet
viser sida no berre teksten **"Kommer"** i staden for oppdikta/placeholder
e-postar og Vipps-nummer:

- Toastmaster-kortet viser "Kommer" i staden for ei mailto-lenke.
- Vipps-feltet viser "Vipps: Kommer".
- RSVP-knappen er gjort om frå ei fungerande `mailto:`-lenke til ein
  ikkje-klikkbar `<span class="knapp">` med teksten "RSVP-e-post kommer",
  sidan ei fungerande knapp med falsk e-post ville gitt gjester ein daud
  lenke.

Desse tre stadene må oppdaterast med ekte verdiar så snart dei ligg føre —
då skal RSVP-knappen igjen bli ei fungerande `<a class="knapp"
href="mailto:...">`-lenke. Dei skal **aldri** fyllast ut med
oppdikta/gjetta verdiar i mellomtida, sidan sida er live og brukt av ekte
gjester til RSVP og betaling.

Bryllaupsdato er **29. mai**, og passordet er sett til **`29mai`**
(matcher datoen).
