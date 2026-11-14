# Test prints

- `clearanceFixtureBase.kcl` — printable fixture base.
- `clearanceFixtureLid.kcl` — printable XMR-05V fixture lid.
- `ceilingFitCoupon.kcl` — printable 76 × 48 × 3 mm sample of the first ceiling connector positions: one XMR-04V and two SMP-04V-BC in one row, with two XMR-05V in the other at the actual 24 mm pitch and 24 mm row spacing. The openings and underside reliefs match `../ceiling.kcl` as modeled.
- `vlFitCoupon.kcl` — printable 84 × 34 × 3 mm sample with VLR-02V and VLR-06V openings and rear reliefs as modeled in `../tray.kcl`. The two openings represent separate walls and their spacing on this coupon is not an assembly feature.
- `main.kcl` — module interface for the review view; not a print part.

The assembled review is `../clearanceFixtureView.kcl`. The accepted WAGO retainer models remain in the project root because the enclosure assembly also uses them; reuse the existing printed 221-420 retainer with this fixture.

Print the two fit coupons in PETG with the flat exterior face on the bed and the rectangular relief pockets facing up. The ceiling coupon's exterior is its z = 3 mm face, so flip it in the slicer; the VL coupon's exterior is its z = 0 mm face. On the ceiling coupon, orient the narrow XM steps and the SM keys up when looking at the exterior: XMR-04V is the leftmost opening in the three-port row, the next two are SMP-04V-BC, and the two-port row is XMR-05V. On the VL coupon, the smaller opening is VLR-02V and the larger VLR-06V.

Test all connectors unpowered for insertion, seating, latch retention and removal, and use mating plugs to check release access at the real ceiling spacing. Coupons reproduce local opening shapes and reliefs only; they do not test tray, carrier or wiring clearances. Their copied dimensions must be synchronized if the corresponding production panels change.

The connector envelopes in the review are references only. See the clearance-fixture section of `../NOTES.md` for setup, print orientation and test limitations.
