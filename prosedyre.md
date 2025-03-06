# Prosedyre for deling av åpen kildekode

Prosedyren omfatter kildekode laget av Norsk rikskringkasting AS
(NRK) som blir delt under en åpen kildekodelisens på GitHub-organisasjonen
[`nrkno`](https://github.com/nrkno).

## Formål

Formålet med prosedyren er å sørge for en felles forståelse av omfang og
forpliktelser når vi deler åpen kildekode.

Deling av åpen kildekode innebærer at NRK lisensierer og offentliggjør sine kodebrønner åpent så andre kan se, bruke og lære av dem.

## Dokumentets gyldighet

Prosedyre og anbefalinger i dette dokumentet gjelder for alle nye
kodebrønner og kildekode som åpnes etter vedtaksdato.

Unntak fra ledd i prosedyren skal begrunnes av teamet. For spesielt viktig kildekode skal dette løftes til produkteier, eller tilsvarende rolle.

## Lisensiering av åpen kildekode

Hos NRK bruker vi `MIT` for lisensiering av åpen kildekode.

`MIT` er en [OSI-godkjent](https://opensource.org/licenses) kodelisens som gir
brukeren fri og ubegrenset tilgang til koden for egne prosjekter.

For selve lisensieringen brukes [SPDX](https://spdx.dev/). Dette er en
standard for å beskrive lisenser, kode og leveringskjeder innenfor åpen
kildekode-miljøet. Den definerer maskinlesbare markører for kodelisenser og kopirett.
Kildekode delt av NRK skal ha SPDX-markører i toppen av alle kodefiler.

Eksempel:

```
# SPDX-License-Identifier: MIT
# SPDX-FileCopyrightText: Copyright (c) Norsk rikskringkasting AS (NRK).
```

## Eierskap og vedlikehold

Tech-lead, eller tilsvarende rolle som forvalter teamets kildekode, skal ta stilling til hvordan vedlikehold av kodebrønnen skal gjennomføres. Dette skal dokumenteres i kildekoden, og være tydelig for eksterne bidragsytere.

Offentliggjøring av en kodebrønn skal skriftlig godkjennes av produkteier, eller tilsvarende rolle, før publisering.

Vi anbefaler at dette loggføres i et internt dokumentasjonsverktøy for teamet.

Det praktiske eierskapet til kildekoden ligger hos teamet.

### Språklige hensyn

Åpne kodebrønner og tilhørende dokumentasjon skrives på engelsk.

Selv om arbeidsspråket i NRK er norsk, ser vi at det vil være gunstig å bruke engelsk for å bidra til åpen kildekode der dette er sedvane.

Teamet kan selv vurdere å avvike fra dette om det er hensiktsmessig.

### Rutine for arkivering

Kodebrønner som ikke lenger vedlikeholdes, eller brukes aktivt av NRK, skal tydelig markeres som arkiverte kodebrønner. I Github skal "Archive" funksjonaliteten brukes, samt andre språkspesifikke arkiveringsmerknader.

En arkivert kodebrønn kan ved behov gjenåpnes. Det bør samtidig vurderes om eventuelle forgreninger (forks) kan ha verdi for videre forvaltning.

## Versjonering av kildekode

Det forventes at kildekoden versjoneres. Nåværende standard på prosjekter i
NRK er å bruke [semver](https://semver.org/).
