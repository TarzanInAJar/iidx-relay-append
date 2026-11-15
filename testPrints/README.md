# Test prints

- `clearanceFixtureBase.kcl` — printable fixture base.
- `clearanceFixtureLid.kcl` — printable XMR-05V fixture lid.
- `ceilingFitCoupon.kcl` — printable 76 × 48 × 3 mm sample of the first ceiling connector positions: one XMR-04V and two SMP-04V-BC in one row, with two XMR-05V in the other at the actual 24 mm pitch and 24 mm row spacing. The openings and underside reliefs match `../ceiling.kcl` as modeled.
- `vlFitCoupon.kcl` — printable 84 × 34 × 3 mm sample with VLR-02V and VLR-06V openings and rear reliefs as modeled in `../tray.kcl`. The two openings represent separate walls and their spacing on this coupon is not an assembly feature.
- `insertFitCoupon.kcl` — 60 × 9 × 7 mm insert-test strip for the user's AB012 M3 × 5 × 4 inserts. Four nominal blind-hole diameters, from the end with the tiny marker hole: 4.3, 4.4, 4.5 and 4.6 mm; each is 5.2 mm deep. The strip width matches the existing carrier-post diameter but is not the same boss geometry; sideways-printed west-panel holes are not represented.
- `sideInsertFitCoupon.kcl` — 8 × 60 × 12 mm coupon with the same four blind-hole trial diameters and 5.2 mm depth, arranged horizontally to compare sideways-printed holes. Its top marker hole identifies the 4.3 mm end. This rectangular block does not reproduce actual west-boss geometry, support needs or insertion access.
- `main.kcl` — module interface for the review view; not a print part.

The assembled review is `../clearanceFixtureView.kcl`. The accepted WAGO retainer models remain in the project root because the enclosure assembly also uses them; reuse the existing printed 221-420 retainer with this fixture.

Print the two fit coupons in PETG with the flat exterior face on the bed and the rectangular relief pockets facing up. The ceiling coupon's exterior is its z = 3 mm face, so flip it in the slicer; the VL coupon's exterior is its z = 0 mm face. On the ceiling coupon, orient the narrow XM steps and the SM keys up when looking at the exterior: XMR-04V is the leftmost opening in the three-port row, the next two are SMP-04V-BC, and the two-port row is XMR-05V. On the VL coupon, the smaller opening is VLR-02V and the larger VLR-06V.

Test all connectors unpowered for insertion, seating, latch retention and removal, and use mating plugs to check release access at the real ceiling spacing. Coupons reproduce local opening shapes and reliefs only; they do not test tray, carrier or wiring clearances. Their copied dimensions must be synchronized if the corresponding production panels change.

For the insert-fit strips, print in PETG using the intended final print settings. Place `insertFitCoupon.kcl` flat with its four blind openings up. Print `sideInsertFitCoupon.kcl` on its 8 × 60 mm bottom (z = 0), with its four insert openings horizontal and the small marker hole vertical. Inspect horizontal holes for drooping and avoid support material inside them if practical. Trial diameters are not specified by Bambu; test seating and retention with the actual inserts and screws after cooling. Do not drill out the holes before judging the printed fit.

The connector envelopes in the review are references only. See the clearance-fixture section of `../NOTES.md` for setup, print orientation and test limitations.
