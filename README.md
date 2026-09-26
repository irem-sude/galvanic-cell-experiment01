## Setup

**Electrolyte (NaCl solution):**
- Container weight: 715 g
- Water used: 970 g
- Salt used: 30 g
- NaCl concentration: 3.00% (w/w)

## Observations

| Time | Elapsed under load | Voltage at 15th min (mV) | Notes |
|---|---|---|---|
| 17:04 | – | 812 | Initial open-circuit voltage |
| 20:04 | 3h | 814 | Dropped briefly below open-circuit under load, then recovered; propeller spun briefly when motor was reconnected |
| 23:04 | 3h | 835 | Same pattern as above: brief dip and recovery, propeller spun briefly |
| 02:04 | 3h | 812 | Coating continued peeling |
| 13:43 | 11h 39min | 451 | Zinc coating mostly gone, steel exposed; rust visible on bolt |
| 18:00 | 4h 17min | 457 | Bolt significantly rusted |
| 00:00 | 6h | 527 | Electrolyte turned yellow; almost no coating left except a few small spots |

Note: The explanations below are qualitative interpretations based on general electrochemistry principles (mixed potential theory, polarization phenomena), not confirmed by additional diagnostic methods (e.g. reference electrode, EIS). They represent the most plausible explanation for the observed data, not proven mechanisms.

1. Reversible dips under load (e.g. 812 → ~606 mV, recovering within minutes once the load is removed) are consistent with polarization effects under current flow    - likely some combination of activation, ohmic, and concentration polarization. With the equipment used (no reference electrode, no current-interruption            technique), these three contributions cannot be separated. What can be said is that all such effects are reversible at (near-)zero current, which matches the      observed recovery: since the multimeter draws negligible current, voltage returns close to the open-circuit value almost immediately after disconnecting the       load.    This was also confirmed physically - the propeller spun briefly each time the motor was reconnected, showing real current was being drawn.

2. The permanent drop after ~9-20 hours (readings staying near 450-530 mV even 15 minutes after reconnecting the near-infinite-resistance voltmeter) cannot be        polarization, since polarization would relax within seconds at open circuit, not persist. A more likely explanation is a change in electrode identity: as the      zinc coating wore through unevenly, the nail's surface became a patchwork of remaining zinc and exposed steel. The open-circuit potential of a single              homogeneous electrode is independent of its surface area, but a patchy, mixed-metal surface produces a mixed potential that shifts toward whichever metal          dominates the exposed area - in this case, increasingly toward steel as coating loss progressed. This is consistent with the small remaining zinc patches still    visible on the nail without fully restoring the original zinc-copper voltage.

3. **Comparison with standard electrode potentials.** Using standard reduction potentials
   (Cu²⁺/Cu = +0.34 V, Zn²⁺/Zn = -0.76 V, Fe²⁺/Fe = -0.44 V), the theoretical cell
   voltages would be ~1.10 V for a zinc-copper pair and ~0.78 V for an iron-copper pair.
   The measured values (≈812 mV initially, ≈450-530 mV after the coating wore through)
   are consistently lower than both theoretical values by a similar margin. This is
   expected given the non-standard conditions used here: standard potentials assume
   1 M ion concentrations and pure metal electrodes at 25°C, while this experiment used
   a 3% (w/w) NaCl solution and a galvanized (not pure) zinc coating over steel. The fact
   that both readings deviate from theory by a comparable amount - rather than randomly -
   supports treating the drop as a genuine shift from a zinc-copper to an iron-copper
   couple, not measurement noise.

      *Standard reduction potential values (Cu²⁺/Cu = +0.34 V, Zn²⁺/Zn = -0.76 V,
   Fe²⁺/Fe = -0.447 V) from Chemistry LibreTexts, an open academic chemistry resource:
   https://chem.libretexts.org/Courses/Smith_College/Advanced_General_Chemistry/11%3A_Appendices/11.12%3A_Standard_Electrode_(Half-Cell)_Potentials*

4. **Electrolyte turning yellow** toward the end of the experiment is consistent with
   dissolved iron corrosion products (Fe³⁺/Fe²⁺ species, or early-stage rust) entering
   the solution as the exposed steel corroded. This wasn't quantified (e.g. no pH or
   ion concentration measurement), but it's a visual confirmation that the underlying
   steel was actively corroding, not just passively exposed.

   ## Limitations

- Single trial, no replicate measurements
- Ambient temperature not controlled or logged (the experiment ran ~31 hours,
  spanning day and night, which could add uncontrolled thermal noise to the readings)
- No reference electrode used, so absolute electrode potentials (only the overall
  cell voltage) were measured
- Coating condition (zinc vs. exposed steel) assessed visually, not quantified
  (e.g. no microscopy or image analysis of surface coverage)
