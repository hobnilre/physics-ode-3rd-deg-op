# Hidden States and Unassigned Work

Exact models and decisive measurements for higher-order ODEs

This companion develops eighteen questions about physical realization, preparation, identification, collision release, switching, and signed work. It distinguishes exact model results from the physical transfers and measurement questions that remain open. All worked values follow from closed forms; the project contains no numerical simulations or measured data.

The related article is [*Third- and Higher-Order ODEs*](https://github.com/hobnilre/physics-ode-3rd-deg/blob/main/third-and-higher-order-odes.pdf).

## What this article adds, and why it matters

Stored energy is not always constant: contact release can remove a positive store, a bias coil can gain energy with the plant drives off, and switching can redirect the transferred work. The article develops exact constructions that expose these changes and identifies measurements that distinguish their physical destinations.

- **Energy remains when contact force reaches zero.** In one exact collision, force-zero detachment leaves a positive spring store of $e^{-\pi}\,\mathrm{J}$. A retained material-state model predicts delayed relaxation and $e^{-\pi}/4\,\mathrm{J}$ remaining after $\log2\,\mathrm{s}$. Repeated impacts must carry residual strain and heat or include a measured reset. Different separation laws change both restitution and the energy left at release; fracture, acoustic, thermal and fixture measurements distinguish the possible destinations.

- **A vanishing state can carry finite energy.** A prepared capacitor family retains finite initial energy while capacitance and charge tend to zero. The work released depends on the ratio of switching duration to discharge time. A finite example drops from $2$ to $1/2\,\mathrm{mJ}$, exposing the transfer that a reduced model can discard along with its initial state.

- **Equal final voltages leave individual switch work undetermined.** Reversing two connection channels exchanges their signed works, $-3/4$ and $-3/16\,\mathrm{mJ}$, while both capacitor endpoints stay the same. Simultaneous connection gives a third partition. Complete finite transformer return paths retain both winding currents, the output capacitor, clamp, two return channels and eight separate work integrals. Equal source durations still give a strictly nonzero difference in old-return work.

- **Bias-coil energy can increase with the plant drives and external charger off.** An exact controlled transducer transfers actuator reaction work into its controller while the bias coil gains stored energy. A different receiving path gives identical plant motion and a decreasing coil store. A finite reciprocal actuator adds its own magnetic endpoints and copper loss. The article derives voltage, force, slew and uncertainty requirements and a conditional efficiency threshold for separate actuator, bias and DC-link measurements. Wider bias-dependent thermal and subledger accuracy questions remain explicit.

- **Zero reference-output current can accompany growing receiver energy.** An accelerating-reference circuit adds $1/5\,\mathrm{J}$ to its receiver while drawing zero net current from the reference-driver output. Separate compensation and driver work determine the supply costs. A causal compound driver and an exact reversing receiver retain all their states. The receiver has zero net work while its finite driver supplies $3/200000\,\mathrm{J}$. A dissipative extension has a complete exact event certificate and separately supplied winding and driver losses. A winding preparation can retain finite energy while its common current tends to zero. Reference-change work grows inversely with duration at fixed positive driver resistance and capacitance.

- **Matching terminal behavior can conceal different stores and stresses.** The article carries damped mechanical/electrical correspondences through preparation, relaxation and reset, then gives explicit controls for hidden states. Two tuned absorbers can both produce zero terminal reaction while their coupling stresses and stored energies differ. Measuring the internal motion and strain reveals what the terminal trace leaves undetermined.

Exact separation budgets and component-rating bounds distinguish finite physical comparisons from constitutive acquisition and accounting controls across the eighteen questions. Independently measured work and endpoint stores decide which transfer path the apparatus follows. A signed residual outside calibrated uncertainty remains an explicit unresolved gain or deficit.

## Article

[Read the article (PDF)](hidden-states-and-unassigned-work.pdf) · [Manuscript source](hidden-states-and-unassigned-work.md)
