# Enclosure checklist

## Current direction: open-bench frame with two rows of WAGOs
- [x] Create an east/west-ear alternative without replacing the north/south-ear floor; a separate closed review shows the end-mounted ears.
- [ ] Confirm the 269.6 mm east/west-ear length against the original 10-inch maximum and the actual slicer build area; verify screw/plug access and mounting strength. The original-side-ear option is 106 mm wide and exceeds the original 3-inch width.
- [x] Model a proposed permanent wood-wall backer and assembled/exploded review views for the printed frame. The exploded review's floor holes are illustrative and do not modify the frame part.
- [ ] Before drilling or wall mounting, verify floor-hole and washer clearance against actual hardware and wiring, rear nut and spacer height, wood screw choice, and the expected load; the layout is not load-tested.
- [x] Model separate screw-down wood clips for the printed 76 × 88 mm open-frame box, plus a four-clip placement review. This does not modify the enclosure.
- [ ] Confirm actual box height and width, clip engagement, wood-screw fit, connector access, lid fastener strength and retention under expected loads; the mounting clips project beyond the original size limits and have not been physically verified.
The user elected to print the current build candidate without further coupon or pre-build physical testing. Unchecked items below remain open risks, not completed validations. See `PRINT-LIST.md` for the selected parts.
- [x] Explore two rows of three 221-415s, one above the other, with three +5 V above three ground and the 221-420s in a longitudinal floor row. Upper holders now rest on modeled rail concepts; WAGO bodies are approximate and mounts are untested.
- [x] Add schematic split-layout bundle paths, candidate tie locations and initial wire-diameter-based straight clearance samples. These are not a complete harness or exact wire paths.
- [x] Remove three redundant saddles while retaining the west tie rail, middle-post tie eyes, and three other added saddles.
- [x] Add two interior Ø3.6 mm tie through-eyes to each east corner support without opening the exterior wall or panel slide grooves. Actual tie access and strength are not tested.
- [x] Remove both supply-end saddles to eliminate their potential VLR rear-body interference. Use the east-support tie holes instead; the west saddle remains.
- [ ] Check actual cable-tie threading, harness fit, saddle strength, supply-connector clearance and WAGO lever access; the schematic paths do not prove these.
- [x] Replace recessed supply panels, overlapping guides and outer U-frames with full-height supply walls that use the same slide tracks as the plain walls. CAD shows split, dual-north and dual-south arrangements. The dual/blank review uses contrasting color for visibility.
- [x] Remove the full-height cylindrical lid posts and transfer their lid insert seats to short pads joined to the six wall tracks. Move the two center lid holes to match. The ceiling traps the slide panels; internal WAGO and rail screws remain.
- [x] Check the current `openFrameWestSlide.kcl`: its two legacy mounting holes are filled and the visible openings are the three XAD cutouts. The older `westPanelTall.kcl` still has the historical holes.
- [ ] Verify PETG slide fit, track/pad strength, heat-insert installation, long-wall flex, panel push-through and connector accessibility. The nominal panel-to-pad clearance is 0.2 mm; an engine intersection attempt failed and is inconclusive.
- [x] Place split 221-420 keeper concepts in the open-frame review at the 40 mm floor pitch. Remove the snap hooks from the 221-420 cradle, keeping its base, side rails, end stops and fastener locations. The 221-415 retainers are unchanged.
- [ ] Rework the unprinted 221-420 keeper: the user measured 0.59 mm between entry rows and 2.75 mm from one end to the nearest entry. A separate two-piece end-keeper candidate and single/pair review views are modeled; it assumes equivalent land at both ends and a flat contact at the simplified envelope top. Contact, land shape, retention under lever operation, wire and lever clearance, removal with terminated wires and mounting remain unverified. The hookless cradle does not independently prevent vertical removal.
- [ ] The full harness, WAGO lever access, west connector bodies, wire bends, all three supply layouts and actual print fit are not physically verified.
- [ ] Confirm the XAD contact part number and wire/crimp compatibility. The corrected 1.397 mm insulated OD is within the 0.8–1.9 mm range for SXAM-001T-P0.6, but below the 1.5 mm minimum for SXAM-01T-P0.6; the actual contact and crimp are unknown.
- [x] Measure the installed CN18 XADR-12V projection: 11.5 mm from the inside panel face to the wire exit. Updated the CN18 reference and signal approach.
- [ ] Deferred physical check: proceed with CAD assuming the CN18 dry fit works; this is not a passed test. Before finalizing, check the eight individual signals plus power/ground against the nearby upper 221-415 and lever movement. The slide-in west panel is now 3 mm farther out; bends and lever clearance remain unverified.
- [ ] Maintain the 10 × 3 × 3.5 inch maximum. Nominal printed-body envelope is approximately 239.6 × 76 × 88 mm. Check print tolerances, projecting non-countersunk screw heads and external connector projections; width has only 0.2 mm nominal margin.
- [x] Model two floor-mounted support rails for the upper WAGO row, with insert bores aligned to the retainer and floor mounting holes.
- [ ] Verify the rail concept's rigidity and 1.5 mm nominal outboard-leg-to-lower-retainer clearance, physical PETG fit, inserts, screw lengths and access, and the assumed 34 mm level pitch against real lever swing, wire exits and XMR housings. Check the last retainer's nominal 17.5 mm to the west panel against actual XADR rear housings and wiring before selecting a final layout.

