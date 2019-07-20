# Ricette

## ricetta_01:

- Sito: https://it.wikipedia.org/wiki/Coste_italiane
- Tabella: Coste Italiane
- tag: table.wikitable

## script

```
curl "https://it.wikipedia.org/wiki/Coste_italiane" | scrape -be 'table.wikitable'| vd -f html
```

## risultato:
```
+------------------------+-----------------+------------------+
| Regione                | Km di costa [1] | Superficie (km²) |
+------------------------+-----------------+------------------+
| Toscana                | 397             | 22.987,04        |
| Veneto                 | 130             | 18.345,35        |
| Friuli Venezia Giulia  | 93              | 7.924,36         |
| Calabria               | 780             | 15.221,90        |
| Liguria                | 330             | 5.416,21         |
| Lazio                  | 360             | 17.232,29        |
| Sardegna               | 1.849           | 24.100,02        |
| Sicilia                | 1.637           | 25.832.39        |
| Marche                 | 185             | 9.491,38         |
| Molise                 | 35              | 4.460,65         |
+------------------------+-----------------+------------------+
```

## ricetta_02:

- Sito: https://www.tuttitalia.it/province/popolazione/
- Tabella: Province/Città Metropolitane per popolazione 2019
- tag: table.ut

## script

```
curl "https://www.tuttitalia.it/province/popolazione/" | scrape -be 'table.ut'| vd -f html
```

## risultato:

```
+------+-----------------------------------------+-----+-----------------------+----------------+----------------------+---------------+
| nro  | Provincia/Città Metropolitana           | Reg | Popolazione residenti | Superficie km² | Densità abitanti/km² | Numero Comuni |
+------+-----------------------------------------+-----+-----------------------+----------------+----------------------+---------------+
| 1.   | RM Città Metropolitana di ROMA CAPITALE | LAZ | 4.342.212             | 5.363,28       | 810                  | 121           |
| 95.  | SO Sondrio                              | LOM | 181.095               | 3.195,76       | 57                   | 77            |
| 83.  | LO Lodi                                 | LOM | 230.198               | 782,99         | 294                  | 60            |
| 84.  | TR Terni                                | UMB | 225.633               | 2.127,18       | 106                  | 33            |
| 44.  | TP Trapani [4]                          | SIC | 430.492               | 2.469,62       | 174                  | 24            |
| 9.   | CT Città Metropolitana di CATANIA       | SIC | 1.107.702             | 3.573,68       | 310                  | 58            |
| 70.  | MC Macerata                             | MAR | 314.178               | 2.779,34       | 113                  | 55            |
| 90.  | NU Nuoro                                | SAR | 208.550               | 5.638,02       | 37                   | 74            |
| 59.  | PU Pesaro e Urbino                      | MAR | 358.886               | 2.567,78       | 140                  | 53            |
| 86.  | CB Campobasso                           | MOL | 221.238               | 2.925,41       | 76                   | 84            |
+------+-----------------------------------------+-----+-----------------------+----------------+----------------------+---------------+
```