# Open-frame enclosure — print list

This is the selected open-frame build candidate, not a physically verified final assembly. The user elected to proceed without more coupon tests. Print the individual part files below—not the review views, `testPrints`, or the root `main.kcl`, which is the older non-modular enclosure. Quantities are for one box; reuse acceptable retainers already printed where possible.

## Common parts

Use the current `floorFrame.kcl` for the corner tie holes, `openFrameCeiling.kcl` for non-countersunk screws, and `wagoTenRetainer.kcl` for the hookless 221-420 cradle. Earlier 221-420 prints have snap hooks; print two of the current cradle if you want the simplified version.

| Quantity | KCL file | Part and purpose |
|---:|---|---|
| 1 | `concepts/openFrameBench/floorFrame.kcl` **or** `floorFrameEndEars.kcl` | Floor with panel seats, lid insert pads and tie holes; choose north/south ears (first file) or east/west ears (second), not both |
| 1 | `openFrameCeiling.kcl` | Connector ceiling with six Ø3.4 mm screw through-holes, no countersinks |
| 2 | `concepts/openFrameSlideWalls/plainSide.kcl` | Plain long-wall slide panels |
| 1 | `concepts/openFrameSlideWalls/eastPanel.kcl` | Blank short-wall slide panel |
| 1 | `openFrameWestSlide.kcl` | Three-opening XAD slide panel; no panel screws |
| 2 | `concepts/upperWagoRail/main.kcl` | Upper 221-415 row mounting rails; two legs per rail |
| 6 | `wagoFiveRetainer.kcl` | Three lower and three upper 221-415 retainers |
| 2 | `wagoTenRetainer.kcl` | Hookless lower 221-420 cradles; require the separate keeper halves for intended lift restraint |
| 4 | `concepts/tenEndKeeper/main.kcl` | Two keeper halves for each 221-420; rotate one half 180° in assembly. Contact and retention are unverified. |

### Floor mounting choices

- `concepts/openFrameBench/floorFrame.kcl`: four north/south ears; 239.6 × 106 mm floor footprint.
- `floorFrameEndEars.kcl`: four east/west ears; 269.6 × 76 mm floor footprint. `openFrameEndEarReview.kcl` is a review, not a print part.
- Each has four Ø5 mm screw holes accessible with the lid on. Both exceed an original footprint limit when ears are included. Check slicer build area, actual plug/driver clearance and mounting strength; the alternatives have not been physically validated.
- The previously printed earless floor remains unchanged. `slidePanelRetrofitStop.kcl` is a separate retrofit, not required for either newly printed floor.

### WAGO mounting versus the earlier carriers

The open-frame assembly does **not** use the earlier removable carrier plates, including `centerSupportedCarrier.kcl` and `upperCarrierFourPost.kcl`. Instead, the frame floor mounts the two 221-420 retainers and three lower 221-415 retainers directly. The two upper WAGO rails carry the other three 221-415 retainers. Each upper rail has two legs, not a middle leg; its rigidity has not been verified. All eight individual retainers are still screwed in place.

### Pick ONE supply-wall set

- **One supply connector on each long wall:** `openFrameSupplyTwo.kcl` ×1 and `openFrameSupplySix.kcl` ×1.
- **Both supply connectors on either long wall:** `openFrameSupplyBoth.kcl` ×1 and `openFrameSupplyBlank.kcl` ×1. Swap sides to choose north or south; the other long wall is blank.
- To retain all three layout choices, print all four files above, one each. The two plain long walls listed above are still needed.

That is 22 printed parts for one layout, including all four end keepers. Two extra panels enable the other layout choices.

### Optional mounting and bench aids

- `woodMountClip.kcl` ×4 secure the assembled box to a wood surface: two clips on each long side, each held by a wood screw through a nominal Ø4.8 mm hole. The clips capture the ceiling edge and require removal for lid access. They assume an 88 mm box height and 76 mm width; fit, load capacity and real connector clearance are unverified. With clips the nominal width is about 116.7 mm and the height about 91.6 mm, exceeding the box-only 3 × 3.5 inch limit. `woodMountReview.kcl` is a placement view, not a print part.
- `openFrameCeilingCradle.kcl` ×2 hold the ceiling upright while wiring. They are not installed in the enclosure. Clamp or strap the ceiling so it cannot tip; do not let it hang by the wires. Alternatively use your own secure bench supports.

## Orientation and slicer guidance