## Earlier two-tier modular enclosure study
The following records the previous approach. The user has set aside the tray/transfer approach in favor of the open-bench frame; these items are historical, not the active plan.

- [x] Model 230 × 70 × 85 mm modular tray and interchangeable VL panels.
- [x] Execute the split, both-north and both-south CAD views.
- [x] Check representative VLR-to-WAGO wire reach on the taller bench setup.
- [x] User reports the short supply slide-guide coupon and panel fit fine; detailed retention and stop results were not specified.
- [ ] Rework 221-420 retention: a two-piece end-keeper concept follows the user's entry-face photos and measured 2.75 mm end land, but the simplified WAGO lacks real contact surfaces, wire entries and lever motion. Verify the assumed contact and physically test retention and access with representative wiring; do not print the concept yet.
- [ ] Address midspan flex. A candidate adds a center floor-bearing foot and a web between tiers, plus four corner spacers. Assess actual rigidity, web strength, lever and wire clearances, printability, fasteners and existing-tray fit before printing.
- [ ] Develop and verify the bench workflow. Trial risers now position the same guides at the tray-frame height on the bench, but the loose risers do not carry the wired assembly into the tray, and their stability is untested. All three layouts have raised static CAD views, and split also has a seated static view; wires, lid motion and full harness remain unvalidated. The VLR-06V panel physically slid down without a connector clash, with its wires resting above the WAGO; an approximate CAD sample warned of a potential clash during the opposite carrier-first-through-seated-panel motion. Design supported transfer, wire securing and service-loop space for 86.5 mm panel travel before a print request.
- [ ] For the final design, address long-wall flex (consider one mid-wall lid fastener per side) and verify panel retention under realistic connector insertion/removal. Keep the existing printed tray as-is for the current tests.
- [ ] Resolve full-height supply-panel fit and retention. The user reports loose panels and possible inward push-through with the lid off. With the lid in place the panels feel more secure, but the wall flexes when pushed; actual escape and whether the lid was fastened were not specified.
- [ ] Check the complete VLR-06V wire bundle, both VLR-02V leads and service loops in all three arrangements. Photos show a populated dual-input panel and carrier in the printed tray; the user confirms the lid closes without pinching the partial wiring shown. Complete-harness clearance and all-layout routing remain unconfirmed.
- [ ] Decide on a consistent retention approach for the two supply panels and the three-connector end panel; preserve the printed tray if practical.
- [ ] Check installed ceiling connectors, wires, west-panel assembly and fastener access.
- [ ] Confirm wire protection, branch fusing and actual electrical loads before energizing.

The original `main.kcl` remains the earlier non-modular design. The taller variant is shown in the `modularSupply...View.kcl` files. CAD execution and partial bench tests do not establish full assembly or electrical safety.
