# Hidden States and Unassigned Work

Physical questions and signed work behind higher-order coefficients

This companion develops the twelve physical questions marked in [*Third- and Higher-Order ODEs*](https://github.com/hobnilre/physics-ode-3rd-deg). That article constructs higher-order coefficient laws; this one develops their physical comparisons, hidden-state observations and signed energy accounts. The rotary impact driver is the principal example, linking contact and joint identification to the energy left at release.

The six main sections follow that comparison from its physical questions and signed-work conventions through contact/joint identification, release, measurement conclusions and the remaining scope. Six appendices in the same PDF retain the complete supporting systems, finite implementations and uncertainty calculations. The guide after the conclusion and the configuration lookup in the measurement appendix provide direct access to the detailed cases.

## What this article adds, and why it matters

The coefficients describe a declared physical system. Which internal states do its measurements identify, and where does energy go when contact releases, a return wire changes or a controller acts? Exact constructions give distinct predictions and the observations that separate them. Encoders, torque sensors, voltage probes and current shunts make the leading comparisons accessible on slow, low-voltage laboratory models.

- **Which part carries the additional dynamics?** Synchronized hammer and anvil angles and torque measurements separate contact from joint response. Controlled electrical shunts provide a complementary voltage–current and phase comparison. Independent component changes test whether a coefficient law belongs to the proposed physical part and predicts the connected system.

- **Energy remains when an impact releases.** A slow hammer–anvil rig uses synchronized encoders and contact torque to follow the deformation through release. In one exact collision, force-zero detachment leaves a positive spring store of $e^{-\pi}\,\mathrm{J}$. A retained material-state model predicts delayed relaxation and $e^{-\pi}/4\,\mathrm{J}$ remaining after $\log2\,\mathrm{s}$. Repeated impacts must carry residual strain and heat or include a measured reset. Different separation laws change both restitution and the energy left at release; fracture, acoustic, thermal and fixture measurements distinguish the possible destinations.

- **A quiet terminal can hide changing energy.** A three-state RC loop carries equal-and-opposite capacitor voltages while its loop current stays zero. Branch voltage and shunt measurements reveal the resistor transfers. A finite-coupling bound shows exactly what terminal uncertainty says about hidden energy—and what additional preparation and coupling information it needs.

- **A vanishing state can carry finite energy.** A prepared capacitor family retains finite initial energy while capacitance and charge tend to zero. The work released depends on the ratio of switching duration to discharge time. A finite example drops from $2$ to $1/2\,\mathrm{mJ}$, exposing the transfer that a reduced model can discard along with its initial state.

- **Equal final voltages leave individual switch work undetermined.** Reversing two connection channels exchanges their signed works, $-3/4$ and $-3/16\,\mathrm{mJ}$, while both capacitor endpoints stay the same. Simultaneous connection gives a third partition. Complete finite transformer return paths retain both winding currents, the output capacitor, clamp, two return channels and eight separate work integrals. Equal source durations still give a strictly nonzero difference in old-return work.

- **A real probe changes the circuit.** Explicit isolated and tapped transformer graphs include return conductances, interwinding and chassis capacitances, and probe loading. A finite probe draws a strictly positive work from a prepared state. Synchronized channels and independently measured magnetic and electric endpoints test whether one calibrated model predicts both connections.

- **Bias-coil energy can increase with the plant drives and external charger off.** An exact controlled transducer transfers actuator reaction work into its controller while the bias coil gains stored energy. A different receiving path gives identical plant motion and a decreasing coil store. A finite reciprocal actuator adds its own magnetic endpoints and copper loss. The article derives voltage, force, slew and uncertainty requirements and a conditional efficiency threshold for separate actuator, bias and DC-link measurements. Wider bias-dependent thermal and subledger accuracy questions remain explicit.

- **Zero reference-output current can accompany growing receiver energy.** An accelerating-reference circuit adds $1/5\,\mathrm{J}$ to its receiver while drawing zero net current from the reference-driver output. Separate compensation and driver work determine the supply costs. A causal compound driver and an exact reversing receiver retain all their states. The receiver has zero net work while its finite driver supplies $3/200000\,\mathrm{J}$. A dissipative extension has a complete exact event certificate and separately supplied winding and driver losses. A winding preparation can retain finite energy while its common current tends to zero. Reference-change work grows inversely with duration at fixed positive driver resistance and capacitance.

- **Matching terminal behavior can conceal different stores and stresses.** The article carries damped mechanical/electrical correspondences through preparation, relaxation and reset, then gives explicit controls for hidden states. Two tuned absorbers can both produce zero terminal reaction while their coupling stresses and stored energies differ. Measuring the internal motion and strain reveals what the terminal trace leaves undetermined.

Exact separation budgets and component-rating bounds distinguish finite physical comparisons from constitutive acquisition and accounting controls across the twelve principal questions and their supporting cases. Independently measured work and endpoint stores decide which transfer path the apparatus follows. A signed residual outside calibrated uncertainty remains an explicit unresolved gain or deficit.

All worked values follow from exact declared models. The article reports no hardware acquisition or numerical simulations. Identical terminal predictions can establish an identification limit; internal observations supply the discrimination. The bounded absorber result remains resolved, with its wider physical questions kept distinct.

The main text carries the slow torsional comparison from calibration to independently changed contact/joint settings and release. The appendices develop terminal identification, physical correspondence and connection paths, transformer attachments, controlled transducers and supplied references, finite implementations and events, and calibrated measurement bounds. Finite bank reconnection, loaded four-terminal correspondence and the shared-core circuit retain their complete treatments. Their conclusions remain separate: finite receiver service, no full-state cycle in an insulated timing-drive model, and an exact limit on finite-error energy identification. None supplies hardware validation.

## Article and build

[Read the article (PDF)](hidden-states-and-unassigned-work.pdf) · [Manuscript source](hidden-states-and-unassigned-work.md)

Install GNU Make, Pandoc, XeLaTeX and the TeX Gyre fonts, including the LaTeX
packages used by `preamble.tex` and the standalone TikZ/PGFPlots figures. Run `make pdf`
from this repository. The build uses only files in this checkout; no sibling
repository or private working files are needed.

The first page gives the PDF creation time in UTC, followed by this repository's
GitHub link. An up-to-date PDF keeps its timestamp; `make -B pdf` forces a rebuild.
Intermediates go to ignored `build/` by default; `BUILD_DIR=/absolute/path`
selects another location. `make clean` removes that build directory and keeps
the published PDF and figure assets.

The title date records the first version. Keep `ARTICLE_DATE` in the Makefile
and the manuscript's `date` fixed across revisions. The separate `PDF created`
timestamp continues to record each PDF rebuild in UTC.
