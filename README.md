# AMQ Artemis

Fagarbeid prosjekt - Ønsker å bli bedre kjent med Artemis.

## 24.09.20 - Dag 1
Veldig tydelig at det er en del forskjeller mellom AMQ classic og 
Artemis når det kommer til oppsett av brokere.

Classic setter opp en AMQ dir hvor man finner alt av oppsett og executables osv, 
mens for Artemis har man en hoved dir, men oppretter en egen lokasjon for brokeren
med innstillinger osv.

Tar en 180 og sjekker ut docker containers for å sette opp brokerne. 
Blir litt mye rot å ha hele Artemis liggende i et repo.

### Docker
Docker fungerer ganske bra for å sette opp to Artemis instanser i en fei.
Videre blir å endre oppsett med persistant volumes og mekke en bitteliten komponent 
(Spring Integration?) som kan produsere og sende meldinger via brokerne.

### Interessante funn
Enn så lenge ingen.
Ønsker å teste ut følgende:
1. Kan man få begge brokerne inn i samme GUI uten ekstremt mye mikkmakk 
(ser at det er mulighet for å legge til remote brokers, men antar dette gjøres via 
cookies som ikke er en god løsning)
2. Hvordan man setter opp nettwork of brokers for Artemis.
3. Under `Artemis -> Queues` er det en rekke filtreringsmuligheter (bl.a. User) 
som jeg er nysgjerrig på hvordan fungerer. Hvis dette lar en somehow tagge queues med 
users kunne dette vært beleilig for fremtidig bruk.

