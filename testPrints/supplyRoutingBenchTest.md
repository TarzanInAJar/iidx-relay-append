# VL supply-routing bench check

This is a temporary, unpowered check of the taller modular-panel layout using existing prints; no new print is required. `../supplyRoutingBenchView.kcl` shows the proposed 230 × 70 × 85 mm envelope: the blue VL coupon, red approximate 06V rear, purple approximate 02V rear, and simplified WAGO bodies and XMR-05V rear bodies. The lid is a floating reference at the proposed height, not an existing taller tray. The view shows four upper retainers for context even if only one of each has been printed. Change `northTrial` in the view from 0 to 1 to compare both-north with both-south; the split arrangement is not shown simultaneously. Connector and WAGO boxes are simplified; supports, the tray, other ceiling connector bodies and wiring are not represented. Do not print the view or energize a mockup.

## Setup
- Use the assembled two-tier carrier, the accepted 221-415 retainer and WAGO on the upper tier, and the existing `vlFitCoupon` with both VL housings installed. The final upper tier has 221-415 positions at x = −54 and −18 mm and 221-420 positions at x = 18 and 54 mm. Move the 221-415 between its two positions if only one is available. The carrier's long direction is x; the −54 mm end is the enclosure's east/left end.
- Stand the VL coupon vertically with its keys up and the recessed face and connector backs facing the carrier. Hold it with temporary supports; do not clamp wires. The coupon has the same 40 mm port-center spacing as the proposed dual panel, though it does not reproduce the guide, panel perimeter or adjacent walls.
- Set the coupon's inner/recessed face 31 mm from the carrier centerline, measured across its width: nominally 11 mm outboard of the straight edge of the 40 mm-wide upper plate, not its projecting tie tabs. Place the coupon center along the carrier in line with the upper 221-415 position at x = −54 mm; the true staged panel center is x = −53.8 mm. Thus the VL opening centers are approximately x = −74 and −34 mm.
- Set the opening centers 20 mm above the upper carrier's top face (z = 51.5 mm in the taller trial), or the top edge of the 34 mm coupon 37 mm above that face. This is 8.5 mm higher than the earlier low-position trial. The proposed lid underside is 50.5 mm above the upper plate (z = 82 mm). Do not infer clearance for real ceiling connectors or their wires from a flat lid reference alone.

## Positions to check
With the housing backs facing into the carrier and keys up, use the appropriate side of the carrier. Orient the coupon so the housings occupy the positions listed; the rear recesses must remain inward.

| Configuration | Side | x ≈ −74 mm | x ≈ −34 mm |
| --- | --- | --- | --- |
| Both south | South | VLR-06V | VLR-02V |
| Both north | North | VLR-02V | VLR-06V |
| Split | South | VLR-06V | Not used |
| Split | North | VLR-02V | Not used |

The split case can be checked one side at a time, but cannot demonstrate interaction of the two loose panels or common service loops. The coupon is reversible for these trials: rotate its installed panel arrangement as needed while keeping the connector backs inward and keys up.

## What to observe
- With the setup unpowered, start with one or two properly terminated representative 22 AWG leads at the tightest VL exit. If those cannot leave and route gently, stop rather than forcing them. If promising, test all six conductors in the 06V and both in the 02V. Route the 06V conductors to the three +5 V/GND WAGO pairs on the two tiers; route the 02V conductors toward the two upper 221-420s. Keep each intended supply and return group separate. Do not make permanent-length cuts until service loops are assessed.
- Look for tight turns at wire exits, contact with WAGO bodies and retainer hooks, insulation pinching, lever/tool access, and space for six wires to fan out. Test a gentle vertical panel insertion/removal motion without pulling on or trapping the wires. Check both adjacent connectors and mating-plug release access.
- Use the existing ceiling fit coupon with representative connectors at the local ceiling positions if practical. A plain horizontal lid reference is not a substitute for connector bodies and wires. The test does not prove full-harness, guide, opposite-wall, west-panel, or final lid assembly clearance.
- Compare with the earlier 11.5 mm center height only if useful; the user reported little space in a nearby lower position. The 20 mm center height and 85 mm overall box are a model proposal, not an accepted panel or finished tray. Nearby ceiling connector bodies and their wires, mating access, top edge, guide, and actual service loops must still be checked. Do not force a bend to make either position fit.

Record which side and port position is tight, what contacts or binds, whether the panel can move with slack, and a photo from the side and above. Both actual connector projection datum and the measured 17.07 mm distance still require confirmation; the CAD references conservatively extend 18.7 mm from the panel inner face.
