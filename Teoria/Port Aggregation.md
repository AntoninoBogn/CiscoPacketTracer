\### PORT AGGREGATION ###



In Cisco Packet Tracer, fare port aggregation (chiamato anche EtherChannel o Link Aggregation) serve per unire più interfacce fisiche (di due switch) in un unico collegamento logico, così da ottenere diversi vantaggi in una rete simulata (e anche reale).



Ecco i principali motivi:



* Aumento della banda
* Ridondanza e resilienza
* Migliore gestione del traffico
* Scalabilità



\## Come Fare ##



en

conf t

interface range f0/1-4 /> cosi prendiamo un range delle interface

switchport mode access

switchport access vlan 100 -> assegniamo vlan

interface f0/1-4 => seleziono di nuovo range

channel-group 6 mode ? -> con il punto interrogativo vedo le opzioni disponibili

channel-group 6 mode desirable

\###sul secondo switch faccio lo stesso procedimento pero al channel-group mode metto auto ###



