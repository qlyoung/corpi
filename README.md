# corpi
fuzzing corpuses

Repository map
--------------
Some information on the pedigree of various corpi in this repo.

- bgp: BGP packets
- bgp/basic: Handcrafted BGP packets, one for each of the defined message types. Each of these originate from AS 10, 10.0.1.1. No IP headers.
- bgp/bird: Corpus generated from fuzzing BIRD in state `OpenSent`.
- bgp/bgpd: Corpus generated from fuzzing FRRouting's `bgpd`, in state `Established`.
- zebra/zapi: Corpus generated from fuzzing FRRouting's `zebra` daemon on its IPC surface, which uses the `ZAPI` protocol.
