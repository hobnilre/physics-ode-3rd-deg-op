---
title: "Hidden States and Unassigned Work"
subtitle: "Exact models and decisive measurements for higher-order ODEs"
author: "Hob Nilre & Bo C. Herlin"
date: "2026-09-26"
abstract: |
  Eliminating physical states can raise the differential order of an observation while concealing preparation, internal stress and transfers at a change of connection. We develop eighteen questions associated with higher-order ODEs, retaining the distinction between unresolved measurements and results already settled within bounded models. Exact damped analogies, hidden-state controls and finite switching paths provide discriminating observables. A compliant contact can release a positive spring store at zero force; equal capacitor endpoints can accompany unequal switch work; a controlled source-off transducer can transfer energy into its bias coil; and an accelerating-reference correspondence requires a separately powered compensation port. Each construction specifies its boundary, states, signed port integrals and endpoint stores. Finite laboratory realizations and alternative predictions delimit what would close the remaining physical questions. All calculations use closed forms; the article reports no measured data.
keywords:
  - higher-order ordinary differential equations
  - hidden states
  - physical preparation
  - signed work
  - contact release
  - switching
  - identifiability
documentclass: article
classoption:
  - 11pt
geometry:
  - margin=1.1in
mainfont: "TeX Gyre Termes"
sansfont: "TeX Gyre Heros"
monofont: "TeX Gyre Cursor"
mathfont: "TeX Gyre Termes Math"
numbersections: true
secnumdepth: 3
indent: true
linestretch: 1.05
colorlinks: true
linkcolor: MidnightBlue
urlcolor: MidnightBlue
citecolor: MidnightBlue
---

Latest PDF on GitHub:

<https://github.com/hobnilre/physics-ode-3rd-deg-op/blob/main/hidden-states-and-unassigned-work.pdf>

# Questions left by state elimination
\label{sec:introduction}

A third- or fourth-order equation can correctly describe one measured coordinate while leaving the physical meaning of its initial derivatives, other ports and connection changes undetermined. The distinction between differential order, observable order and physical storage developed in [*Third- and Higher-Order ODEs*][main] leads to two connected tasks: identify the states that a terminal trace conceals, and identify the transfers that a reduced model removes. This companion develops those tasks through explicit finite models and measurements.

The damped correspondence question is whether a collision or oscillator and an electrical circuit with positive damping can transport preparation, relaxation and reset ports as well as their homogeneous equations [OP-LR50-01]. Contact identification asks whether hammer measurements, supplemented by anvil measurements, can separate contact coefficients from a frequency-dependent support; an additional support state can remain inaccessible [OP-LR08-01]. Coefficient identification asks whether independently varied physical coordinates and correlated or temporally colored uncertainty permit recovery of weak contributions that are indistinguishable on a restricted path [OP-LR31-01]. None of these questions requires a measured energy discrepancy.

The resonator question requires calibrated impedance measurements across devices and fixtures, including the shunt state that changes the rational port law [OP-LR12-01]. The polarization question concerns order recovery with arbitrary branch preparations and noisy data: equal-time-constant branches can contain an independently decaying difference state absent from the terminal current [OP-LR01-04]. For a tuned absorber, the bounded conclusion that terminal reaction alone does not identify internal coupling stress is resolved; the remaining practical question is which calibrated internal observations identify that stress in physical devices and wider models [OP-LR58-01]. A zero reaction with finite coupling strain is a direct control for that distinction.

The energy questions arise at more specific boundaries. A linear contact released when force first reaches zero retains $U_c=d^2v_-^2/(2k)>0$ if its separation speed $v_-$ is nonzero. Removing the contact state assigns a negative event work to the retained system but leaves the fracture, acoustic, thermal or fixture destination unidentified [OP-LR03-01]. Choosing force-zero, deformation-zero or a law with damping only in compression gives different restitution and release stores; the constitutive choice is unresolved [OP-LR03-02]. Across repeated impacts, both the destination and the restitution law need identification for each engagement [OP-LR04-01]. Friction, plasticity, adhesion, motor ripple, additional engagements and changing gaps, contact geometry or damping can alter the accumulated transfer, beyond a fixed two-impact model [OP-LR04-02]. Section \ref{sec:contact} gives positive removed work $e^{-\pi}\ \mathrm J$ in one exact force-zero example, and zero removed spring store for two distinct alternative laws.

Singular passive-network reductions can discard a prepared reactive state with finite energy even when its terminal charge or linkage vanishes. Which component coscalings, endpoint stores and impulse works describe the physical approach is unresolved [OP-LR21-01]. A zero-state smooth response does not determine the signed switching work of that prepared system [OP-LR21-02]. For two connected capacitors the total difference-store decrease can be fixed while the individual channel works differ: in Section \ref{sec:connection}, the same endpoints accompany $(-3/4,-3/16)\ \mathrm{mJ}$ or the reversed pair [OP-LR48-02]. Actual switch and gap laws, arc ignition and restrike, winding capacitance and clamp release must determine where the transfer goes [OP-LR48-03]. The joint approaches to zero parasitic capacitance and zero duration, other coupling orientations and continuous or wider limiting ratios remain separate questions [OP-LR48-05]. Exact zero duration and zero capacitance are mathematical boundaries, not apparatus settings.

In a loaded transformer, switching a source voltage to zero retains a conductor path. Actual winding opening, energized tap or return commutation and capacitor charge sharing require individual winding, clamp, return and control-supply work that this operation does not specify [OP-TRF-02]. The controlled third-order transducer raises a different question: during source-off operation a positive bias-coil energy change can accompany actuator reaction work into its controller, while the finite supply realization and its complete physical ledger remain unresolved [OP-LR59-02]. Section \ref{sec:transducer} derives an instrumentable conditional example with bias-store change $(3\log 2/10000-3/800000)\ \mathrm J>0$.

Finally, an accelerating mechanical reference changes relative kinetic storage. Its electrical counterpart needs an actual compensation source, with work of either sign. The prescribed-reference capacitor cell is settled within its model; a state-dependent compound driver, energized constraints, complete event coverage and hardware supply costs remain unresolved [OP-TRF-12]. Section \ref{sec:reference} distinguishes a capacitor receiving $1/5\ \mathrm J$ from an uncompensated capacitor receiving zero under the same prescribed reference motion. The closing measurements compare these physical alternatives, retaining the settled local results.

# Boundaries, ports and exact work
\label{sec:ledger}

For each system let $x$ contain its independent physical states. Its constitutive store $E(x)$ is evaluated at both ends of the declared interval. A port has effort $e_\ell$ and conjugate flow $f_\ell$, with positive product into that boundary. The definitions are
\begin{equation}
 W_\ell(t_0,t_1)=\int_{t_0}^{t_1}e_\ell(t)f_\ell(t)\,\dd t,
 \qquad r_E=E(x(t_1))-E(x(t_0))-\sum_\ell W_\ell.
 \label{eq:ledger}
\end{equation}
Electrical ports use $vi$, mechanical ports use $Fv$ or $\tau\omega$. A thermal export uses $-T\dot S_{\rm out}$; acoustic transfer uses the integral of pressure times outward normal volume flow over its boundary. A resistor outside the stored subsystem contributes $-v(v/R)$, and a damper contributes $-(dv)v$. These are separate integrals, even when their sum has a simpler expression.

At a connection event, $x(t_e^-)$ and $x(t_e^+)$ belong to different vector fields or constraints. A finite interval resolving the event determines each work. A singular work is the limit of those integrals if it exists. Deleting a constitutive store and writing an event term equal to its negative closes a mathematical ledger, but supplies no effort, flow or physical recipient. That term must remain distinguished from a measured transfer.

For a finite mass, $m\dot v=F$ gives $\int Fv\,\dd t=m[(v^+)^2-(v^-)^2]/2$ by integrating the product. This equals $J(v^-+v^+)/2$ when $J=m(v^+-v^-)$; it does not define a product of an unspecified delta force with a discontinuous velocity. A fixed support can exchange momentum while its work is zero. A moving support needs its own force--velocity integral.

All integrations below are exact, so the numerical integration residual is exactly zero. A closed ideal ledger has $r_E=0$ by direct substitution after the separate integrals. The physical model residual $r_{\rm model}$ includes omitted material memory, switch-control supply, heat storage, exterior fields or release destinations, as named for each construction. Its sign and magnitude remain unevaluated unless a declared additional law determines them. Existing unresolved finite-precision integration and endpoint uncertainties are not converted into physical transfers by these exact examples.

Figure \ref{fig:boundaries} separates the observed port from hidden states and event transfers.

