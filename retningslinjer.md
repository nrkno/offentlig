# Retningslinjer for deling av åpen kildekode

Retningslinjene omfatter interne prosjekter laget av Norsk rikskringkasting
(NRK) som blir delt under en åpen kildekodelisens på GitHub-organisasjonen
[`nrkno`](https://github.com/nrkno).

Deling av åpen kildekode innebærer at NRK lisensierer og offentliggjør sine kodebrønner åpent så andre kan se, bruke og lære av dem.

## Motivasjon

Målet med retningslinjene er å sørge for en felles forståelse av omfang og
forpliktelser når vi deler åpen kildekode.

## Dokumentets gyldighet

Retningslinjer og anbefalinger i dette dokumentet gjelder for alle nye
kodebrønner og kodeprosjekter som åpnes etter vedtaksdato.

For å sikre vedvarende forpliktelse skal retningslinjene revideres årlig. Techleadforum nedsetter en arbeidsgruppe som holder i dette.

## Lisensiering av åpen kildekode

Hos NRK bruker vi `MIT` for lisensiering av åpen kode.

`MIT` er en [OSI-godkjent](https://opensource.org/licenses) kodelisens som gir
brukeren fri og ubegrenset tilgang til koden for egne prosjekter.

For selve lisensieringen av kode brukes [SPDX](https://spdx.dev/). Dette er en
standard for å snakke om lisenser, kode og leveringskjeder innenfor åpen
kildekode. Den definerer maskinlesbare merker for kodelisenser og kopirett.
Kildekode delt av NRK skal ha SPDX-merker i toppen av alle kodefiler.

Eksempel:

```
# SPDX-License-Identifier: MIT
# SPDX-FileCopyrightText: Copyright (c) Norsk Rikskringkasting AS (NRK).
```

## Eierskap og vedlikehold

Offentliggjøring av en kodebrønn skal skriftlig godkjennes av tilhørende produkteier, eller tilsvarende rolle, før publisering.

Vi anbefaler at dette loggføres i et internt dokumentasjonsverktøy for teamet.

Det praktiske eierskapet til prosjektet ligger hos teamet.

For strategisk viktige prosjekter bør offentlig tilgjengelige forvaltningsverktøy, f.eks. GitHub, vurderes som del av ordinær arbeidsflyt slik at arbeid med videreutvikling skjer åpent og allment tilgjengelig.

### Språklige hensyn

NRK anbefaler at åpne kodebrønner og tilhørende dokumentasjon skrives på engelsk.

Selv om arbeidsspråket i NRK er norsk, ser vi at det vil være gunstig å bruke engelsk for å bidra til åpen kildekode hvor dette er sedvane.

Teamet kan selv vurdere å avvike fra dette om det er hensiktsmessig.

### Rutine for arkivering

Kodebrønner som ikke lenger vedlikeholdes, eller brukes aktivt av NRK, skal tydelig markeres som arkiverte prosjekter. I Github skal "Archive" funksjonaliteten brukes, samt andre språkspesifikke arkiveringsmerknader.

En arkivert kodebrønn kan ved behov gjenåpnes. Det bør samtidig vurderes om eventuelle forgreninger (forks) kan ha verdi for videre forvaltning.

## Versjonering

Det forventes at prosjektet blir versjonert. Nåværende standard på prosjekter i
NRK er å bruke [semver](https://semver.org/). Se [blåboka](https://xn--blbok-nra.plattform-int.weu.k8s.az.nrk.cloud/Standarder/RFC-3-semver.html) for mer informasjon.