- Material: PETG. The user's 0.4 mm nozzle is a reasonable starting point; these are not verified slicer settings.
- **Frame:** Place its broad bottom on the build plate with tracks upright. Mesh screening found horizontal overhangs beneath the six upper lid pads, and parts of the track bases (earlier frame revision). Use slicer-generated support where needed, including support starting on the frame where appropriate. Keep the panel slide channels and insert holes accessible for cleanup.
- **Upper WAGO rails:** In the upright orientation, the long rail and projecting feet have downward overhangs. Use supports under these surfaces and inspect their removal and insert holes in preview; the two narrow leg bottoms alone have limited bed contact. An alternative orientation is possible but has not been validated for strength or fit.
- **221-420 end keepers:** The broad outside face of the tall side wall can lie against the build plate. A sampled mesh check of this orientation found no unsupported islands, but flagged small overhangs; inspect the horizontal screw hole and contact pad in the slicer. The as-modeled foot-down orientation has a small unsupported pad island.
- **Ceiling:** Place the outside face—the face opposite the connector latch recesses—against the build plate, with the larger connector latch recesses facing upward. Do not print vertically. Inspect screw through-holes and connector openings in the layer preview.
- **Supply panels:** Lay the outside face flat on the bed, connector latch recesses upward. The narrowed slide edges face upward as well.
- **West XAD panel:** Lay the outside face flat on the bed, with the latch reliefs upward. The plain long and short panels can also be laid flat.
- **Wood-mount clips:** Lay one broad side face of each clip flat on the bed, not upright on the screw foot. Inspect the 4.8 mm mounting hole and the top lip in the slicer preview.
- **Retainers:** Place their broad mounting bases on the bed. Preserve the 221-415 retainers' small snap lips and inspect overhangs in the slicer; the revised 221-420 cradles have no snap lips. The optional ceiling cradles print with their broad solid base down and slots upward.
- Check the actual build area in Bambu Studio for the selected nozzle(s), support and bed arrangement. The ceiling and north/south-ear frame are approximately 239.6 mm long; the east/west-ear frame is 269.6 mm long. Orient the length along bed Y if using both X2D nozzles and needed to fit the narrower X direction; confirm the complete job in the slicer.

The mesh screening used 0.2 mm layer sampling and a 45° overhang threshold measured from the build plate. It is not a slicer simulation or print-success/strength certification.

## Hardware (not printed)

- **26 × Bambu AB012 M3 heat-set inserts:** 6 lid pads, 10 lower retainer mounting points, 4 upper-rail feet and 6 upper retainer mounting points in the rails. The 4.4 mm insert-hole size follows the user's earlier PETG coupon result. Install inserts square and flush; do not melt through thin bore bottoms.
- **26 × M3 screws, if all modeled mounting points are used:**

  | Location | Count | Breakdown |
  |---|---:|---|
  | Ceiling | 6 | Six non-countersunk M3 screws; heads sit above the lid |
  | 221-415 retainers | 12 | Six retainers × two screws each; three on the floor and three on the upper rails |
  | 221-420 retainers | 4 | Two retainers × two screws each; the four keeper halves share these screws |
  | Upper rail feet | 4 | Two rails × two screws each |
  | **Total** | **26** | No separate wall-panel or keeper screws |

  The CAD does not model the screws. Lengths, head sizes, engagement and driver access have not been finalized or verified; select the hardware for each stack without bottoming out or protruding through the floor.
- Cable ties for the middle-post holes and corner columns. Each corner column has two nominal Ø3.6 mm interior through-holes; thread narrow ties before installing the wall panels. Check actual tie fit, threading and strength. No additional screws or printed parts are required. The colored routing and bundle lines in the review views are diagrams, not printed parts or cut lengths.

## Assembly and limitations

Use `BENCH-WIRING.md` for bench assembly and `WIRING.md` for the connector pin map. Slide the supply and west panels in before wiring; wire and dress the exposed frame with the ceiling supported, then insert the remaining walls and fasten the ceiling. The ceiling retains all six slide-in walls; no individual exterior panel screws are used.

The nominal enclosure body without mounting ears is approximately 239.6 × 76 × 88 mm. Including the integral floor ears, the north/south variant is 239.6 × 106 × 88 mm and the east/west variant is 269.6 × 76 × 88 mm. These exclude external mating connectors, wires, screw-head projection and print dimensional variation. The projecting screw heads must fit within the remaining 0.9 mm if the 3.5-inch limit includes hardware. Only 0.2 mm of nominal width remains under the requested 3-inch limit. The frame, complete wiring, all three supply configurations, panel retention/flex, upper rail strength, driver access, 221-420 end-keeper contact and retention have not been physically verified. The hookless 221-420 cradle alone does not retain the connector against lifting; the keeper halves are intended to do so but must be checked for contact, wire/lever clearance and retention. The modeled panel-to-pad clearance is only 0.2 mm; a prior CAD intersection attempt was inconclusive. The user accepts these risks rather than printing more coupons. Inspect the actual assembled unit with power disconnected, and make sure external fusing protects the installed conductors and connectors before energizing.
