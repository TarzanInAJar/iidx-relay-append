# Wiring plan

User-supplied connections are recorded here as a working schedule, not a verified wiring diagram. Physical pin orientation and remaining connector pin assignments have not yet been specified.

## Eight-port +5 V ceiling row

Names run east/left to west/right. Connector types follow the previously supplied list in the same order; confirm before making cutouts.

| Position | Name | Connector |
|---:|---|---|
| 1 | STAGE | XMR-04V |
| 2 | 1P CABINET SIDE | SMP-04V-BC |
| 3 | 2P CABINET SIDE | SMP-04V-BC |
| 4 | COMPANE | XMR-04V |
| 5 | UPPER | XMR-04V |
| 6 | TP SIDE | SMP-04V-BC |
| 7 | 1P SIDE PILLAR | XMR-04V |
| 8 | 2P SIDE PILLAR | XMR-04V |

For every connector in this row, pin 1 is +5 V and pin 4 is GND. Pin 2 routes to the corresponding CN18 pin. Pin 3 is empty on all eight connectors.

| WAGO 221-415 pair | Ceiling connectors | Additional connection |
|---|---|---|
| A | STAGE, 1P CABINET SIDE, 2P CABINET SIDE | — |
| B | COMPANE, UPPER, TP SIDE | — |
| C | 1P SIDE PILLAR, 2P SIDE PILLAR | CN18-11 (+5 V) and CN18-9 (GND) |


## Six-port +12 V ceiling row

All are XMR-05V. The user confirmed the WOO, TT, and IC pair labels in row order. Left/right order within each pair remains provisional.

| Position | Name |
|---:|---|
| 1 | WOO1 |
| 2 | WOO2 |
| 3 | TT1 |
| 4 | TT2 |
| 5 | IC1 |
| 6 | IC2 |

For every connector in this row, pin 1 is +12 V and pin 5 is GND; the individual power and ground conductors have separate slots in the respective +12 V and GND 221-420 WAGOs. Pins 2–4 carry the west-stack connections listed below.

## Supply inputs

- North JST VLR-02V: pin 1 = +12 V; pin 2 = GND.
- South JST VLR-06V: pins 1–3 = +5 V; pins 4–6 = GND. Confirmed matched supply pairs: pins 1 (+5 V)/4 (GND) feed WAGO pair A; pins 2 (+5 V)/5 (GND) feed pair B; pins 3 (+5 V)/6 (GND) feed pair C.

## CN18 — top west XADR-12V

| CN18 pin | Connection |
|---:|---|
| 1 | STAGE-2 |
| 2 | 1P CABINET SIDE-2 |
| 3 | 2P CABINET SIDE-2 |
| 4 | COMPANE-2 |
| 5 | UPPER-2 |
| 6 | TP SIDE-2 |
| 7 | 1P SIDE PILLAR-2 |
| 8 | 2P SIDE PILLAR-2 |
| 9 | GND — third 221-415 GND connector |
| 10 | Empty |
| 11 | +5 V — third 221-415 +5 V connector |
| 12 | Empty |

The functions of the eight individual CN18-to-ceiling connections have not been specified.

## CN10 — middle west XADR-10V

| CN10 pin | Connection |
|---:|---|
| 1 | IC1-2 |
| 2 | IC1-3 |
| 3 | IC1-4 |
| 4 | IC2-2 |
| 5 | IC2-3 |
| 6 | IC2-4 |
| 7 | WOO1-2 and WOO2-2 |
| 8 | WOO1-3 and WOO2-3 |
| 9 | Empty |
| 10 | Empty |

CN10-7 and CN10-8 each feed the two WOO connectors. The user proposes daisy-chaining WOO pins 2 and 3; the physical first/second order and contact termination remain to be determined.

## CN19 — bottom west XADR-08V

| CN19 pin | Connection |
|---:|---|
| 1 | WOO1-4 and WOO2-4 |
| 2 | TT1-2 |
| 3 | TT1-3 |
| 4 | TT1-4 |
| 5 | TT2-2 |
| 6 | TT2-3 |
| 7 | TT2-4 |
| 8 | Empty |

CN19-1 feeds WOO pin 4 on both connectors; the user proposes daisy-chaining these pins. Confirm the chosen XMR contact and crimp are approved for two wires before putting two wires in one contact. If a two-wire crimp does not work out, the user will use an appropriately rated inline splice with a single wire per connector contact. Allow space for all three inline splices if needed.

Do not infer physical pin locations from numbers; connector views/orientations and the supply-return topology remain to be confirmed.