![Schematic of an observed physical system. The terminal trace constrains a projection of the state. Separate preparation, release and internal-observation paths remain necessary.](figures/boundaries.pdf){#fig:boundaries width=100%}

\FloatBarrier

# Damping, preparation and what a terminal identifies
\label{sec:identification}

## A damped correspondence with a complete finite path

Let $x$ be the relative compression of two free masses during a linear contact, with reduced mass $m=m_1m_2/(m_1+m_2)$, or the displacement of a mass against a fixed spring and damper. Relative force balance is $m\ddot x+d\dot x+kx=f$. In the free-pair interpretation the center-of-mass mode is separately retained and the relative applied effort $f$ is the one conjugate to $\dot x$; it equals $m(F_1/m_1-F_2/m_2)$. The fixed-support interpretation has zero support velocity. A series electrical circuit has charge $q$, current $i=\dot q$ and applied voltage $V$.

\begin{theorem}
For positive constants $\alpha,\beta$, the map
\begin{equation}
 q=\alpha x,\quad i=\alpha\dot x,\quad V=\beta f,
 \quad L=\frac{\beta m}{\alpha},\quad
 R=\frac{\beta d}{\alpha},\quad C=\frac{\alpha}{\beta k}
 \label{eq:analogy}
\end{equation}
maps force balance to Kirchhoff's voltage law, including prescribed preparation and reset efforts. Each electrical source, loss and spring/inertial transfer work equals $\alpha\beta$ times its corresponding mechanical work on every smooth interval. Compatible finite event paths have the same property.
\end{theorem}

Substitution gives $L\dot i+Ri+q/C=\beta(m\ddot x+d\dot x+kx)=V$. Independently, $Vi=\alpha\beta f\dot x$, $-Ri^2=-\alpha\beta d\dot x^2$, $Li\dot i=\alpha\beta m\dot x\ddot x$, and $(q/C)\dot q=\alpha\beta kx\dot x$. Integrating each equality proves the assertion, and direct state evaluation gives $E_e=\alpha\beta E_m$. A finite event equality passes to a limit only if its individual integrals converge. $\square$

Configuration I uses $m=1\ \mathrm{kg}$, $d=2\ \mathrm{N\,s/m}$, $k=2\ \mathrm{N/m}$, $\alpha=1\ \mathrm{C/m}$ and $\beta=1\ \mathrm{V/N}$. Thus $L=1\ \mathrm H$, $R=2\ \Omega$, $C=1/2\ \mathrm F$, the work scale is one, and $\rho=d^2/(mk)=2>0$. In the following formulas time is expressed in seconds and displacement in metres. Starting at rest, prescribe $x=t(t+1)^2$ on $[-1,0]$. The required force, derived from the equation of motion, is $f=2t^3+10t^2+16t+6$. The source and damper integrals give $23/30\ \mathrm J$ and $-4/15\ \mathrm J$; the final independently evaluated kinetic store is $1/2\ \mathrm J$ and the spring store is zero.

With the source off, the exact response is
\begin{equation}
 x=e^{-t}\sin t,\quad \dot x=e^{-t}(\cos t-\sin t),\quad
 E_m=\tfrac12e^{-2t}(\cos t-\sin t)^2+e^{-2t}\sin^2t.
 \label{eq:oscillator}
\end{equation}
Keep this bilateral oscillator connected until $T=\pi/2$. Then $X=x(T)=e^{-\pi/2}$, $V_T=\dot x(T)=-X$, and $E_T=3e^{-\pi}/2\ \mathrm J$. On a further one-second interval put $s=t-T$ and prescribe the finite reset
\begin{equation}
 x=X(1-3s^2+2s^3)+V_T(s-2s^2+s^3),\qquad 0\leq s\leq1.
 \label{eq:reset-polynomial}
\end{equation}
The reset force again follows from $f=\ddot x+2\dot x+2x$. Direct integration uses
$\int_0^1\dot x^2\dd s=6X^2/5+XV_T/5+2V_T^2/15$ and yields the ledger below. No impulsive reset is imposed.

| Interval | Source work, J | Damper work, J | Stores before and after, J |
|:------------------|:-------------------------|:---------------------------|:------------------------------|
| Preparation | $23/30$ | $-4/15$ | $0\ \to\ 1/2$ |
| Source off | $0$ | $-1/2+3e^{-\pi}/2$ | $1/2\ \to\ 3e^{-\pi}/2$ |
| Finite reset | $23e^{-\pi}/30$ | $-34e^{-\pi}/15$ | $3e^{-\pi}/2\ \to\ 0$ |

: Independently integrated works in configuration I. The electrical counterpart has the same entries. Each interval has zero residual.

A homogeneous trajectory comparison alone predicts none of the preparation or reset source readings. A complete correspondence predicts all three source works in the table. Transporting a unilateral release additionally requires the same constitutive gate and a mapped destination port; Section \ref{sec:contact} supplies the missing distinction. Lossless coordinates with $d=0$ cannot certify a construction expressed through $m/d$ or $d^2/(mk)$ away from that boundary.

The center-of-mass state can also be retained in an explicit collision circuit. Choose a voltage/velocity scale $\alpha_v>0$ and let $V_j=\alpha_v v_j$, $I_j=F_j/\alpha_v$, $C_j=m_j/\alpha_v^2$, $L_c=\alpha_v^2/k$ and $G_c=d/\alpha_v^2$. Connect the two grounded capacitors by an inductor and conductance in parallel, with $i_c=k\delta/\alpha_v$ flowing from node 1 to node 2. Kirchhoff's laws are
\begin{equation}
 C_1\dot V_1=I_1-i_c-G_c(V_1-V_2),\quad
 C_2\dot V_2=I_2+i_c+G_c(V_1-V_2),\quad
 L_c\dot i_c=V_1-V_2.
 \label{eq:full-collision-map}
\end{equation}
They map both body force balances and $\dot\delta=v_1-v_2$ exactly. Each body input satisfies $V_jI_j=F_jv_j$, the resistor exports $G_c(V_1-V_2)^2=d(v_1-v_2)^2$, and the three component stores map individually. Taking $m_1=m_2=2\ \mathrm{kg}$ and $\alpha_v=1\ \mathrm{V/(m/s)}$ gives $C_1=C_2=2\ \mathrm F$, $L_c=1/2\ \mathrm H$ and $G_c=2\ \mathrm S$. Initial velocities $(1/2,-1/2)\ \mathrm{m/s}$ give configuration I's relative state and zero center-of-mass velocity. Opposite finite drives $(f,-f)$ transport its preparation and reset table without dropping either body port. This three-state collision circuit therefore extends the damped correspondence beyond the relative coordinate alone.

## Contact versus a compliant support

For hammer and anvil angles $\theta_h,\theta_a$, positive inertias $J_h,J_a$, contact torque $\tau_c=k_c(\theta_h-\theta_a)+d_c(\dot\theta_h-\dot\theta_a)$ and support torque $\tau_j=k_j\theta_a+d_j\dot\theta_a$, the equations are
\begin{equation}
 J_h\ddot\theta_h=u-\tau_c,\qquad
 J_a\ddot\theta_a=\tau_c-\tau_j.
 \label{eq:two-inertia}
\end{equation}
They give a generic fourth-order hammer equation. With $Z_c=k_c+d_cs$ and $Z_a=J_as^2+k_j+d_js$, elimination gives
\begin{equation}
 \frac{U}{\Theta_h}=J_hs^2+\frac{Z_cZ_a}{Z_c+Z_a},\qquad
 \frac{\Theta_a}{\Theta_h}=\frac{Z_c}{Z_c+Z_a}.
 \label{eq:contact-inference}
\end{equation}
The terminal observes a composite dynamic stiffness. If a broader rational support is allowed, different admissible decompositions of that composite must be distinguished before assigning internal coefficients. Positivity, a known inertial model and a sufficiently rich frequency domain can impose additional constraints; static ambiguity alone is not a theorem of ambiguity on every frequency domain.

The local ambiguity at one complex frequency is also explicit. Writing $Z_e=Z_cZ_a/(Z_c+Z_a)$ and $H_a=\Theta_a/\Theta_h$, differentiation gives
\begin{equation}
 \delta Z_e=\frac{Z_a^2\delta Z_c+Z_c^2\delta Z_a}{(Z_c+Z_a)^2}.
 \label{eq:contact-null}
\end{equation}
For nonzero $Z_c,Z_a,Z_c+Z_a$, the perturbation $\delta Z_a=-(Z_a/Z_c)^2\delta Z_c$ leaves that terminal observable unchanged to first order, while $\delta H_a=Z_a\delta Z_c/[Z_c(Z_c+Z_a)]$ is generally nonzero. A parameterized passive model constrains which such perturbations extend over the full frequency interval. Consequently the combined observation Jacobian, its covariance-weighted sensitivity and independent-frequency prediction must be checked for the declared family, rather than inferred from this local null alone.

Configuration II makes the simplest ambiguity exact. At static torque $u=1\ \mathrm{N\,m}$, both $(k_c,k_j)=(2,2)$ and $(3,3/2)\ \mathrm{N\,m/rad}$ give $\theta_h=1\ \mathrm{rad}$. The corresponding $\theta_a$ values are $1/2$ and $2/3\ \mathrm{rad}$, and contact deformations are $1/2$ and $1/3\ \mathrm{rad}$. Contact and support stores are respectively $(1/4,1/4)$ and $(1/6,1/3)\ \mathrm J$. Static power is zero; these endpoint stores do not assign the earlier preparation work.

The physical two-body boundary contains both kinetic stores and both springs. Its independently signed external powers are $u\dot\theta_h$, $-d_c(\dot\theta_h-\dot\theta_a)^2$ and $-d_j\dot\theta_a^2$. A movable support at angle $z$ replaces the second deformation by $\theta_a-z$ and adds inward support power $-\tau_j\dot z$. A support inertia and another spring give their own second-order state equation and can raise the full order to six. Measuring the anvil alone then does not guarantee identification of $z$ or of an arbitrary rational support.

The finite closure question is a rank and uncertainty statement for specified contact and support families, followed by prediction under independently changed support and contact conditions. The bounded normalized-map results do not imply universal raw-unit identifiability. Calibrated contact torque, anvil motion and, where required, support motion distinguish the alternatives in \eqref{eq:contact-inference}. The mechanism-level need to represent changing contacts is consistent with [Wettstein, Grauberger and Matthiesen (2021)][wettstein]; that study supplies neither a universal release law nor the destination considered here.

## Independent coordinates and correlated uncertainty

Let $a,b,c>0$ be inertial, damping and stiffness references. The dimensionally admissible coefficients
\begin{equation}
 A_{r,k}=a^{k-1+r}b^{2-k-2r}c^r
 =S\tau^k\rho^{-r},\quad S=b^2/a,\quad\tau=a/b,\quad\rho=b^2/(ac)
 \label{eq:coefficients}
\end{equation}
have the dimensions required to multiply the $k$th derivative. At fixed $\rho$, changing $r$ only rescales a column in coefficient identification. In a two-coordinate contact model a normalized coefficient can take the form
\begin{equation}
 B(\rho,\eta)=w_0+w_1\eta+w_2\eta^2/\rho.
 \label{eq:weak-coefficient}
\end{equation}
Here $B$ is the coefficient divided by its dimensional reference; $\eta>0$ is an independently varied damping ratio. Configuration III has $w=(1,1/100,1/2)$. The alternative $\widetilde w=(101/100,0,1/2)$ agrees at every point with $\eta=1$. At $(\rho,\eta)=(1,1),(4,1),(1,2)$, the design determinant is $3/4$ and the first model predicts $151/100,227/200,151/50$. The alternative predicts $301/100$ at the last point. Independent variation therefore creates an exact separation of $1/100$ there.

For two observations with variance $\sigma^2$ and correlation $\gamma$, the uncertainty variance of their difference is exactly $2\sigma^2(1-\gamma)$. More generally, a linear contrast $c^Ty$ has variance $c^T\Sigma c$, with the full spatial and temporal covariance $\Sigma$. These expressions follow by expanding the covariance of the sum; positive-definiteness requires $|\gamma|<1$ in the nonsingular two-channel case. With bounded contrast error $\epsilon$, predictions separated by $1/100$ have disjoint error intervals when $2\epsilon<1/100$. A covariance alone does not supply a deterministic bound without a distributional assumption.

This is a finite discrimination result for a declared support. A device may require another support or another observation operator. Calibration, coefficient estimation, model choice and the final independent condition must use separate information. The remaining question concerns realistic covariance and weak contributions on independently varied physical coordinates, not a change in energy when a coefficient becomes difficult to estimate.

## A shunt state and a transferable resonator law

A motional series branch $(R_m,L_m,C_m)$ in parallel with $C_0$ obeys, at complex frequency $s$,
\begin{equation}
 Y(s)=sC_0+\frac{sC_m}{L_mC_ms^2+R_mC_ms+1}.
 \label{eq:resonator}
\end{equation}
This follows from Kirchhoff's current law with common voltage $v$, motional current $i_m$, charge $q_m$, and state laws $\dot q_m=i_m$, $L_m\dot i_m=v-R_mi_m-q_m/C_m$, $i=C_0\dot v+i_m$. It is the conventional motional-plus-shunt description discussed by [Bible (2002)][bible]. A voltage-driven experiment prescribes the shunt voltage; a finite source impedance restores that capacitor as an independent state of the connected system.

At $\omega_s=1/\sqrt{L_mC_m}$ the motional admittance is $1/R_m$, hence a changed shunt capacitance predicts $\Delta\operatorname{Im}Y=\omega_s\Delta C_0$. Configuration IV uses illustrative low-frequency values $R_m=1\ \Omega$, $L_m=1\ \mathrm H$, $C_m=1\ \mathrm F$, with $C_0=1$ or $2\ \mathrm F$. At $\omega_s=1\ \mathrm{rad/s}$, the two impedances are $(1-\ii)/2$ and $(1-2\ii)/5\ \Omega$. A series-only reading gives $1\ \Omega$ in both cases. These are exact component controls, not quartz parameter values.

For peak voltage $V$ at resonance over one period $T=2\pi/\omega_s$, separately integrating $vi$, $-R_mi_m^2$ and the shunt product $vC_0\dot v$ gives
\begin{equation}
 W_{\rm source}=\frac{TV^2}{2R_m},\qquad
 W_{R_m}=-\frac{TV^2}{2R_m},\qquad
 \int_0^T vC_0\dot v\,\dd t=0.
 \label{eq:rf-work}
\end{equation}
Each component returns to its initial periodic state, but its instantaneous store varies. At $V=1\ \mathrm V$ in configuration IV the source and loss works are $\pi$ and $-\pi\ \mathrm J$. The imaginary admittance, rather than the equal period work, distinguishes the shunts.

The open acquisition requires calibrated multi-device complex impedance and independent shunt variation, with synchronized internal/terminal traces where an internal claim is made. A bounded comparison can retain twelve resonators and three fixture/component variants, with calibration and final conditions separated. Fixture compensation and RF current/voltage definitions follow the measurement distinctions in [Keysight Technologies (2026)][keysight]. Neither a one-device coefficient law nor the exact low-frequency control establishes temperature, aging or nonlinear transferability.

## Polarization preparations invisible at the terminal

A coil feeding a polarization emulator has states $i,v_1,\ldots,v_N$ and equations
\begin{equation}
 L\dot i+R_\Sigma i+V_{\rm oc}+\sum_jv_j=0,
 \qquad C_j\dot v_j=i-v_j/R_j.
 \label{eq:polarization}
\end{equation}
Positive $i$ enters the emulator. With a diode this law ends at the first downward current zero; each polarization branch then relaxes with $i=0$. For distinct active time constants $\tau_j=R_jC_j$, eliminating the branches gives generic order $N+1$ for $i$, while equal time constants combine at that observation. The storage boundary includes the coil and branch capacitors. Its external powers are $-V_{\rm oc}i$, $-R_\Sigma i^2$ and the separately retained $-v_j^2/R_j$; the DC source and all heat reservoirs are outside.

For two equal branches define $z_+=(v_1+v_2)/2$ and $z_-=(v_1-v_2)/2$. Direct addition and subtraction give
\begin{equation}
 C\dot z_+=i-z_+/R,\qquad C\dot z_-=-z_-/R,
 \qquad E_C=Cz_+^2+Cz_-^2.
 \label{eq:hidden-battery}
\end{equation}
The terminal loop sees $2z_+$ and is independent of $z_-$. Two states with identical $i,z_+$ and arbitrary different $z_-$ therefore have identical terminal current for as long as the same graph applies. This is an exact unobservable direction, rather than a small nonzero sensitivity.

Configuration V has $C=1\ \mathrm{mF}$, $R=1\ \mathrm{k}\Omega$, $v_1(0)=1\ \mathrm V$, $v_2(0)=-1\ \mathrm V$ and terminal current zero. It can be isolated during observation, or compared with another preparation on the same driven terminal trajectory using superposition. On $[0,\log2]\ \mathrm s$, its hidden store falls from $1$ to $1/4\ \mathrm{mJ}$. The two independently integrated resistor works are each
\begin{equation}
 -\int_0^{\log2}\frac{e^{-2t}}{1000}\,\dd t
 =-\frac38\ \mathrm{mJ}.
 \label{eq:battery-loss}
\end{equation}
An unprepared pair gives zero branch voltages and zero hidden heat under the same zero terminal current.

These states have a finite preparation. With accessible branch current sources, prescribe $v_j=\pm(t+1)\ \mathrm V$ on $[-1,0]\ \mathrm s$ while the terminal connection is open. The required source current is $i_{pj}=C\dot v_j+v_j/R$. Its work $\int v_ji_{pj}\dd t=5/6\ \mathrm{mJ}$ per branch and the resistor work $-1/3\ \mathrm{mJ}$ leave $1/2\ \mathrm{mJ}$ in each capacitor. The source efforts and flows, including the negative-voltage branch, have their specified signs.

After a deliberate split into time constants $\tau_1\ne\tau_2$, the same isolated opposite preparation yields terminal voltage $a(e^{-t/\tau_1}-e^{-t/\tau_2})$. At $a=1\ \mathrm V$, $\tau_1=1\ \mathrm s$, $\tau_2=2\ \mathrm s$ and $t=\log2\ \mathrm s$, this is $1/2-1/\sqrt2\ \mathrm V$, versus zero for equal constants. Branch probes distinguish exact hidden freedom from a transient lying below terminal resolution. No finite noise bound can certify arbitrary order when time constants and amplitudes can approach coincident or vanishing values without a separation restriction.

## Terminal reaction and internal absorber stress

Take primary mass $M$, absorber mass $m$, fixed-base spring/damper $k_0,c_0$ and coupling $k_2,c_2$. With fixed base and primary force $F(t)$,
\begin{align}
 M\ddot x_1+c_0\dot x_1+k_0x_1+c_2(\dot x_1-\dot x_2)+k_2(x_1-x_2)&=F,\nonumber\\
 m\ddot x_2+c_2(\dot x_2-\dot x_1)+k_2(x_2-x_1)&=0.
 \label{eq:absorber}
\end{align}
The terminal reaction is $R_b=k_0x_1+c_0\dot x_1$ and the coupling force is $F_2=k_2(x_1-x_2)+c_2(\dot x_1-\dot x_2)$. At $c_2=0$ and $\omega^2=k_2/m$, a prepared exact periodic solution is
\begin{equation}
 F=F_0\cos\omega t,\qquad x_1=0,
 \qquad x_2=-\frac{F_0}{k_2}\cos\omega t,
 \qquad R_b=0,\quad F_2=F_0\cos\omega t.
 \label{eq:antiresonance}
\end{equation}
Substitution proves the result without inferring force from the zero reaction. In a calibrated known model with known drive, the force can of course be inferred from that additional information; the unresolved inference is from the reaction alone and uncertain internal realization.

Configuration VI compares $(m,k_2)=(1/10\ \mathrm{kg},100\ \mathrm{N/m})$ and $(1/5\ \mathrm{kg},200\ \mathrm{N/m})$, with the same $\omega=10\sqrt{10}\ \mathrm{rad/s}$, $F_0=1\ \mathrm N$, $M=1\ \mathrm{kg}$, $k_0=100\ \mathrm{N/m}$ and $c_0=1\ \mathrm{N\,s/m}$. Coupling cross sections of $1$ and $2\ \mathrm{mm^2}$ with the same modulus and length give these stiffness ratios. The two zero terminal reactions coexist with extension amplitudes $1/100$ and $1/200\ \mathrm m$, and stress amplitudes $1$ and $1/2\ \mathrm{MPa}$.

The boundary contains both masses and both springs. Its source power $F\dot x_1$ and support-damper power $-c_0\dot x_1^2$ vanish separately on this solution; $c_2=0$. Nevertheless its independently evaluated coupling-plus-absorber store is $F_0^2/(2k_2)$, respectively $1/200$ and $1/400\ \mathrm J$, at both ends of every period. The initial state is prepared, not assumed to arise from rest with these zero works. Internal strain and motion separate the configurations; a bounded structural-negative result needs no reopening. Practical stress conversion, material calibration, additional modes and loading remain physical questions.

# Contact release and repeated engagement
\label{sec:contact}

## Three constitutive laws with different endpoint predictions

For a free normal collision the center-of-mass motion separates from relative compression $\delta\geq0$. The relative boundary contains $K=m\dot\delta^2/2$ and $U=k\delta^2/2$. On active contact its law is $m\ddot\delta=-F_c$, initially $\delta=0$, $\dot\delta=v_0>0$. Contact damping exports power $-(d\dot\delta)\dot\delta$; external relative drive and fixture powers, when present, are separately $f_d\dot\delta$ and $f_b\dot\delta$. They vanish during the free contact considered here. The two-body center-of-mass kinetic energy is evaluated separately and remains unchanged because the external force sum is zero.

For $F_c=k\delta+d\dot\delta$ with $a=d/(2m)$, $\omega_0=\sqrt{k/m}$ and $\omega_d=\sqrt{\omega_0^2-a^2}>0$, force balance gives
\begin{equation}
 \delta(t)=\frac{v_0}{\omega_d}e^{-at}\sin\omega_dt,
 \qquad \dot\delta(t)=v_0e^{-at}
 \left(\cos\omega_dt-\frac a{\omega_d}\sin\omega_dt\right).
 \label{eq:contact-solution}
\end{equation}
Let $\zeta=a/\omega_0\in(0,1)$. The first force zero occurs at
$t_F=2\arccos\zeta/\omega_d$, with restitution $e_F=e^{-at_F}$, velocity $-e_Fv_0$ and deformation $d e_Fv_0/k$. The first deformation zero is $t_D=\pi/\omega_d$ and gives $e_D=e^{-at_D}$. Between $t_F$ and $t_D$ the linear force is tensile. A unilateral law must therefore specify which event ends the model.

A third law acts with damping only in compression:
$F_c=k\delta+d\max(\dot\delta,0)$ for $\delta>0$, followed by separation at $\delta=0$. It follows \eqref{eq:contact-solution} until maximum compression $t_P=\arccos\zeta/\omega_d$, then an undamped spring rebound for $\pi/(2\omega_0)$. Its restitution is $e_C=e^{-at_P}$. This is a different constitutive law, not an instruction to clip a tensile force while retaining an unchanged store balance.

Configuration I, now interpreted as contact, has $m=1$, $d=2$, $k=2$ in the SI units already specified and $v_0=1\ \mathrm{m/s}$. Thus $a=\omega_d=1\ \mathrm{s^{-1}}$, $\omega_0=\sqrt2\ \mathrm{s^{-1}}$, and $F_c=2e^{-t}\cos t\ \mathrm N$ before any change of law.

| Constitutive release | Release time, s | Restitution | Pre-release $U$, J | Damper work, J |
|:-------------------------------|:--------------------------|:-----------------|:--------------------|:---------------------------|
| Linear, force zero | $\pi/2$ | $e^{-\pi/2}$ | $e^{-\pi}$ | $-1/2+3e^{-\pi}/2$ |
| Linear, deformation zero | $\pi$ | $e^{-\pi}$ | $0$ | $-1/2+e^{-2\pi}/2$ |
| Compression damping only | $\pi/4+\pi/(2\sqrt2)$ | $e^{-\pi/4}$ | $0$ | $-1/2+e^{-\pi/2}/2$ |

: Exact mutually distinct release predictions. The second law includes a tensile interval; the third changes the damping effort at maximum compression.

To check the first two loss entries independently, integrate $-2e^{-2t}(\cos t-\sin t)^2$ to the listed time. For the third, integrate that product only to $\pi/4$; the subsequent damping power is zero. The outgoing kinetic energies are $e^{-\pi}/2$, $e^{-2\pi}/2$ and $e^{-\pi/2}/2\ \mathrm J$. Combining those independent endpoints and integrals leaves a negative event work $-e^{-\pi}\ \mathrm J$ only for the force-zero deletion of the spring.

Figure \ref{fig:contact} locates the two linear-law release events on the same exact force expression.

![Exact configuration-I contact force before the force-zero gate and the continued linear force up to deformation zero. The shaded time interval denotes the tensile continuation of that linear law.](figures/contact-release.pdf){#fig:contact width=90%}

\FloatBarrier

## A removed store is not a physical destination

At a general force-zero event, $k\delta_-+d\dot\delta_-=0$ implies
\begin{equation}
 U_-=\frac{k\delta_-^2}{2}
     =\frac{d^2\dot\delta_-^2}{2k},\qquad
 W_{\rm deletion}=-U_-.
 \label{eq:removed-contact}
\end{equation}
Velocities can be continuous while this mathematical store disappears. Zero impulse therefore does not establish zero event work. The expression $W_{\rm deletion}$ labels a missing transfer or a missing retained state; it is not added to independently measured destination work a second time.

For a candidate finite unloading path, let the isolated elastic coordinate fall as $z=z_-(1-s/\epsilon)$, $0\leq s\leq\epsilon$. Its outward elastic effort--flow product is $(kz)(-\dot z)$, and direct integration gives $kz_-^2/2=U_-$. A physical receiver attached to that coordinate still requires a specified coupling. Four exclusive destination hypotheses assign this whole transfer to fracture work $\int F_f\dot\ell\,\dd t$, acoustic work $\iint p v_n\,\dd A\dd t$, thermal transfer $\int T\dot S_{\rm out}\,\dd t$, or fixture work $\int F_bv_b\,\dd t$. They predict the four vectors
\begin{equation}
 (U_-,0,0,0),\quad(0,U_-,0,0),\quad
 (0,0,U_-,0),\quad(0,0,0,U_-)
 \label{eq:destination-vectors}
\end{equation}
in that ordered list of outward channels. A mixed destination would require independently identified fractions summing to one under the assumed complete boundary. These exclusive hypotheses are compared separately, never summed as four simultaneous releases.

Synchronized force and motion locate the event and fix $\delta_-,\dot\delta_-$. Contact strain checks $U_-$ under an identified stiffness. Calibrated acoustic intensity, temperature or calorimetric energy, fracture deformation and moving-support work then distinguish \eqref{eq:destination-vectors}. A microphone voltage alone does not determine acoustic energy; temperature alone does not determine heat without heat capacity and boundary flow. A perfectly fixed fixture predicts zero fixture work, so a nonzero fixture destination requires measured compliance or another moving support state.

## Restitution through more than one contact

The same release waveform repeated with incident velocity $v_n$ scales displacement and force by $v_n/v_0$ and each work by its square. If flight returns the same speed magnitude and the same contact law remains valid, then $v_n=e^{n-1}v_0$. For force-zero release,
\begin{equation}
 U_n=\frac{d^2v_0^2}{2k}e^{2n},\qquad
 \sum_{n=1}^{N}U_n=
 \frac{d^2v_0^2}{2k}\frac{e^2(1-e^{2N})}{1-e^2},\quad 0<e<1.
 \label{eq:repeated-release}
\end{equation}
For configuration I, two contacts remove $e^{-\pi}+e^{-2\pi}\ \mathrm J$, and three remove $e^{-\pi}+e^{-2\pi}+e^{-3\pi}\ \mathrm J$. The competing compression-only damping law gives zero deleted spring energy on each contact, with the distinct speed sequence $v_n=e^{-(n-1)\pi/4}\ \mathrm{m/s}$. Measuring release speed as well as destination prevents conflating a changed restitution with a changed energy recipient.

The flight work is explicit. Let separation $s$ leave contact with speed $ev_n$, obey $\ddot s=-a_f$ until turnaround, then the same acceleration until it returns to zero. Its maximum gap is $e^2v_n^2/(2a_f)$ and its duration $2ev_n/a_f$. Integrating the signed motor product $(-ma_f)\dot s$ gives $-me^2v_n^2/2$ outward and $+me^2v_n^2/2$ inward. The net is zero with separately nonzero transfers. If the inward acceleration magnitude is $b_f$, the next incident speed becomes $ev_n\sqrt{b_f/a_f}$ and net motor work is $me^2v_n^2(b_f/a_f-1)/2$. Any actual fixture exchange remains an additional measured port.

This recurrence closes only constant-law flight and contact. A finite extension must distinguish changes in $v_n$ caused by measured motor work from changes in $e$, $k$ or the recipient channels caused by the contact. Friction needs tangential force--slip work; plasticity needs irreversible deformation; adhesion needs a tensile-separation law and its work; acoustic and thermal storage need their own endpoints. A third engagement, an independently changed gap, a changed contact area and a changed damper provide separate finite comparisons against \eqref{eq:repeated-release}. Each omitted constitutive contribution remains in $r_{\rm model}$ until measured. Closure for one material and fixture does not assign a universal restitution law.

# Prepared states and singular passive reductions
\label{sec:singular}

## Derive the constrained topology before its limit

A concrete passive two-store network consists of $R_C\parallel C$ in series with $R_L\parallel L$. Its terminal impedance is
\begin{equation}
 Z(s)=\frac{R_C}{1+sR_CC}+\frac{sLR_L}{R_L+sL}.
 \label{eq:passive-network}
\end{equation}
Kirchhoff's laws give branch states $C\dot v_C=i-v_C/R_C$ and $L\dot i_L=R_L(i-i_L)$. The branch terminal voltages are $v_C$ and $R_L(i-i_L)$. Thus the boundary of the capacitor and inductor has input power $[v_C+R_L(i-i_L)]i$, two separate resistor powers $-v_C^2/R_C$ and $-R_L(i-i_L)^2$, and store $Cv_C^2/2+Li_L^2/2$.

Setting $C=0$ in the branch equations first yields $v_C=R_Ci$; it does not permit an independent initial $v_C$. Setting $L=0$ imposes zero winding voltage; $L\to\infty$ at bounded voltage instead freezes the current over a finite interval and does not remove its preparation. The exact finite components must decide what happens to an incompatible state.

For an illustrative dimensionless evaluation with $R_C=R_L=L=1$, $C=\epsilon$ and $s=1$, \eqref{eq:passive-network} is $1/(1+\epsilon)+1/2\to3/2$. Along $R_C=C=\epsilon$, it is $\epsilon/(1+\epsilon^2)+1/2\to1/2$. At $\epsilon=1/4$, the exact values are $13/10$ and $25/34$. The units are restored with fixed resistance and time scales. These transfer limits follow from different physical families; neither computes an event work.

## A finite prepared family with vanishing charge

Disconnect the terminal current and set the inductor state to zero. A capacitor $C_\epsilon=\epsilon C_*$ prepared to $V_\epsilon=V_*/\sqrt\epsilon$ and discharging through a fixed $R>0$ obeys
\begin{equation}
 v(t)=V_\epsilon e^{-t/(RC_\epsilon)},\quad
 E(0)=E_*:=\tfrac12 C_*V_*^2,
 \quad q(0)=C_*V_*\sqrt\epsilon.
 \label{eq:prepared-singular}
\end{equation}
Although its charge tends to zero, its initial store is finite. The actual resistor effort--flow integral on $[0,T_\epsilon]$ is
\begin{equation}
 W_R=-\int_0^{T_\epsilon}\frac{v(t)^2}{R}\,\dd t
     =-E_*(1-e^{-2h_\epsilon}),\qquad
 E(T_\epsilon)=E_*e^{-2h_\epsilon},\quad
 h_\epsilon=\frac{T_\epsilon}{RC_\epsilon}.
 \label{eq:singular-work}
\end{equation}
The three possibilities $h_\epsilon\to0$, $h_\epsilon\to h>0$ and $h_\epsilon\to\infty$ give resistor works $0$, $-E_*(1-e^{-2h})$ and $-E_*$. These are exact limits of finite integrals, with different endpoint stores. A fixed-voltage preparation instead has initial energy proportional to $\epsilon$ and zero limiting work. A fixed nonzero charge would have unbounded initial energy; it belongs to another preparation class.

Configuration VII takes $C_*=1\ \mathrm{mF}$ and $V_*=2\ \mathrm V$, hence $E_*=2\ \mathrm{mJ}$. The finite member $\epsilon=1/4$ has $C=1/4\ \mathrm{mF}$, initial voltage $4\ \mathrm V$, and $R=1\ \mathrm{k}\Omega$. At $T=(\log2)/4\ \mathrm s$, the final voltage is $2\ \mathrm V$, the store is $1/2\ \mathrm{mJ}$ and $W_R=-3/2\ \mathrm{mJ}$. Its physical absolute charge is $1\ \mathrm{mC}$ initially and $1/2\ \mathrm{mC}$ finally; these are charge observations, not energy measures. The relaxed control has zero voltage, charge, store and work. An inductor discharged through a resistor has the dual formulas with $L$, initial $I$, linkage $LI$ and ratio $RT/L$; charge and linkage magnitudes are never added.

Each member uses fixed components during its interval. Physically changing $C$ or $L$ during that interval would require an additional parameter-actuation port and its effort--flow law. Finite prepared RC/RLC experiments can separate the above families with endpoint voltage/current and resistor power. They cannot realize the diverging voltage at exact $\epsilon=0$. The unresolved broader question is which bounded physical preparation and switching law selects the relevant path, including multiple component ratios and all discarded states.

# Equal endpoints with unequal switch work
\label{sec:connection}

Two capacitors $C_1,C_2>0$ have voltages $v_1,v_2$ and are connected by independently measured parallel conductances $g_A,g_B\geq0$ over $[0,\epsilon]$. Their negative terminals share a fixed return. With $d=v_1-v_2$, $Q=C_1v_1+C_2v_2$, $C_e=C_1C_2/(C_1+C_2)$, Kirchhoff's laws yield
\begin{equation}
 \dot Q=0,\qquad C_e\dot d=-(g_A+g_B)d,\qquad
 E=\frac{Q^2}{2(C_1+C_2)}+\frac{C_ed^2}{2}.
 \label{eq:capacitor-state}
\end{equation}
The boundary contains the two capacitor stores; each conductance is an external dissipative channel with inward power $P_j=-d(g_jd)$. Gate supplies, stray capacitances and magnetic stores are excluded from this ideal law and must be separately instrumented in hardware.

Figure \ref{fig:capacitors} identifies the separate channel currents used in the following integrals.

![Schematic of the two-capacitor boundary and the independently measured connection channels. Currents $i_A=g_A d$ and $i_B=g_B d$ flow from the higher-voltage node to the other node when $d>0$.](figures/capacitor-paths.pdf){#fig:capacitors width=90%}

\FloatBarrier

\begin{theorem}
Suppose $g_j=KC_e\phi_j(t/\epsilon)/\epsilon$, with nonnegative profiles satisfying $\int_0^1\phi_j(u)\dd u=1$. Write $D=C_e(d^-)^2/2$. Both the final difference $d^+=e^{-2K}d^-$ and the total work $-D(1-e^{-4K})$ are independent of ordering. If the two profiles have disjoint supports with $A$ first, their individual works are
\begin{equation}
 W_A=-D(1-e^{-2K}),\qquad
 W_B=-De^{-2K}(1-e^{-2K}).
 \label{eq:partition}
\end{equation}
Reversing their order exchanges the assignments. Identical simultaneous profiles give $W_A=W_B=-D(1-e^{-4K})/2$.
\end{theorem}

Define accumulated action $a(t)=\int_0^t(g_A+g_B)/C_e\,\dd s$. The solved state is $d=d^-e^{-a}$. On the first disjoint channel, substituting $\dd a=g_A\dd t/C_e$ into its own power integral gives $-C_e(d^-)^2\int_0^Ke^{-2a}\dd a$; the second integral has limits $K,2K$. For identical profiles each instantaneous power is half the total. Direct endpoint substitution in \eqref{eq:capacitor-state} gives $\Delta E=-D(1-e^{-4K})$ independently. $\square$

Configuration VIII uses $C_1=C_2=1\ \mathrm{mF}$, $(v_1^-,v_2^-)=(2,0)\ \mathrm V$, and $K=\log2$. Thus $D=1\ \mathrm{mJ}$, $Q=2\ \mathrm{mC}$, and all three paths end at $(v_1^+,v_2^+)=(5/4,3/4)\ \mathrm V$. Initial energy is $2\ \mathrm{mJ}$ and final energy $17/16\ \mathrm{mJ}$.

\Needspace{9\baselineskip}

| Connection path | $W_A$, mJ | $W_B$, mJ | Total work, mJ |
|:-----------------------|----------------:|----------------:|-------------------:|
| $A$ before $B$ | $-3/4$ | $-3/16$ | $-15/16$ |
| $B$ before $A$ | $-3/16$ | $-3/4$ | $-15/16$ |
| Identical coincident profiles | $-15/32$ | $-15/32$ | $-15/16$ |

: A finite event with equal endpoints and distinct channel works for every $\epsilon>0$.

For example, constant $g_A=2KC_e/\epsilon$ on the first half of the interval and $g_B=2KC_e/\epsilon$ on the second half realize the sequential path with finite conductances. Current can jump at their boundaries, while capacitor voltages remain continuous. A finite smooth profile with the same integrated action gives exactly the same sequential work. After connection, a permanent conductance $G_0=C_e/\tau$ gives $d'=-d/\tau$ and each voltage satisfies $v_j''+v_j'/\tau=0$. Before connection, each isolated voltage satisfies $v_j'=0$. The additional accessible difference coordinate, rather than an arbitrary new derivative, determines this order change.

This example settles nonuniqueness of the partition in its scalar family. It also supplies a prepared switching counterexample to inference from a smooth zero-state response. As $\epsilon\to0$ at fixed $K$, the individual integrals retain their different finite values. As $K\to\infty$, the sequential works tend to $(-D,0)$ or $(0,-D)$, whereas identical overlap gives $(-D/2,-D/2)$. Commuting scalar state maps therefore need not determine individual work. Non-scalar state resets can additionally fail to commute.

For arbitrary positive capacitance ratio $r=C_1/C_2$, the same theorem uses $C_e=C_2r/(1+r)$; it is not restricted to a few ratios. The exact $C_1=0$ graph has no independent $v_1$ store and requires its own initial-state constraint. A finite prepared family approaching it can retain energy as in \eqref{eq:prepared-singular}. Wider device laws, overlapping profiles dependent on voltage, non-scalar resets and actual switch-control consumption remain outside this closed family. Measuring both branch powers and both capacitor endpoint voltages separates those remaining physical alternatives.

# Winding opening, clamps and energized returns
\label{sec:transformer}

## A third-order clamp and its separate work integral

Let two lossless windings have symmetric inductance matrix
$\mathsf L=\left(\begin{smallmatrix}L_1&M\\M&L_2\end{smallmatrix}\right)$ with $\Delta=L_1L_2-M^2>0$. The second winding closes through capacitor $C$. Currents enter the positive winding terminals and $C\dot v_C=-i_2$. An opposing primary clamp holds voltage $-V_c$, $V_c>0$, until the first primary current zero. The three state equations are
\begin{equation}
 \mathsf L\binom{\dot i_1}{\dot i_2}=\binom{-V_c}{v_C},
 \qquad C\dot v_C=-i_2.
 \label{eq:clamp-state}
\end{equation}
The boundary comprises magnetic and capacitor stores, $E=(L_1i_1^2+2Mi_1i_2+L_2i_2^2+Cv_C^2)/2$; the clamp is its only external transfer port. The secondary winding/capacitor product cancels only after its two subboundary integrals are evaluated.

For initial state $(i_1,i_2,v_C)=(I,0,0)$, direct solution of \eqref{eq:clamp-state} gives, with $\omega^2=L_1/(C\Delta)$,
\begin{equation}
\begin{aligned}
 v_C&=\frac{MV_c}{L_1}(\cos\omega t-1),\qquad
 i_2=\frac{CMV_c\omega}{L_1}\sin\omega t,\\
 i_1&=I-\frac{V_ct}{L_1}
       -\frac{M^2V_c}{L_1\Delta\omega}\sin\omega t.
\end{aligned}
 \label{eq:clamp-solution}
\end{equation}
Elimination yields $C\Delta i_1^{(3)}+L_1\dot i_1+V_c=0$. At $M=0$ its extra factor is unobservable in the primary response, which is first order. At first-zero opening the retained secondary is second order, with $i_2,v_C$ transported continuously. Thus an actual event can change the scalar order without erasing the remaining stores.

Integrating the sole external product $(-V_c)i_1$ independently gives
\begin{equation}
 W_c(0,t)=-V_cIt+\frac{V_c^2t^2}{2L_1}
  +\frac{M^2V_c^2}{L_1\Delta\omega^2}(1-\cos\omega t).
 \label{eq:clamp-work}
\end{equation}
Substitution of the endpoint currents and voltage in $E$ verifies $\Delta E=W_c$. It does not determine whether a real clamp exports this work to heat, a supply, radiation or another capacitor.

Configuration IX uses $L_1=L_2=1/10\ \mathrm H$, $M=1/20\ \mathrm H$, $C=1/750\ \mathrm F$, $V_c=1\ \mathrm V$, $I=\pi/10\ \mathrm A$. Then $\omega=100\ \mathrm{rad/s}$ and
\begin{equation}
 i_1=\frac{\pi-100t-\sin(100t)/3}{10},\quad
 i_2=\frac{\sin(100t)}{15},\quad v_C=\frac{\cos(100t)-1}{2}.
 \label{eq:clamp-example}
\end{equation}
The derivative of $i_1$ is $-10-(10/3)\cos(100t)<0$, so its first zero is exactly $T=\pi/100\ \mathrm s$. The initial store is $\pi^2/2000\ \mathrm J$; the final state is $(0,0,-1\ \mathrm V)$ and its store is $1/1500\ \mathrm J$. The separately evaluated clamp work is $1/1500-\pi^2/2000\ \mathrm J<0$.

## Another finite removal path and the parasitic scale

A distinct topology temporarily shorts the secondary winding and isolates its initially uncharged capacitor. A primary current controller imposes $i_1=I(1-t/\tau)$ for $0\leq t\leq\tau$. The secondary voltage is exactly zero, so $Mi_1+L_2i_2=MI$ and $i_2=MI t/(L_2\tau)$. The primary voltage is $(L_1-M^2/L_2)\dot i_1$. Its individual integral is
\begin{equation}
 W_{\rm opening}=\int_0^\tau
 (L_1-M^2/L_2)\dot i_1i_1\,\dd t
 =-\frac12(L_1-M^2/L_2)I^2.
 \label{eq:linkage-removal}
\end{equation}
The short has zero voltage and therefore zero work. Reconnecting the secondary to its zero-voltage capacitor can preserve both $i_2$ and $v_C$ under the stated ideal event law. The independent final magnetic store is $M^2I^2/(2L_2)$.

For configuration IX this finite alternative gives $i_2^+=\pi/20\ \mathrm A$, $v_C^+=0$, store $\pi^2/8000\ \mathrm J$ and opening work $-3\pi^2/8000\ \mathrm J$. Its different endpoint and transfer distinguish it from the constant clamp. Sending $\tau$ to zero raises the required primary voltage without selecting a universal physical opening law.

A parasitic capacitor introduces another time scale even in a lossless control. For effective inductance $L_e$ feeding $C_p$, initial $(i,v_p)=(I,0)$ and no source,
\begin{equation}
 i=I\cos\theta,\quad v_p=I\sqrt{L_e/C_p}\sin\theta,\quad
 \theta=\frac{t}{\sqrt{L_eC_p}},\qquad
 \int_0^t v_pi\,\dd s=\frac{L_eI^2}{2}\sin^2\theta.
 \label{eq:parasitic}
\end{equation}
The last integral is positive into the capacitor and negative into the inductor. Their independently evaluated endpoint stores are $E_0\sin^2\theta$ and $E_0\cos^2\theta$, $E_0=L_eI^2/2$. Finite paths with $\tau/\sqrt{L_eC_p}=\pi/2$ deliver $E_0$ to the capacitor; paths with that ratio $\pi$ return its store to zero and reverse the winding current. Both approach $C_p=\tau=0$ along different paths. A resistive or clamped continuation must then assign its own work. Voltage ratings constrain the admissible finite family because $v_p$ need not remain bounded as $C_p\to0$.

The sign of mutual coupling also needs its own control. For the canonical clamp preparation, changing $M$ to $-M$ changes the signs of $i_2$ and $v_C$ but not $W_c$. With both initial winding currents nonzero, the two mutual orientations instead differ in initial store by $2Mi_1i_2$, so that preparation cannot be reused without reevaluating endpoints. At $\Delta=0$, a null vector $n$ of $\mathsf L$ imposes $n^Tv=0$. An incompatible voltage or current preparation requires a specified finite parasitic path; the inverse of $\mathsf L$ in \eqref{eq:clamp-state} is unavailable. These facts resolve particular algebraic controls while leaving device laws, arbitrary joint ratios and the physical destinations open.

## Loaded transformer and actual commutation

A finite transformer with output capacitance has generic scalar order three before additional switch states. Let $\mu=1$ denote a tapped connection and $\mu=0$ an isolated-secondary connection. With source voltage $u$ behind resistance $R_s$, effective core conductance $G_c$, winding resistances $R_1,R_2$, load $G_\ell$ and probe $G_p$, the state laws are
\begin{align}
 v_a&=\frac{u-R_s(i_1-\mu i_2)}{1+R_sG_c},&
 i_s&=i_1-\mu i_2+G_cv_a,\nonumber\\
 \mathsf L\binom{\dot i_1}{\dot i_2}
 &=\binom{v_a}{v_o-\mu v_a}
   -\binom{R_1i_1}{R_2i_2},&
 C_o\dot v_o&=-i_2-(G_\ell+G_p)v_o.
 \label{eq:loaded-transformer}
\end{align}
The boundary contains both magnetic stores including the mutual term, $C_ov_o^2/2$, and the resistors with their heat exported. Its external powers are separately $ui_s$, $-R_si_s^2$, $-R_1i_1^2$, $-R_2i_2^2$, $-G_cv_a^2$, $-G_\ell v_o^2$ and $-G_pv_o^2$. Their sum equals the store derivative by substitution of the circuit equations, not by a choice of store constancy. Appendix \ref{sec:matrix} supplies an exact independent integral for each quadratic power on a constant-connection interval.

Setting $u=0$ in this graph retains $R_s$ and the current paths. Changing a resistive load also leaves $C_o$ attached. Neither action determines the opening law of a winding, the energized overlap of two taps, or the charge transfer of a newly attached return. A voltage-coordinate shift preserves a capacitor's voltage difference; a physical return switch can change that difference by doing work.

For a concrete return connection, join a capacitor $C_r$ at initial voltage $V_0$ to a return-driver voltage $U$ through finite $R_r$. This is a subcircuit for the receiving capacitor and driver path; it does not replace the concurrent winding states. The solved state and independently integrated ports are
\begin{align}
 v(t)&=U+(V_0-U)e^{-t/(R_rC_r)},\nonumber\\
 W_U&=C_rU(U-V_0)(1-e^{-h}),\nonumber\\
 W_{R_r}&=-\tfrac12C_r(U-V_0)^2(1-e^{-2h}),\quad
 h=T/(R_rC_r).
 \label{eq:return-connection}
\end{align}
For $C_r=1\ \mathrm{mF}$, $V_0=1\ \mathrm V$, $U=2\ \mathrm V$ and $h=\log2$, the source gives $1\ \mathrm{mJ}$, the resistor exports $3/8\ \mathrm{mJ}$, and the endpoint store rises from $1/2$ to $9/8\ \mathrm{mJ}$. A coordinate relabeling predicts unchanged capacitor voltage $1\ \mathrm V$ and zero source work. The finite connection predicts $3/2\ \mathrm V$ and nonzero work. The former is a coordinate control; the latter is a changed graph.

A make-before-break tap change can also create a circulating winding loop. For a constant tap-voltage difference $U_t$, loop inductance $L_t$, resistance $R_t>0$ and zero initial loop current, Kirchhoff's law gives $i_t=(U_t/R_t)(1-e^{-R_tt/L_t})$. Over $[0,T]$, with $a_t=R_tT/L_t$,
\begin{align}
 W_t&=\frac{U_t^2}{R_t}\left[T-\frac{L_t}{R_t}(1-e^{-a_t})\right],\nonumber\\*
 W_{R_t}&=-\frac{U_t^2}{R_t}\left[T-\frac{2L_t}{R_t}(1-e^{-a_t})
             +\frac{L_t}{2R_t}(1-e^{-2a_t})\right].
 \label{eq:tap-loop}
\end{align}
The separately evaluated loop store is $L_tU_t^2(1-e^{-a_t})^2/(2R_t^2)$. A break-before-make change instead needs an interruption path for any initial current. A declared finite transformer experiment must retain each winding section, the actual return graph, clamp and switch-control supply. A changed inductance parameter alone specifies none of those transfers. A full switching ledger must combine their separately measured works only after canceling common internal ports.

The finite clamp and connection laws settle their stated paths. Arc ignition, restrike, voltage-dependent conductance, clamp release, winding capacitance and switch-control loss remain constitutive inputs. Identifying them requires voltage and current on the same branch and the same time base, with both event-side states. A low-voltage tapped transformer with finite controlled switches supplies such a comparison; an arc hypothesis needs an identified arc path in its declared operating domain, rather than an extrapolation from a switch that never arcs.

# A source-off transducer and a finite bias supply
\label{sec:transducer}

## Plant and controller are separate boundaries

A reciprocal electrical/mechanical transducer has current $i$, displacement $x$, velocity $v$ and three stored coordinates. A controlled variant obeys
\begin{equation}
 L\dot i=v_s-Ri-g_ev,\qquad \dot x=v,\qquad
 m\dot v=g_mi-cv-kx+F_s.
 \label{eq:plant}
\end{equation}
The plant store is $E_p=Li^2/2+mv^2/2+kx^2/2$. Multiplying the electrical and mechanical equations by their flows derives the port powers $v_si$, $F_sv$, $-Ri^2$, $-cv^2$ and $(g_m-g_e)iv$. Reciprocal coupling has $g_m=g_e$ and the internal transfers cancel. One realization of the controlled law retains a reciprocal device with $g=g_e$ and adds an actuator force $F_a=(g_m-g_e)i$. Its power $F_av$ is a physical controller-to-plant port, with opposite sign into the controller.

The homogeneous characteristic polynomial is
\begin{equation}
 (Ls+R)(ms^2+cs+k)+g_eg_ms,
 \label{eq:transducer-cubic}
\end{equation}
obtained by eliminating $i,v$ while retaining $x$. Its third order does not account for the bias coil or the finite DC link, which belong to a larger connected realization. An unstable controlled law also needs a specified finite observation window; its growing continuation is not a periodic operating state.

## A derived low-force scale

Configuration X chooses time scale $T_*=1/10\ \mathrm s$, current scale $I_*=1/10\ \mathrm A$, displacement scale $X_*=1/100\ \mathrm m$ and velocity scale $V_*=X_*/T_*=1/10\ \mathrm{m/s}$. The component values
\begin{equation}
 L=\tfrac1{10}\ \mathrm H,\quad m=\tfrac1{10}\ \mathrm{kg},\quad
 R=\tfrac12\ \Omega,\quad c=\tfrac12\ \mathrm{N\,s/m},\quad
 k=5\ \mathrm{N/m},\quad g_e=\tfrac12\ \mathrm{V\,s/m},\quad
 g_m=-1\ \mathrm{N/A}
 \label{eq:transducer-scale}
\end{equation}
give electrical effort scale $LI_*/T_*=1/10\ \mathrm V$ and mechanical effort scale $mV_*/T_*=1/10\ \mathrm N$. Writing normalized time $s=t/T_*$, the source-off equations become
$I'=-I/2-V/2$, $X'=V$, $V'=-I-V/2-X/2$. Thus the finite prepared trajectory $I=V=e^{-s}$, $X=-e^{-s}$ is an exact solution. In SI form,
\begin{equation}
 i=\frac{e^{-10t}}{10},\qquad v=\frac{e^{-10t}}{10},\qquad
 x=-\frac{e^{-10t}}{100},\qquad
 0\leq t\leq T=\frac{\log2}{10}\ \mathrm s,
 \label{eq:plant-path}
\end{equation}
with $v_s=F_s=0$. The actuator force is $-3e^{-10t}/20\ \mathrm N$ and its reaction power into the controller is
$P_r=3e^{-20t}/200\ \mathrm W>0$. These values follow from the state laws and the force command, before evaluating any work.

This trajectory is one prepared decaying mode. In normalized frequency $\lambda$, the full characteristic polynomial is $(\lambda+1)(\lambda^2+1/4)$, so two unexcited undamped modes remain. Disturbance rejection and force-tracking robustness require their own finite measurements; they do not follow from the exact trajectory.

The three plant integrals are
\begin{equation}
 W_R=-\frac3{16000}\ \mathrm J,\qquad
 W_c=-\frac3{16000}\ \mathrm J,\qquad
 W_a=-\frac9{16000}\ \mathrm J.
 \label{eq:plant-work}
\end{equation}
Direct state evaluation gives $E_p(0)=1/800\ \mathrm J$, $E_p(T)=1/3200\ \mathrm J$, and their difference $-3/3200\ \mathrm J$ equals the sum. Initial coil current, displacement and velocity are a prepared state. Finite preparation can prescribe differentiable $i,x$ and obtain $v_s=L\dot i+Ri+g_e\dot x$ and $F_s=m\ddot x-g_mi+c\dot x+kx$ from the same equations. Its work belongs to an earlier measured interval and is not inferred from $E_p(0)$.

## Regenerative and dissipative receiving paths

Assume, illustratively, that a converter routes a constant fraction $\eta=4/5$ of $P_r$ into a bias-coil terminal and exports $(1-\eta)P_r$ as heat. Let $L_b=1/10\ \mathrm H$, $R_b=1\ \Omega$, $i_b(0)=1/100\ \mathrm A$, and define positive coil voltage $u_b$ by $L_b\dot i_b+R_bi_b=u_b$, $u_bi_b=\eta P_r$. This is an explicit terminal conversion law; its physical efficiency and bandwidth remain to be measured.

Putting $y=i_b^2$ reduces that law to a linear equation, giving
\begin{equation}
 y'+20y=\frac6{25}e^{-20t},\qquad
 i_b=e^{-10t}\sqrt{\frac1{10000}+\frac6{25}t},\qquad
 u_b=\frac{(3/250)e^{-10t}}{\sqrt{1/10000+(6/25)t}}.
 \label{eq:bias-path}
\end{equation}
The voltage decreases from $6/5\ \mathrm V$, and $i_b^2$ attains its maximum $3e^{-119/120}/250\ \mathrm{A^2}$ at $119/2400\ \mathrm s$, inside the interval. In particular $i_b<\sqrt{3/250}\ \mathrm A<1/5\ \mathrm A$. The bias-coil store change is positive:
\begin{equation}
 \Delta E_b=\frac{3\log2}{10000}-\frac3{800000}\ \mathrm J.
 \label{eq:bias-gain}
\end{equation}
It is obtained by substituting both endpoint currents in $L_bi_b^2/2$. Independently, the integrated reaction, converter heat and winding heat are
\begin{equation}
 W_r=\frac9{16000},\qquad
 W_{\rm conv}=-\frac9{80000},\qquad
 W_{R_b}=-\frac{363}{800000}+\frac{3\log2}{10000}
 \quad\mathrm J.
 \label{eq:bias-work}
\end{equation}
The last expression follows by integrating $-R_bi_b^2$ from \eqref{eq:bias-path}; it is negative. Their sum equals \eqref{eq:bias-gain} without assigning a residual to the coil.

Keep a finite DC link on the controller boundary as well. Let $C_d=1\ \mathrm{mF}$ initially at $5\ \mathrm V$, with a constant illustrative logic demand $P_0=1\ \mathrm{mW}$ and external charger off. If that link supplies only logic on this path, then
\begin{equation}
 V_d(t)=\sqrt{25-2t}\ \mathrm V,\quad
 W_{\rm logic}=-\frac{\log2}{10000}\ \mathrm J,
 \quad E_d(0)=\frac1{80}\ \mathrm J,
 \quad E_d(T)=\frac1{80}-\frac{\log2}{10000}\ \mathrm J.
 \label{eq:dc-link}
\end{equation}
Here the finite link loss is derived from its measured-port model $V_di_d=P_0$ and its capacitor equation. The controller boundary is coil plus link; its inputs are reaction and any charger, its exports are converter heat, winding heat and logic heat. The plant and controller reaction integrals cancel with opposite signs only when the two boundaries are combined. The combined endpoint change is
$-753/800000+\log2/5000\ \mathrm J$, equal to the sum of the five heat integrals in \eqref{eq:plant-work}, \eqref{eq:bias-work} and \eqref{eq:dc-link}, with the internal reaction omitted from that final sum.

Figure \ref{fig:transducer} shows which transfers are internal only after the two ledgers are combined.

![Schematic of separate plant, controller and combined boundaries. The reaction port carries positive work into the controller on the source-off example; coil gain and DC-link change are independent endpoint observations.](figures/transducer-ledger.pdf){#fig:transducer width=100%}

\FloatBarrier

The dissipative alternative sends all $P_r$ to a dump element, with $\eta=0$ and the same force command. Then $i_b=e^{-10t}/100\ \mathrm A$ and $\Delta E_b=-3/800000\ \mathrm J$, while the plant trajectory is identical. It predicts dump export $9/16000\ \mathrm J$; the regenerative path predicts converter export $9/80000\ \mathrm J$ plus the distinct coil heat in \eqref{eq:bias-work}. Bias-terminal voltage/current and both coil endpoints distinguish these paths even when the plant motion does not.

The scale is compatible with a low-voltage, low-force laboratory design: required ranges are within $\pm6\ \mathrm V$ including the DC link, $\pm1/5\ \mathrm A$, $\pm1/5\ \mathrm N$, $\pm1/50\ \mathrm m$ and $\pm1/5\ \mathrm{m/s}$ on a window shorter than $1/10\ \mathrm s$. The actuator must accept reverse power while tracking the specified force; the finite link must actually power sensing and logic. Synchronized electrical and force--velocity integrals are the primary transfer readouts. Coil and converter thermal measurements require a calibrated heat capacity or calorimetric boundary; repeated preparations must be included if repetition is used to increase the thermal signal. These ranges are design requirements derived from the trajectory, not measured component performance.

This construction uses an actively commanded force and an independently controlled regenerative receiver. It establishes a feasible scale and exact conditional predictions, not a realization of every bias-dependent coupling law. In a controller whose $g_e,g_m$ depend directly on the changing $i_b$, their dynamics must be retained and \eqref{eq:plant-path} need not remain a solution. Finite-precision uncertainties in unstable prefixes, thermal endpoints, separate quadrature, interval balances and integrated DC-link ledgers remain unresolved for the earlier broader models; an exact local example does not certify those computations. Physical conversion efficiency, sensor/logic power, saturation, coil material and source return are still model residuals requiring measurement.

# An accelerating reference requires a supplied counterpart
\label{sec:reference}

## Relative kinetic storage and a physical capacitor

For a rotor about a fixed axis, $J\dot\omega=\tau$. A prescribed reference has rate $\Omega(t)$, so the relative rate $w_m=\omega-\Omega$ obeys $J\dot w_m=\tau-J\dot\Omega$. Multiplying the independently derived equation by $w_m$ gives
\begin{equation}
 E_\Omega=\tfrac12J(\omega-\Omega)^2,\qquad
 P_\tau=\tau(\omega-\Omega),\qquad
 P_\Omega=-J\dot\Omega(\omega-\Omega),\qquad
 \dot E_\Omega=P_\tau+P_\Omega.
 \label{eq:frame}
\end{equation}
The second product is the Euler contribution to this frame ledger. For zero physical torque, the ground-frame rotor store is constant while $E_\Omega$ can change. An electrical realization of $E_\Omega$ therefore needs a physical source that represents $P_\Omega$; changing a voltage origin supplies no such source.

Take a capacitor between nodes A and R, with $C=J/\alpha^2$, prescribed $V_R=\alpha\Omega$ and capacitor voltage $w_e=V_A-V_R$. Two floating sources, outside the capacitor boundary, inject from R to A:
\begin{equation}
 I_\tau=\tau/\alpha,\qquad I_\Omega=-C\dot V_R,
 \qquad C\dot w_e=I_\tau+I_\Omega.
 \label{eq:reference-cell}
\end{equation}
With compatible initial states, the equations give $V_A=\alpha\omega$, $w_e=\alpha(\omega-\Omega)$, and $Cw_e^2/2=E_\Omega$. The actual physical source powers are $w_eI_\tau=P_\tau$ and $w_eI_\Omega=P_\Omega$. Node R draws zero net bias current from an ideal reference driver because all three A--R branches sum to zero current. This KCL fact does not eliminate the energy needed by the driver's own states or the floating-source supplies.

Let a separate finite RC driver set $V_R$, with capacitance $C_d$ from R to ground O and resistance $R_d$ from a voltage command $u$ to R. Its state equation is $C_d\dot V_R=(u-V_R)/R_d$ in this zero-load ideal cell. Deriving $u=V_R+R_dC_d\dot V_R$ from the desired state path gives independently signed driver powers $uI_d$ and $-R_dI_d^2$, where $I_d=C_d\dot V_R$. Its store is $C_dV_R^2/2$ and its output power to the cell is zero on this topology.

Figure \ref{fig:reference} distinguishes the floating compensation source from the finite reference driver.

![Schematic of the prescribed-reference capacitor cell. Both floating source powers use the physical capacitor voltage $w_e$. The RC driver has its own command input, resistor export and capacitor endpoint store.](figures/reference-cell.pdf){#fig:reference width=100%}

\FloatBarrier

Configuration XI sets $J=1/10\ \mathrm{kg\,m^2}$, $\alpha=1\ \mathrm{V/(rad/s)}$, $C=1/10\ \mathrm F$, zero initial states, $\tau=0$, and $\Omega=2t\ \mathrm{rad/s}$ on $[0,1]\ \mathrm s$. Then $\omega=V_A=0$, $w_e=-2t\ \mathrm V$ and $I_\Omega=-1/5\ \mathrm A$. Separately integrating $w_eI_\Omega=(2/5)t\ \mathrm W$ gives $+1/5\ \mathrm J$. With $C_d=1/200\ \mathrm F$ and $R_d=3/4\ \Omega$, the command is $u=2t+3/400\ \mathrm V$ and $I_d=1/100\ \mathrm A$.

| Boundary | Individual signed works on $[0,1]$, J | Initial store, J | Final store, J |
|:-------------------------|:-----------------------------------------------|------------------:|----------------:|
| Receiver capacitor | Shaft $0$; compensation $1/5$; bias $0$ | $0$ | $1/5$ |
| Mechanical relative-rate ledger | Shaft $0$; Euler $1/5$ | $0$ | $1/5$ |
| Ground-frame rotor | Shaft $0$ | $0$ | $0$ |
| RC driver | Command $403/40000$; resistor $-3/40000$; output $0$ | $0$ | $1/100$ |

: Independent exact boundaries for configuration XI. The physical receiver and driver together have final store $21/100\ \mathrm J$ and zero signed residual after their own port integrals are combined.

Disabling compensation sets $I_\Omega=0$. Then $w_e=0$, A follows R, and receiver store and source work both remain zero. Its final store differs from the relative mechanical target by $-1/5\ \mathrm J$, while both independently evaluated boundary residuals remain zero. This is a failure of the proposed state/port correspondence under that connection. It does not erase either distinct store or source reading.

The ideal active cell closes its prescribed-reference question. Actual floating-source rail work still requires a supply model. For a purely receiving compensation interval of $1/5\ \mathrm J$, constant illustrative efficiency $\eta_s$ and zero standby demand predict rail input $1/(5\eta_s)\ \mathrm J$: $1/5$ for $\eta_s=1$ and $1/4$ for $\eta_s=4/5$. The finite driver command work $403/40000\ \mathrm J$ is additional in both cases. Measured rail voltage/current distinguishes those supply hypotheses; a zero bias-output current distinguishes neither.

## What the single cell does not settle for a compound system

For several coaxial inertias $J_j$ with elastic potentials depending only on relative angles, let $\omega_j$ be their rates and $\tau_j$ the external shaft torques. Pairwise internal spring forces follow from their constitutive laws; pairwise damping is $d_{jk}(\omega_j-\omega_k)$. Summing the individual equations after multiplying by $\omega_j-\Omega$ combines the spring powers into $\dot U$ and retains the damping products as signed losses, giving
\begin{equation}
 \dot E_\Omega=\sum_j\tau_j(\omega_j-\Omega)
 -\dot\Omega\sum_jJ_j(\omega_j-\Omega)
 -\sum_{j<k}d_{jk}(\omega_j-\omega_k)^2,
 \label{eq:compound-frame}
\end{equation}
where $E_\Omega=\sum_jJ_j(\omega_j-\Omega)^2/2+U$. The sum here explicitly assumes only those internal potentials. A spring grounded to a moving frame introduces the corresponding base-displacement dependence and its support work. Constraints must be imposed on the equations and their allowed velocities before multiplying by flows.

If $\Omega$ is itself the rate of a carrier inside the compound system, $\dot\Omega$ is determined by coupled forces and driver loading. It cannot be prescribed independently by the single RC command above. A finite electrical counterpart must realize that causal dependency, preserve all winding/receiver states, and include the compensation supplies for the resulting current vector. Neither a common coordinate shift nor equality of a terminal power ratio supplies this driver.

An energized locking control shows the event issue exactly. Two otherwise free rotors connected by a finite viscous coupling $d$ have fixed total angular momentum and relative rate $\delta\omega(t)=\delta\omega_0e^{-dt/J_e}$, $J_e=J_1J_2/(J_1+J_2)$. Their external damping work is
\begin{equation}
 W_d=-\int_0^T d(\delta\omega)^2\dd t
 =-\frac{J_e(\delta\omega_0)^2}{2}(1-e^{-2dT/J_e}).
 \label{eq:locking}
\end{equation}
For $J_1=J_2=1\ \mathrm{kg\,m^2}$, initial rates $(1,0)\ \mathrm{rad/s}$ and $dT/J_e=\log2$, final rates are $(3/4,1/4)\ \mathrm{rad/s}$, initial kinetic store $1/2\ \mathrm J$, final store $5/16\ \mathrm J$, and $W_d=-3/16\ \mathrm J$. The exact locked limit instead has rates $(1/2,1/2)$ and store $1/4\ \mathrm J$. A lossless relative-motion receiver could retain the difference energy rather than heating it; that is a different finite path with an added state and transfer port. A compound lock or electrical clamp requires this choice to be made for every constraint, including its drive and reference paths.

A zero-net-work control also requires signed interval resolution. With configuration XI's $J$, zero reference acceleration and $\tau=J(1-2t)$ on $[0,1]\ \mathrm s$, the exact rate is $\omega=t-t^2$. Integrating $\tau\omega$ gives $+1/320\ \mathrm J$ on $[0,1/2]$ and $-1/320\ \mathrm J$ on $[1/2,1]$, with both endpoint stores zero. Under delivery efficiency $\eta_s$ and recovery efficiency $\eta_r$, a rail supporting these two signs has net work $(1/320)(1/\eta_s-\eta_r)\ \mathrm J$, before standby loss. Zero signed receiver work therefore does not determine zero rail work. This polynomial cell establishes all its power zeros directly; it does not establish root completeness for a coupled compound trajectory.

The full compound question retains the state-dependent driver, singular constrained states, energized locking and clamping, ideal-limit reduction and physical supply costs. Earlier finite correspondence calculations have bounded numerical support with empirical accuracy estimates; those estimates are not rigorous enclosures over continuous event families. The remaining measurement must instrument the reference-driver and receiver supplies separately, together with mechanical shaft torque and rate where correspondence is asserted.

# Measurements that discriminate the retained alternatives
\label{sec:measurements}

The comparisons below state a finite observable for every question introduced in Section \ref{sec:introduction}. Predictions are conditional on the explicitly declared models. A hardware result closes a stated comparison when its calibrated uncertainty intervals separate the competing values and its complete signed ledger includes both endpoints, each transfer port and the actual event sides. If intervals overlap, the result remains unresolved; if neither prediction agrees, the specified models require revision with the signed disagreement retained. There are no measured outcomes in these tables.

\Needspace{12\baselineskip}

## Identification and correspondence

| Question and held condition | Measured comparison | Exact alternative predictions |
|:-------------------------------------|:----------------------------------------|:------------------------------------------|
| Damped analogy: retain I's finite preparation, free interval and reset | Independent mechanical $f\dot x$ and electrical $Vi$ integrals | Full map gives source works $(23/30,0,23e^{-\pi}/30)\ \mathrm J$ in both devices; omitting the preparation/reset ports records $(0,0,0)$ while endpoint states differ from rest |
| Contact/support assignment: hold II's torque and hammer angle | Anvil angle and contact deformation; then support motion for a dynamic rational model | Anvil $1/2$ versus $2/3\ \mathrm{rad}$ despite hammer $1\ \mathrm{rad}$ in both |
| Weak coefficient: retain III's two calibration points with $\eta=1$ | Independently set $(\rho,\eta)=(1,2)$ and estimate normalized coefficient with full covariance | $151/50$ versus $301/100$; the difference is $1/100$ |
| Resonator transfer: change only the independently known shunt | Calibrated complex admittance on each device and fixture | IV gives $1+\ii$ versus $1+2\ii\ \mathrm S$; a series-only description gives $1\ \mathrm S$ |
| Polarization order: hold zero terminal current and equal time constants | Branch voltages at $\log2\ \mathrm s$, then split time constants | V gives $(1/2,-1/2)\ \mathrm V$ versus $(0,0)$; split constants give terminal $1/2-1/\sqrt2\ \mathrm V$ versus zero |
| Absorber stress: hold VI's force and antiresonant frequency | Coupling strain/stress and absorber motion alongside reaction | Reaction is zero in both; stress amplitude is $1$ versus $1/2\ \mathrm{MPa}$ |

: Exact finite comparisons for the six inherited questions. The first comparison identifies an omitted audit port, not a second correctly prepared physical trajectory.

For the damped analogy, forces/torques and motions, not homogeneous equation coefficients alone, must be transported through preparation and reset. The contact experiment must vary support and contact independently, first within a declared finite constitutive family; failure of added anvil data to resolve a frequency-dependent support requires a support sensor or a narrower model, not an assertion of full identification. The coefficient experiment must retain temporal correlation and calibration covariance when evaluating the $1/100$ separation. A successful comparison on the declared support does not prove that support globally minimal.

The resonator task remains an acquisition across physical devices, calibrated fixtures and independently changed shunts. The normalized example predicts a discriminant but supplies no substitute traces. Polarization order recovery requires independently prepared branches, a finite time-constant separation domain and actual noise bounds. The absorber's bounded inability to infer stress from terminal reaction is already resolved; calibrated strain, section area and material conversion address the remaining practical extension. None of these identification questions is made into an energy anomaly by uncertainty alone.

\Needspace{12\baselineskip}

## Release law, destination and continuation

| Distinct release question | What is held or changed | Predictions that separate the readings |
|:-------------------------------------|:-------------------------------------------|:-------------------------------------------|
| Destination of a force-zero store | Hold I's incident state and force-zero gate; measure contact strain and each receiver channel | Fracture, acoustic, thermal and fixture alternatives give the distinct vectors in \eqref{eq:destination-vectors}, with $U_-=e^{-\pi}\ \mathrm J$ |
| Constitutive separation criterion | Hold $m,d,k,v_0$ and resolve force, deformation and velocity through release | $(t,e)=(\pi/2,e^{-\pi/2})$, $(\pi,e^{-\pi})$, or $(\pi/4+\pi/(2\sqrt2),e^{-\pi/4})$ |
| Repeated restitution and destination | Measure both incoming speeds and receiver work for two contacts, plus signed flight drive | Force-zero deletion totals $e^{-\pi}+e^{-2\pi}\ \mathrm J$ under matched flight; compression-only damping gives zero deletion and a different outgoing speed |
| Wider constitutive behavior | Add a third engagement; change gap, area or damping independently and record tangential, thermal and fixture channels | Constant force-zero law adds $e^{-3\pi}\ \mathrm J$ for the third matched-flight contact; compression-only law adds zero; any extra material transfer requires its own measured effort--flow product |

: The same force/motion instrument can support several comparisons, but destination, release criterion, repeated restitution and wider material behavior have separate closure requirements.

An unchanged gap affects flight timing but not the constant-law contact recurrence. A different measured recurrence after accounting for actual incident velocity distinguishes the unchanged-law reading from material memory or a changed geometry; it does not by itself identify which one. Friction is separated with tangential force and slip, plasticity with permanent deformation and its force history, adhesion with tensile work, motor ripple with drive torque and rate, and thermal/acoustic transfer with calibrated receiver boundaries. Unknown additional laws have no universal numerical prediction; their conditional values require constitutive measurements. The exact zero-deletion and positive-deletion alternatives above remain distinct, finite controls while those laws are identified.

\Needspace{12\baselineskip}

## Singular paths, switching and transformer returns

| Distinct switching question | Boundary readout and controlled change | Exact alternative predictions |
|:-------------------------------------|:------------------------------------------|:--------------------------------------------|
| Incompatible preparation and component coscaling | Prepare VII, measure both endpoints and resistor $vi$; compare relaxed preparation | $E^+=1/2\ \mathrm{mJ}$, $W_R=-3/2\ \mathrm{mJ}$ versus $(0,0)$; $h=0,h=\log2,h\to\infty$ predict limiting works $0,-3E_*/4,-E_*$ |
| Switching work beyond a zero-state response | Hold VIII's prepared voltages and final state; interchange two finite paths | $(W_A,W_B)=(-3/4,-3/16)$ versus $(-3/16,-3/4)\ \mathrm{mJ}$ |
| Instantaneous partition | Shrink finite duration at fixed integrated conductance; compare sequential and overlapping paths | Sequential pair as above versus $(-15/32,-15/32)\ \mathrm{mJ}$; all endpoints agree |
| Actual switch/gap and clamp release law | Record winding, switch, clamp and receiver powers and event states | IX constant clamp: $v_C^+=-1\ \mathrm V$, $i_2^+=0$, $W_c=1/1500-\pi^2/2000\ \mathrm J$; secondary-short path: $v_C^+=0$, $i_2^+=\pi/20\ \mathrm A$, $W=-3\pi^2/8000\ \mathrm J$ |
| Joint zero limits, ratios and orientations | Vary finite $C_p$, duration and coupling sign with known preparation | Capacitor fraction $\sin^2\theta$: $1$ at $\theta=\pi/2$, $0$ at $\theta=\pi$; canonical $M$ reversal reverses secondary voltage/current signs; two prepared currents change the store by $2Mi_1i_2$ |
| Transformer opening, tap and return commutation | Retain separate winding sections; measure clamp, overlap loop, return and control rails | For the finite return example, $v^+=3/2\ \mathrm V$, source work $1\ \mathrm{mJ}$; a coordinate change gives $v^+=1\ \mathrm V$, work zero. Winding-opening alternatives are the two IX paths |

: Each work is measured on its named branch. Equality of their total or of the terminal waveform does not establish equality of their partitions.

The prepared-network comparison must cover the stated component and preparation families, including charge and linkage observations separately, before a singular physical path is assigned. The two-capacitor proof already settles path dependence within its scalar model; hardware closure concerns the measured voltage-dependent switch laws and added stores. The two finite clamp models neither identify an arc nor establish a full release topology. Arc ignition/restrike and clamp release require actual branch conductance and both event-side states on the relevant finite operating interval. Finite ratio measurements cannot establish an entire continuous singular surface without an analytic bound; \eqref{eq:parasitic} supplies such an exact result only for its stated lossless cell.

For the transformer, make-before-break and break-before-make choices must preserve the actual winding incidence and initial linkages. The return-capacitor reading in \eqref{eq:return-connection} distinguishes a physical reconnection from a coordinate shift; the loop reading in \eqref{eq:tap-loop} accounts for an energized overlap. Capacitor charge sharing adds the separate channel comparison of Section \ref{sec:connection}. Switch-control supplies remain measured external ports even if winding and capacitor balance closes without them in an ideal model.

\Needspace{12\baselineskip}

## Controlled supply and accelerating reference

| Remaining question | Independently instrumented quantities | Exact conditional alternatives |
|:---------------------------------|:------------------------------------------|:---------------------------------------------|
| Source-off bias-coil transfer | X's plant $F_av$, coil $u_bi_b$, DC-link power and both endpoint stores | Regenerative $\Delta E_b=3\log2/10000-3/800000\ \mathrm J$ versus dissipative $-3/800000\ \mathrm J$, with identical plant states; reaction work is $9/16000\ \mathrm J$ in both |
| Physical accelerating-reference correspondence | XI's receiver compensation, separate driver command and actual supply rails; shaft torque/rate for the mechanical comparison | Compensation gives receiver store/work $1/5\ \mathrm J$ versus zero without it. Driver command is $403/40000\ \mathrm J$ in both; compensation rail input is $1/5$ or $1/4\ \mathrm J$ for efficiencies $1$ or $4/5$ |

: Supply costs and state correspondence require different measurements. A receiver balance alone determines neither converter efficiency nor the compound driver.

In the transducer, the plant controller force must be observed independently of its command, and the DC-link subledger must close separately. A positive coil change is compared with signed actuator reaction and all supply paths. The illustrative efficiency law cannot be used as a measured result. The accelerating-reference experiment must likewise distinguish the settled prescribed cell from a full compound driver: reference motion dependent on internal carrier state, constraint events and ideal-limit reduction require additional states and causal connections. A signed zero-work interval must retain its positive and negative portions; \eqref{eq:locking} and the reversal control provide local discriminants, with wider compound event coverage still open.

# Relation to earlier work

[*Third- and Higher-Order ODEs*][main] supplies the broader distinction between coefficient constructions, state elimination and physical realization. The present results develop its open questions by attaching explicit preparations, event paths, recipient channels and calibrated observations. The complete finite port correspondence in \eqref{eq:analogy}, the distinct contact release laws and the two-channel work partition each identify information absent from a scalar trajectory.

[Wettstein, Grauberger and Matthiesen (2021)][wettstein] relate hammer-mechanism behavior to a changing sequence of contacts and embodiment relations. That modeling context motivates retaining contact and support coordinates through engagement. The exact release destination and repeated constitutive law here require their own measurements. [Bible (2002)][bible] describes the conventional crystal motional branch and shunt capacitance used in \eqref{eq:resonator}; that component description does not establish a transferable coefficient law across arbitrary devices. [Keysight Technologies (2026)][keysight] explains impedance methods and fixture compensation. Those measurement distinctions support the calibrated complex-port comparison, while uncertainty and internal-state identification remain specific to the apparatus and model class.

# Conclusions

Damped correspondence can be proved for complete finite preparations and resets: configuration I predicts source works $23/30$, zero and $23e^{-\pi}/30\ \mathrm J$. Contact/support ambiguity, weak coefficient recovery, resonator transfer and polarization order require independent internal or component variation. Their exact discriminants are, respectively, anvil angles $1/2$ and $2/3\ \mathrm{rad}$, coefficient separation $1/100$, changed imaginary admittance, and opposite hidden branch voltages. The bounded absorber conclusion remains resolved: zero reaction coexists with different coupling stresses, including $1$ and $1/2\ \mathrm{MPa}$ in configuration VI; calibrated internal measurements address the practical extension.

Force-zero release in configuration I removes $e^{-\pi}\ \mathrm J$ of spring store, whose physical destination remains unidentified. Alternative separation laws predict distinct release times, restitution and zero deleted store. Two and three constant-law impacts predict the exact sums in \eqref{eq:repeated-release}; measured drive work and material channels must distinguish a changed incident state, a changed restitution law and a changed recipient. Friction, plasticity, adhesion and evolving fixtures require additional constitutive work, beyond that recurrence.

A prepared singular RC family can retain finite energy while charge vanishes, with work set by the finite time-scale ratio. Equal capacitor endpoints can also conceal $(-3/4,-3/16)$ or reversed channel works in millijoules. The scalar partition result is settled; actual switch laws, joint zero limits, orientations and additional reset coordinates remain open physical extensions. Constant-voltage winding clamps, linkage-preserving removal, energized tap overlap and physical return reconnection have different exact state and work predictions. Their real clamp, arc, parasitic and control-supply recipients require separate branch measurements.

A source-off transducer can deliver $9/16000\ \mathrm J$ of actuator reaction to a controller while its bias coil gains the positive store in \eqref{eq:bias-gain}. The scaled finite example specifies the force and electrical ranges needed to distinguish regeneration from a dissipative receiving path, while the broader supply realization and unresolved numerical uncertainties remain separate. An accelerating-reference capacitor can receive $1/5\ \mathrm J$ through compensation while its finite driver consumes additional command work. That prescribed cell is settled; state-dependent compound drivers, energized constraints and actual rail costs are not fixed by it. For every boundary, the decisive comparison is a separately integrated signed effort--flow transfer against independently evaluated endpoint states and a declared physical recipient.

\appendix

# Closed work integrals for a finite linear connection
\label{sec:matrix}

Some finite models above, such as \eqref{eq:loaded-transformer}, have a less convenient modal expression than the worked controls. They still permit exact separate port integrals without time integration. On an interval with fixed components and constant source, augment the state with a constant coordinate so that $z'=Gz$ and $z(t)=e^{Gt}z_0$. Each affine effort times affine flow becomes $P_\ell=z^TH_\ell z$, with $H_\ell$ the symmetric part of their outer product. A resistor has the corresponding negative quadratic matrix. Define the entire scalar function $\Phi_T(\xi)=(e^{T\xi}-1)/\xi$, extended by $\Phi_T(0)=T$ and by its derivatives on Jordan blocks.

\begin{lemma}
For any finite real matrix $G$ and any quadratic port matrix $H_\ell$,
\begin{equation}
 W_\ell=(z_0\otimes z_0)^T
 \Phi_T(G^T\otimes I+I\otimes G^T)\operatorname{vec}(H_\ell).
 \label{eq:matrix-work}
\end{equation}
The formula remains exact for repeated or zero eigenvalues.
\end{lemma}

Column vectorization gives
$\operatorname{vec}(e^{G^Tt}H_\ell e^{Gt})
=e^{(G^T\otimes I+I\otimes G^T)t}\operatorname{vec}(H_\ell)$.
Integrating this expression gives \eqref{eq:matrix-work}; the entire extension removes any division by a zero eigenvalue. Multiplication by $z_0\otimes z_0$ recovers the original effort--flow integral. $\square$

Store endpoints are instead evaluated from $x_0$ and the physical components of $e^{GT}z_0$. A new connection has a new matrix and the actual transported state, including any separately specified impulse. Equation \eqref{eq:matrix-work} is not an event law, and it does not supply a missing switch port. Polynomial or sinusoidal drives can be included through their exact finite generating states on a declared interval; no numerical evolution is required.

# Exact checks and scope of the calculations

| Construction | Independent algebraic check | What remains outside the identity |
|:----------------------------|:---------------------------------------------|:--------------------------------------|
| Damped map | Substitute \eqref{eq:analogy} in the two element equations and each power | Hardware gains, preparation authority and unmapped release |
| Contact | Differentiate \eqref{eq:contact-solution}; integrate damping on each actual law | Constitutive separation and recipient channels |
| Identification | Static force balance, nonzero design determinant, exact hidden difference mode | Covariance, noise, model-family choice and calibrated stress |
| Singular RC | Integrate $-v^2/R$ before evaluating both capacitor endpoints | Physical approach and voltage constraints at zero capacitance |
| Two capacitors | Integrate each accumulated-action interval separately | Measured conductance, control supply and additional states |
| Clamp | Substitute all three states in \eqref{eq:clamp-state}; integrate $-V_ci_1$ | Real opening, arc/restrike and release destinations |
| Controlled plant | Substitute \eqref{eq:plant-path}; integrate each loss and reaction | Bias-dependent gains and actual actuator tracking |
| Bias and link | Differentiate $i_b^2$ and $V_d^2$; integrate each controller port | Converter efficiency, sensing, thermal material and supply hardware |
| Reference cell | Independently solve mechanical, capacitor and driver laws | Full compound causal driver and constrained events |

: The exact constructions have zero numerical integration residual. Named omitted mechanisms remain unevaluated model residuals.

Every figure is either a schematic or the exact closed form given in the text. All tabulated works and endpoints follow by algebra and integration of those forms. No decimal residual, finite-precision failure or coordinate magnitude has been used as physical evidence. The bounded structural and prescribed-cell conclusions remain bounded; resolving an inherited local question does not replace its practical measurement extension.

\Needspace{16\baselineskip}

# References {-}

1. Nilre, H., and Herlin, B. C. (2026). [*Third- and Higher-Order ODEs: Coefficient families, physical realizations, identification, and initial data*][main]. Companion manuscript, latest PDF on GitHub.
2. Wettstein, A., Grauberger, P., and Matthiesen, S. (2021). [Modeling dynamic mechanical system behavior using sequence modeling of embodiment function relations: case study on a hammer mechanism][wettstein]. *SN Applied Sciences* **3**, article 128. DOI: 10.1007/s42452-021-04149-8.
3. Bible, S. (2002). [Crystal Oscillator Basics and Crystal Selection for rfPIC and PICmicro Devices][bible]. Microchip Technology, Application Note AN826, DS00826A, pp. 1--14.
4. Keysight Technologies (2026). [*Impedance Measurement Handbook: A Guide to Measurement Technology and Techniques*][keysight]. Application note 5950-3000, 6th edition, published February 28, 2026.

[main]: https://github.com/hobnilre/physics-ode-3rd-deg/blob/main/third-and-higher-order-odes.pdf
[wettstein]: https://doi.org/10.1007/s42452-021-04149-8
[bible]: https://ww1.microchip.com/downloads/en/appnotes/00826a.pdf
[keysight]: https://www.keysight.com/us/en/assets/7018-06840/application-notes/5950-3000.pdf
