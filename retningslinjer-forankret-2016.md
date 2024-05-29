# Retningslinjer for deling av åpen kildekode

## Hvorfor deler vi ut kode?

1. kodeproduksjon er lisensfinansiert og bør gis tilbake på lik linje med tv/radio-innhold
1. økt samarbeid med en hardt prøvet mediebransje
1. som konsument av annen åpen kildekode, bør vi dele tilbake
1. økte kvalitetskrav når koden synliggjøres
1. mer modulære kodebaser som forbedrer mulighet for gjenbruk også internt
1. gratis feedback og forbedringer fra community
1. rekruttering og markedsføring av NRK

## Fallgruver

1. **Juridisk**: deling av prosjekter som bruker andre komponenter som ikke tillater videredistribusjon
1. **Abandonware**: kode som er publisert krever oppfølging (issues, PRs)
1. **Breaking changes**: krever et strikt versjoneringsregime
1. **Hemmeligheter**: kode (og commitmeldinger) som inneholder informasjon om brukernavn, passord, infrastruktur
1. Roller: utviklere må opptre som representanter for NRK

## Hva slags type kode deler vi?

1. gists; dvs. mindre kodesnutter (MIT-kommentar i toppen)
1. bugfixes og forbedringer (PR) på andre open source prosjekter vi bruker
1. utilities, plugins, widgets, byggescript (MIT lisens)
1. komplette systemer, uten strategisk betydning (GPL lisens)
   - Dvs. det finnes tilsvarende systemer fra før, men som er løst annerledes av NRK

## Hva slags type kode deler vi ikke?

1. Konfigurasjon av brukernavn, passord, domenenavn
1. Komplette systemer med strategisk betydning
   - Dvs. det finnes ingen andre systemer som er løst slik NRK har gjort det og er konkurransemessig viktig

## Hvordan deler jeg min kode?

1. Koden skal deles på http://github.com/nrkno
1. Prosjektleder / produkteier får rollen som github-admin for sitt team/prosjekt og får bestemme om koden skal deles eller ei
1. Prosjektleder / produkteier har ansvar for å melde ut brukere av nrkno-organisjonen når de slutter i NRK
1. Utviklere bruker sin private github-konto og får tilgang til nrkno-organisasjonen av prosjektleder / produkteier
1. Utviklere må følge opp PR og issues som meldes inn. Tidsbruk på dette samordnes med prosjektleder / produkteier.
1. Koden skal kvalitetsikres for fallgruver av annen utvikler/team, i samråd med prosjektleder/produkteier. Der det oppstår faglig uenighet kan fagansvarlige og utviklingssjef involveres.
1. Pakken skal publiseres på dertil egnet kodesentral

   - NPM for javascript
   - NuGet for .NET
   - Maven centrail for Java
   - RubyGems for Ruby
   - PyPi for Python
   - DockerHub for Docker
   - … etc

## Sjekkliste for delt kode

1. Vi skriver på engelsk
1. Readme-fil som forklarer hensikten med repoet, hvordan man kommer igang, hva som kreves etc
1. License.txt og copyright-kommentar i alle eksporterte kode-/tekstfiler
1. Koden skal versjoneres vha av tag-er, med bruk av semantisk versjonering
   - vMajor.Minor.Patch (les mer på http://semver.org/)
     - Major = API-endringer som ikke er bakoverkompatible
     - Minor = API-endringer som er bakoverkompatible
     - Patch = API-endringer som bare retter bugs
1. God testdekning, både for kvalitetsikring av kodebase, økt tillit hos konsumenter og forenkling av PR-håndtering.
1. Tools for CI, tester, coverage og badges (gratis for åpne prosjekter)
   - http://travis-ci.org eller https://ci.appveyor.com för CI / automatiska tester skall vara på plass
   - https://coveralls.io/ - code coverage är nice to have beroende på omfanget av projektet.
   - http://shields.io/ - skapa "badges" med linker till npm/nuget/travis/coveralls etc.
1. Hvis koden er av typen GPL, skrive en artikkel på http://nrkbeta.no/dev for å markedsføring av prosjektet. MIT-prosjekter kan også omtales på nrkbeta, men det er ikke påkrevet

## TLDR; om lisenser

1. Hva er en MIT-lisens (https://tldrlegal.com/license/mit-license)?

   - koden kan fritt brukes, endres og distribueres og inkluderes i åpen/lukket kode
   - konsument må inkludere copyright-teksten og lisens der den benyttes.
   - Eksempler: jQuery, Ruby on Rails, Node.js, Lua

2. Hva er en GPL-lisens (https://tldrlegal.com/license/gnu-general-public-license-v3-(gpl-3))?
   - koden kan fritt brukes, endres og distribueres, men versjonshistorikken må beholdes
   - konsument må inkludere copyright-teksten og lisens der den benyttes.
   - Prosjekter som bruker GPL-lisensiert kode må videredistribueres under GPL-lisens
   - Eksempler: Linux kernel, MySql

## Inspirasjonskilder

Internasjonale organisasjoner

- https://github.com/bbc
- https://github.com/guardian
- https://github.com/NYTimes
- https://github.com/voxmedia
- https://github.com/associatedpress
- https://github.com/PressAssociation
- https://github.com/channel4
- https://github.com/huffpostdata
- https://github.com/TimeMagazine
- https://github.com/BuzzFeedNews

Nordiske organisasjoner

- https://github.com/SVT
- https://github.com/sverigesradio
- https://github.com/TV4
- https://github.com/drdk
- https://github.com/Yleisradio
- https://github.com/finn-no
- https://github.com/amedia
- https://github.com/Aftenposten
- https://github.com/BergensTidende
- https://github.com/Aftonbladet
- https://github.com/Jyllands-Posten
