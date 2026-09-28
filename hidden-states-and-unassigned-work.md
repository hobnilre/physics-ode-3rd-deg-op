---
title: "Hidden States and Unassigned Work"
subtitle: "Exact models and decisive measurements for higher-order ODEs"
author: "Hob Nilre & Bo C. Herlin"
date: "2026-09-27"
abstract: |
  Force-zero contact release removes a positive elastic store whose fracture, acoustic, thermal or fixture destination remains unidentified. Equal capacitor endpoints admit unequal individual switch works, and a controlled source-off transducer admits a positive bias-coil store change whose complete physical supply realization remains open. Exact finite models expose these transfers: a contact releases $e^{-\pi}\ \mathrm J$, two switch channels exchange the assignments $-3/4$ and $-3/16\ \mathrm{mJ}$, and a receiving bias coil gains $(3\log2/10000-3/800000)\ \mathrm J$. Preparation and residual material strain, complete transformer commutation, and separately supplied accelerating references determine what must be measured. Conditional identification formulas retain the six inherited state and observation questions. All eighteen questions distinguish established model results from unresolved physical laws. Independently integrated signed powers, both endpoint stores and calibrated uncertainty define a test that preserves any unexplained gain or deficit. The derivations use closed forms and predict finite instrumentable comparisons.
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

\begingroup\scriptsize\noindent PDF created: \pdfbuildtimestamp\par\noindent Latest on GitHub: \url{https://github.com/hobnilre/physics-ode-3rd-deg-op}\par\endgroup

# Open transfers and hidden states
\label{sec:introduction}

The open physical questions concern the energy retained, released or redirected when a preparation, contact or electrical connection changes. A third- or fourth-order equation can describe one measured coordinate while leaving those transfers undetermined. The distinction between differential order, observable order and physical storage developed in [*Third- and Higher-Order ODEs*][main] connects the transfer questions to the states that a terminal trace conceals. The six inherited questions establish that connection; the energy questions then determine the order of the developments below.

The damped correspondence question is whether a collision or oscillator and an electrical circuit with positive damping can transport preparation, relaxation and reset ports as well as their homogeneous equations [OP-LR50-01]. Contact identification asks whether hammer measurements, supplemented by anvil measurements, can separate contact coefficients from a frequency-dependent support; an additional support state can remain inaccessible [OP-LR08-01]. Coefficient identification asks whether independently varied physical coordinates and correlated or temporally colored uncertainty permit recovery of weak contributions that are indistinguishable on a restricted path [OP-LR31-01].

The resonator question requires calibrated impedance measurements across devices and fixtures, including the shunt state that changes the rational port law [OP-LR12-01]. The polarization question concerns order recovery with arbitrary branch preparations and noisy data: equal-time-constant branches can contain an independently decaying difference state absent from the terminal current [OP-LR01-04]. For a tuned absorber, the bounded conclusion that terminal reaction alone does not identify internal coupling stress is resolved; the remaining practical question is which calibrated internal observations identify that stress in physical devices and wider models [OP-LR58-01]. A zero reaction with finite coupling strain is a direct control for that distinction.

The energy questions arise at more specific boundaries. A linear contact released when force first reaches zero retains $U_c=d^2v_-^2/(2k)>0$ if its separation speed $v_-$ is nonzero. Removing the contact state assigns a negative event work to the retained system but leaves the fracture, acoustic, thermal or fixture destination unidentified [OP-LR03-01]. Choosing force-zero, deformation-zero or a law with damping only in compression gives different restitution and release stores; the constitutive choice is unresolved [OP-LR03-02]. Across repeated impacts, both the destination and the restitution law need identification for each engagement [OP-LR04-01]. Friction, plasticity, adhesion, motor ripple, additional engagements and changing gaps, contact geometry or damping can alter the accumulated transfer, beyond a fixed two-impact model [OP-LR04-02]. Section \ref{sec:contact} gives positive removed work $e^{-\pi}\ \mathrm J$ in one exact force-zero example, and zero removed spring store for two distinct alternative laws.

Singular passive-network reductions can discard a prepared reactive state with finite energy even when its terminal charge or linkage vanishes. Which component coscalings, endpoint stores and impulse works describe the physical approach is unresolved [OP-LR21-01]. A zero-state smooth response does not determine the signed switching work of that prepared system [OP-LR21-02]. For two connected capacitors the total difference-store decrease can be fixed while the individual channel works differ: in Section \ref{sec:connection}, the same endpoints accompany $(-3/4,-3/16)\ \mathrm{mJ}$ or the reversed pair [OP-LR48-02]. Actual switch and gap laws, arc ignition and restrike, winding capacitance and clamp release must determine where the transfer goes [OP-LR48-03]. The joint approaches to zero parasitic capacitance and zero duration, other coupling orientations and continuous or wider limiting ratios remain separate questions [OP-LR48-05]. Exact zero duration and zero capacitance are mathematical boundaries, not apparatus settings.

In a loaded transformer, switching a source voltage to zero retains a conductor path. Actual winding opening, energized tap or return commutation and capacitor charge sharing require individual winding, clamp, return and control-supply work that this operation does not specify [OP-TRF-02]. The controlled third-order transducer raises a different question: during source-off operation a positive bias-coil energy change can accompany actuator reaction work into its controller, while the finite supply realization and its complete physical ledger remain unresolved [OP-LR59-02]. Section \ref{sec:transducer} derives an instrumentable conditional example with bias-store change $(3\log 2/10000-3/800000)\ \mathrm J>0$.

Finally, an accelerating mechanical reference changes relative kinetic storage. Its electrical counterpart needs an actual compensation source, with work of either sign. Prescribed and state-dependent compound references admit bounded active constructions; finite constraint paths and conditional rigid reductions also have specified models. The remaining physical question is whether finite mechanical and electrical realizations reproduce corresponding signed works and endpoint stores through preparation, reference commutation and reset [OP-TRF-12]. Bounded active and nonideal driver models, dissipative event certificates and conditional preparation limits are established model results. Unmeasured converter and sensor costs, wider connection laws and unrestricted state/port correspondence retain their separate scope. Section \ref{sec:reference} derives the causal compound driver and a fixed-resistance obstruction to an instantaneous reference change, alongside the $1/5\ \mathrm J$ prescribed-cell control.

# Boundaries, ports and exact work
\label{sec:ledger}

For each system let $x$ contain its independent physical states. Its constitutive store $E(x)$ is evaluated at both ends of the declared interval. A port has effort $e_\ell$ and conjugate flow $f_\ell$, with positive product into that boundary. The definitions are
\begin{equation}
 W_\ell(t_0,t_1)=\int_{t_0}^{t_1}e_\ell(t)f_\ell(t)\,\dd t,
 \qquad r_E=E(x(t_1))-E(x(t_0))-\sum_\ell W_\ell.
 \label{eq:ledger}
\end{equation}
Electrical ports use $vi$, mechanical ports use $Fv$ or $\tau\omega$. A thermal export uses $-T_b\dot S_{\rm out}$, where $T_b$ is the boundary temperature and $\dot S_{\rm out}$ is entropy carried outward by heat, excluding internal entropy production. Acoustic export is $-\int p v_n\,\dd A$ with outward normal velocity $v_n$. A resistor outside the stored subsystem contributes $-v(v/R)$, and a damper contributes $-(dv)v$. These are separate integrals, even when their sum has a simpler expression. Whenever a resistor is included physically but only reactive storage is retained, its thermal storage is explicitly neglected; otherwise electrical dissipation first changes its thermal state and need not equal immediate exterior heat flow.

At a connection event, $x(t_e^-)$ and $x(t_e^+)$ belong to different vector fields or constraints. A finite interval resolving the event determines each work. A singular work is the limit of those integrals if it exists. Deleting a constitutive store and writing an event term equal to its negative closes a mathematical ledger, but supplies no effort, flow or physical recipient. That term must remain distinguished from a measured transfer.

For a finite mass, $m\dot v=F$ gives $\int Fv\,\dd t=m[(v^+)^2-(v^-)^2]/2$ by integrating the product. This equals $J(v^-+v^+)/2$ when $J=m(v^+-v^-)$; it does not define a product of an unspecified delta force with a discontinuous velocity. A fixed support can exchange momentum while its work is zero. A moving support needs its own force--velocity integral.

All integrations below are exact, so the numerical integration residual is exactly zero. A closed ideal ledger has $r_E=0$ by direct substitution after the separate integrals. The physical model residual $r_{\rm model}$ includes omitted material memory, switch-control supply, heat storage, exterior fields or release destinations, as named for each construction. Its sign and magnitude remain unevaluated unless a declared additional law determines them. This use of storage and supplied work is consistent with [Willems (1972)][willems]; the physical ports and stores still have to be identified for each realization.

Figure \ref{fig:boundaries} separates the observed port from hidden states and event transfers.

![Schematic of an observed physical system. The terminal trace constrains a projection of the state. Separate preparation, release and internal-observation paths remain necessary.](figures/boundaries.pdf){#fig:boundaries width=100%}

\FloatBarrier

# Damped correspondence through preparation and reset
\label{sec:analogy}

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

The distinction between these collision endpoints for a linear dashpot is developed by [Schwager and Pöschel (2007)][schwager]. That constitutive distinction determines restitution within the selected law; it does not identify a physical recipient for an omitted elastic state.

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

The truncated event description with continuous body velocities and no assigned event port has the explicit signed deficit
\begin{equation}
 r_{E,\rm unassigned}=-U_-=-e^{-\pi}\ \mathrm J
 \quad\hbox{in configuration I}.
 \label{eq:contact-deficit}
\end{equation}
Entering $W_{\rm deletion}=-U_-$ makes its formal residual zero. The physical destination remains open because that entry has no independently specified effort and flow. For a finite release window with unchanged body kinetic energy, retained elastic store $U_{\rm ret}(T_r)$ and outward receiver works $Q_j=\int_0^{T_r}e_jf_j\dd t$, the measured test instead uses
\begin{equation}
 r_{E,\rm release}=U_{\rm ret}(T_r)-U_-+\sum_jQ_j.
 \label{eq:release-residual}
\end{equation}
Any changed body, fixture or thermal store and any actual drive work enter separately. A signed remainder survives the comparison until a measured transfer or retained state accounts for it; destination fractions are not fitted to force it to zero.

For a candidate finite unloading path, let the isolated elastic coordinate fall as $z=z_-(1-s/\epsilon)$, $0\leq s\leq\epsilon$. Its outward elastic effort--flow product is $(kz)(-\dot z)$, and direct integration gives $kz_-^2/2=U_-$. A physical receiver attached to that coordinate still requires a specified coupling. Four exclusive destination hypotheses assign this whole transfer to fracture work $\int F_f\dot\ell\,\dd t$, acoustic work $\iint p v_n\,\dd A\dd t$, thermal transfer $\int T\dot S_{\rm out}\,\dd t$, or fixture work $\int F_bv_b\,\dd t$. They predict the four vectors
\begin{equation}
 (U_-,0,0,0),\quad(0,U_-,0,0),\quad
 (0,0,U_-,0),\quad(0,0,0,U_-)
 \label{eq:destination-vectors}
\end{equation}
in that ordered list of outward channels. Under a complete-transfer hypothesis, independently identified mixed fractions sum to one. Measured channel works are retained without normalization: an excess or deficit tests that hypothesis. These exclusive hypotheses are compared separately, never summed as four simultaneous releases.

Synchronized force and motion locate the event and fix $\delta_-,\dot\delta_-$. Contact strain checks $U_-$ under an identified stiffness. Calibrated acoustic intensity, temperature or calorimetric energy, fracture deformation and moving-support work then distinguish \eqref{eq:destination-vectors}. A microphone voltage alone does not determine acoustic energy; temperature alone does not determine heat without heat capacity and boundary flow. A perfectly fixed fixture predicts zero fixture work, so a nonzero fixture destination requires measured compliance or another moving support state.

There is also a retained-state alternative. Assume detachment transfers $\delta_-$ to an unloaded internal material coordinate $z(0)=\delta_-$, independent of subsequent body separation. Its massless spring and dashpot obey $d_r\dot z+kz=0$, $d_r>0$, with zero resultant traction on the detached bodies. This mapping and the separation of material strain from geometric overlap are additional constitutive assumptions. For elapsed time $s$ after detachment,
\begin{equation}
 z(s)=\delta_-e^{-ks/d_r},\quad U(s)=U_-e^{-2ks/d_r},\quad
 W_{d_r}(0,T_r)=-U_-(1-e^{-2kT_r/d_r}).
 \label{eq:retained-contact}
\end{equation}
The last result integrates the actual product $-(d_r\dot z)\dot z$. No store is deleted from the enlarged material boundary. If the dashpot is outside the elastic subboundary, this is its outward work; if the dashpot's thermal state is inside the material boundary, the same transfer is internal heating and exterior heat needs a separate integral.

For configuration I with $d_r=d=2\ \mathrm{N\,s/m}$ and $T_r=\log2\ \mathrm s$, the residual strain is $e^{-\pi/2}/2\ \mathrm m$, the retained store is $e^{-\pi}/4\ \mathrm J$, and the dashpot receives $3e^{-\pi}/4\ \mathrm J$. A prompt-transfer hypothesis completed before $T_r$ instead predicts zero residual elastic store and receiver transfer $e^{-\pi}\ \mathrm J$. Contact strain and receiver energy over that same window separate these conditional predictions. The four pure vectors in \eqref{eq:destination-vectors} describe prompt limiting destinations; they are not a complete list of material continuations. Energy first transferred to fracture or fixture motion and later converted to heat is counted at each subboundary separately, then canceled internally, rather than counted twice as export from one boundary.

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

The recurrence also assumes a compatible fresh contact state. Under \eqref{eq:retained-contact}, a finite flight leaves residual $z$ and possibly stored heat; neither is exactly reset by waiting a finite time. Reuse of the same material region must transport those states through a specified re-engagement law, or include a measured active reset. The third constant-law impact is therefore a continuation control. Friction, adhesion and plasticity remain separate constitutive identification tasks until their own laws predict distinct observations.

Flight duration already separates two specified continuations before the next contact. If the detached coordinate relaxes throughout a flight of duration $T_f$, independently measured strain and stiffness predict
\begin{equation}
 z_{\rm next}=\delta_-e^{-kT_f/d_r},\qquad
 U_{\rm next}=U_-e^{-2kT_f/d_r},\qquad
 Q_{d_r}=U_-(1-e^{-2kT_f/d_r}).
 \label{eq:contact-memory}
\end{equation}
The last quantity integrates $d_r\dot z^2$ over that flight. Prompt completion before re-engagement predicts zero residual elastic store and receiver work $U_-$. For I with $d_r=2\ \mathrm{N\,s/m}$ and $T_f=\log2\ \mathrm s$, the store predictions differ by $e^{-\pi}/4\ \mathrm J$; equal combined half-widths below $e^{-\pi}/8\ \mathrm J$ separate them. Changing flight duration requires measuring its drive work as in the preceding flight calculation. Predicting the next restitution additionally requires the constitutive map from $z_{\rm next}$ to the new contact deformation and force.

## A finite material comparison beyond fresh-state recurrence

A tangential control isolates one wider transfer. A slider of mass $m_s$ has prescribed constant speed $v_t>0$ on $[0,T_s]$, normal load $N>0$ and fixed normal position. Compare zero tangential coupling with the stated sliding law $F_t=-\mu N$, $\mu>0$. Force balance determines the required drive $F_d=\mu N$. The kinetic boundary has separate powers $F_dv_t$ and $F_tv_t$; the normal port has zero flow. Direct integration gives
\begin{equation}
 W_d=\mu Nv_tT_s=\mu Ns_t,\qquad
 W_t=-\mu Ns_t,\qquad
 E_s(0)=E_s(T_s)=\tfrac12m_sv_t^2,
 \label{eq:sliding-control}
\end{equation}
where $s_t=v_tT_s$. The equality of endpoint stores is evaluated from the prescribed motion. For $m_s=1\ \mathrm{kg}$, $v_t=1/5\ \mathrm{m/s}$, $N=2\ \mathrm N$, $\mu=1/4$ and $T_s=1\ \mathrm s$, the works are $+1/10$ and $-1/10\ \mathrm J$, with store $1/50\ \mathrm J$ at both ends. The zero-coupling control has the same speed and stores but both works vanish. Preparation to that speed belongs to an earlier interval. Equal work half-widths below $1/20\ \mathrm J$ separate these conditional predictions. If the contact's thermal store is retained, $-W_t$ enters it before exterior heat is separately measured.

| Constitutive extension | Finite comparison and missing relation |
|:----------------------------|:-----------------------------------------------------------|
| Plasticity | Fix incident state and contact geometry; measure permanent deformation and its force history to identify the irreversible deformation law and retained store. |
| Adhesion | Compare a prescribed finite opening at fixed material condition; identify tensile force versus separation and its signed work. |
| Motor ripple | Hold the declared flight endpoints; compare synchronized drive torque and rate with the constant-acceleration work before attributing changed incident speed to contact memory. |
| Acoustic and thermal memory | Compare two flight durations at the same release state; retain material/fixture endpoints and integrate calibrated receiver channels on both windows. |
| Further engagements and geometry | Carry the measured strain and thermal state into a third contact, then change one gap, area or damping parameter while measuring the resulting contact law. |

: Separate finite dependencies for the wider repeated-contact question. The sliding law and retained-strain law provide explicit controls; the other relations must be identified before their work predictions are assigned.

The open release question is which constitutive gate and continuation reproduce the measured restitution, retained strain and receiver works at each engagement. A measured release residual from \eqref{eq:release-residual} remains signed and unresolved when those channels and their uncertainty do not account for it.

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

For a declared voltage ceiling $V_{\max}$, the bounded apparatus family instead satisfies
\begin{equation}
 E_\epsilon(0)\leq\tfrac12\epsilon C_*V_{\max}^2\longrightarrow0,
 \qquad \epsilon\geq(V_*/V_{\max})^2
 \quad\hbox{for the fixed-energy preparation.}
 \label{eq:capacitor-rating}
\end{equation}
These are different domains: with the illustrative ceiling $V_{\max}=4\ \mathrm V$, configuration VII's fixed-energy family has $\epsilon\geq1/4$. Its formal limit proves a model distinction, while a finite experiment compares admissible members. Current, power and preparation limits impose additional independent restrictions.

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

A conductance ceiling $g_{\max}$ restricts these rectangular profiles to $\epsilon\geq2KC_e/g_{\max}$. For VIII with the illustrative $g_{\max}=1\ \mathrm S$, this is $\epsilon\geq\log2/1000\ \mathrm s$. A branch-current ceiling adds its own restriction through $i_j=g_jd$. Fixed integrated action at arbitrarily short duration is a formal family, distinct from these finite instrumentable members.

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

The two secondary subboundary products also integrate separately: $\int_0^T v_Ci_2\,\dd t=-1/1500\ \mathrm J$ enters the winding terminals, and $\int_0^T v_C(-i_2)\,\dd t=1/1500\ \mathrm J$ enters the capacitor. These cancel when the magnetic and capacitor boundaries are combined; neither is added to the external clamp work again.

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

In particular, a path reaching the first voltage maximum requires $C_p\geq L_eI^2/V_{\max}^2$ under a fixed ceiling $V_{\max}$. This exact bound follows from the amplitude in \eqref{eq:parasitic}; it neither selects the subsequent clamp law nor extends the accessible family to zero capacitance.

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
The boundary contains both magnetic stores including the mutual term, $C_ov_o^2/2$, and the resistors with thermal storage neglected and heat exported. Its external powers are separately $ui_s$, $-R_si_s^2$, $-R_1i_1^2$, $-R_2i_2^2$, $-G_cv_a^2$, $-G_\ell v_o^2$ and $-G_pv_o^2$. Their sum equals the store derivative by substitution of the circuit equations. Appendix \ref{sec:matrix} supplies an exact independent integral for each quadratic power on a constant-connection interval. A finite resistor heat capacity would add a thermal state and separate the dissipation from exterior heat flow.

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

## A complete finite return commutation
\label{sec:commutation}

Figure \ref{fig:commutation} specifies one complete tapped winding connection. Winding 1 runs from A to ground O with current $i_1$; winding 2 runs from B to A with current $i_2$. The inductance matrix is the positive-definite $\mathsf L$ already defined. A capacitor $C_o$ and load $G_o$ connect B to a return node R, with voltage $w=V_B-V_R$. Return conductances $g_A$ and $g_B$ connect R to A and O, respectively. A source $u$ drives A through $R_s$; a finite shunt $G_k$ from A to O is a resistive clamp path. Winding resistances are $R_1,R_2$. There is no core-loss branch in this construction.

![Schematic of the complete return commutation. The two winding sections remain connected and magnetically coupled throughout. The old return is A and the new return is O; their finite conductances overlap. The resistive clamp has its own measured power.](figures/transformer-commutation.pdf){#fig:commutation width=100%}

\FloatBarrier

For $g_\Sigma=g_A+g_B>0$, put $\lambda=g_A/g_\Sigma$, $\mu=1-\lambda$ and $g_e=g_Ag_B/g_\Sigma$. KCL at B and R and at the driven node A gives
\begin{align}
 v_a&=\frac{u-R_s(i_1-\mu i_2)}{1+R_s(G_k+g_e)},&
 v_r&=\lambda v_a-i_2/g_\Sigma,& i_s&=(u-v_a)/R_s,\nonumber\\
 \mathsf L\binom{\dot i_1}{\dot i_2}
 &=\binom{v_a-R_1i_1}{w-\mu v_a-(R_2+1/g_\Sigma)i_2},&
 C_o\dot w&=-i_2-G_ow.
 \label{eq:commutation-state}
\end{align}
For example, the old-return current from A to R is $g_A(v_a-v_r)$ and the new-return current from R to O is $g_Bv_r$. These oriented branches fix the port signs without inferring them from a balance.

Configuration XII uses $L_1=L_2=1/10\ \mathrm H$, $M=1/20\ \mathrm H$, $R_1=R_2=1/10\ \Omega$, $R_s=1\ \Omega$, $C_o=1/100\ \mathrm F$, $G_o=1/10\ \mathrm S$, $G_k=1/2\ \mathrm S$ and $u=1\ \mathrm V$. Three consecutive intervals each last $h=1/100\ \mathrm s$: old return $(g_A,g_B)=(2,0)$, overlap $(2,2)$, and new return $(0,2)$ in siemens. Initially $(i_1,i_2,w)=(1/10\ \mathrm A,1/20\ \mathrm A,1\ \mathrm V)$. Both winding currents and the capacitor voltage are continuous at the phase changes. The piecewise constant conductance law idealizes the gate edges but imposes no winding-current interruption or reactive-state reset. Actual edge storage and gate-supply consumption are separate physical costs.

Use SI numerical state coordinates $z=(i_1,i_2,w,1)^T$. Equation \eqref{eq:commutation-state} gives $z'=G_jz$, with the following exact matrices for the old, overlap and new intervals:
\begin{equation}
\begin{aligned}
G_0&=\begin{pmatrix}-92/9&4&-20/3&80/9\\46/9&-8&40/3&-40/9\\0&-100&-10&0\\0&0&0&0\end{pmatrix},\\[3pt]
G_1&=\begin{pmatrix}-8&17/3&-20/3&20/3\\6&-22/3&40/3&-16/3\\0&-100&-10&0\\0&0&0&0\end{pmatrix},\\[3pt]
G_2&=\begin{pmatrix}-44/3&52/3&-20/3&40/3\\14&-64/3&40/3&-40/3\\0&-100&-10&0\\0&0&0&0\end{pmatrix}.
\end{aligned}
\label{eq:commutation-matrices}
\end{equation}
Thus $z_0=(1/10,1/20,1,1)^T$, $z_{j+1}=e^{hG_j}z_j$ and $z_3=e^{hG_2}e^{hG_1}e^{hG_0}z_0$ specify every endpoint in closed form. Nonzero prepared energy is retained: with
$S=\operatorname{diag}(\mathsf L/2,C_o/2,0)$ understood in block form, $E_j=z_j^TSz_j$ and $E_0=47/8000\ \mathrm J$.

Every transfer can also be specified without an unevaluated quadrature. Let $e_1,e_2,e_3,e_4$ denote the coordinate vectors. Write $v_a=a_j^Tz$, $v_r=r_j^Tz$, $i_s=s_j^Tz$, where
\begin{equation}
 a_j=\frac{(-1,\mu_j,0,1)^T}{3/2+g_{e,j}},\quad
 r_j=\lambda_ja_j-e_2/g_{\Sigma,j},\quad s_j=e_4-a_j.
 \label{eq:commutation-ports}
\end{equation}
The eight individual inward powers and their symmetric matrices $H$ are

| Port | Power | Matrix $H$ in $P=z^THz$ |
|:-------------------|:----------------------|:--------------------------------------|
| Source | $ui_s$ | $(e_4s_j^T+s_je_4^T)/2$ |
| Source resistance | $-R_si_s^2$ | $-s_js_j^T$ |
| Winding 1 | $-R_1i_1^2$ | $-e_1e_1^T/10$ |
| Winding 2 | $-R_2i_2^2$ | $-e_2e_2^T/10$ |
| Resistive clamp | $-G_kv_a^2$ | $-a_ja_j^T/2$ |
| Load | $-G_ow^2$ | $-e_3e_3^T/10$ |
| Old-return channel | $-g_A(v_a-v_r)^2$ | $-g_A(a_j-r_j)(a_j-r_j)^T$ |
| New-return channel | $-g_Bv_r^2$ | $-g_Br_jr_j^T$ |

: The eight ports of configuration XII, in the SI coordinates of \eqref{eq:commutation-matrices}. Dissipative elements have no retained thermal store in this model.

Denote the exact expression in \eqref{eq:matrix-work} by $\mathcal W(G,H,z,T)$. The worked prediction for each named port, independently of every other port, is
\begin{equation}
 W_\ell=\sum_{j=0}^{2}\mathcal W(G_j,H_{\ell j},z_j,h),\qquad
 E_3-E_0=z_3^TSz_3-47/8000\ \mathrm J.
 \label{eq:commutation-work}
\end{equation}
These are exact matrix-function values at fully specified rational arguments. Direct multiplication gives $G_j^TS+SG_j=\sum_\ell H_{\ell j}$ for each phase, verifying zero residual after the separate integrals. The source and receiver paths are therefore determined by one connection and one prepared state, rather than by adding isolated subcircuit examples.

The comparison uses the same prepared state, $u=1\ \mathrm V$ and total duration $3h$: keep the old return for $h$, then the new return for $2h$. Its endpoints and independent works are
\begin{equation}
 \widetilde z=e^{2hG_2}z_1,\qquad
 \widetilde W_\ell=\mathcal W(G_0,H_{\ell0},z_0,h)
                  +\mathcal W(G_2,H_{\ell2},z_1,2h),
 \quad z_1=e^{hG_0}z_0.
 \label{eq:commutation-comparison}
\end{equation}
Write $\mathcal D_\ell=\mathcal W(G_1,H_{\ell1},z_1,h)+\mathcal W(G_2,H_{\ell2},z_2,h)-\mathcal W(G_2,H_{\ell2},z_1,2h)$. The common old-return interval cancels only after its work has been evaluated for each path. The differences below are exact values of matrix functions at the rational arguments in \eqref{eq:commutation-matrices}.

| Observable | Overlap path minus immediate new-return path |
|:-------------------------------|:---------------------------------------------------------|
| Old-return signed work | $\mathcal D_A=\mathcal W(G_1,H_{A1},z_1,h)=-\delta_A<0$ |
| New-return signed work | $\mathcal D_B$ |
| Resistive-clamp signed work | $\mathcal D_k$ |
| Source signed work | $\mathcal D_s$ |
| Final reactive store | $z_3^TSz_3-\widetilde z^TS\widetilde z=\sum_\ell\mathcal D_\ell$ |

: Complete-path work and endpoint differences on the common interval $[0,3h]$. The final equality follows after all eight separate works; the endpoint value is evaluated from the states.

The old-return work provides a strictly nonzero energy discriminant. In the overlap phase $v_a-v_r=l^Tz$, with $l^T=(-1/5,7/20,0,1/5)$ in the stated SI numerical coordinates. Hence
\begin{equation}
 \delta_A=2\int_0^h(l^Te^{G_1t}z_1)^2\dd t
 =-\mathcal W(G_1,-2ll^T,z_1,h)>0.
 \label{eq:overlap-separation}
\end{equation}
For a direct proof of the strict sign, the matrix obtained by stacking the covectors $l^T,l^TG_1,l^TG_1^2,l^TG_1^3$ has determinant $-4691046/25$. If the analytic integrand vanished throughout an interval, these four observations would give $z_1=0$, contradicting its constant coordinate one. The new-return comparison has $g_A=0$ after $h$, so no other old-return work can cancel this separation. Equal combined half-widths $B_A<\delta_A/2$ distinguish the two predictions. This budget uses the exact matrix-function value rather than a trajectory approximation.

The overlap conductance $g_e=1\ \mathrm S$, versus zero without overlap, supplies a separate topology check from synchronized $i_s,i_1,i_2,v_a$. The open physical question is which measured switch law reproduces these individual works, endpoint stores and any additional control-supply transfer. Both-returns-open operation requires another capacitive, clamp or arc path for nonzero $i_2$. Actual gate work and edge storage remain explicit additional ports and states in that experiment.

# A source-off transducer and a finite bias supply
\label{sec:transducer}

## Plant and controller are separate boundaries

The conditional construction below uses a plant with fixed coupling coefficients and a separate receiving bias coil. The wider open question concerns a finite realization whose actual bias current also changes the coupling, with independently resolved plant, controller, thermal and DC-link ledgers. A reciprocal electrical/mechanical transducer has current $i$, displacement $x$, velocity $v$ and three stored coordinates. The fixed-coupling controlled variant obeys
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

## A reciprocal actuator with finite electrical storage

Retain the plant force command, and implement it by an auxiliary reciprocal actuator whose inertia is neglected but whose winding storage and resistance are retained. Positive $u_ai_a$ enters its electrical terminals, while $F_av$ leaves it mechanically into the plant. With coupling $k_a>0$,
\begin{equation}
 F_a=k_ai_a,\qquad u_a=L_a\dot i_a+R_ai_a+k_av,\qquad
 E_a=\tfrac12L_ai_a^2.
 \label{eq:actuator-law}
\end{equation}
Its boundary has inward powers $u_ai_a$, $-F_av$ and $-R_ai_a^2$. Configuration X extends to $k_a=1\ \mathrm{N/A}=1\ \mathrm{V\,s/m}$, $L_a=1/100\ \mathrm H$ and $R_a=1/10\ \Omega$. Exact tracking of \eqref{eq:plant-path} requires
\begin{equation}
 i_a=-\frac3{20}e^{-10t}\ \mathrm A,\quad
 u_a=\frac1{10}e^{-10t}\ \mathrm V,\quad
 P_e:=-u_ai_a=P_r.
 \label{eq:actuator-path}
\end{equation}
The last equality holds here because $L_a\dot i_a+R_ai_a=0$ on this prepared trajectory; it is not a general identity between electrical export and mechanical reaction. Independent integration on $[0,T]$ gives electrical work $-9/16000\ \mathrm J$, mechanical reaction $+9/16000\ \mathrm J$, and copper work $-27/320000\ \mathrm J$. The independently evaluated winding stores are $E_a(0)=9/80000\ \mathrm J$ and $E_a(T)=9/320000\ \mathrm J$. Their decrease supplies the copper loss in this particular path.

Preparation must include $i_a(0)$ as well as the plant states. Any prescribed differentiable preparation $i_a,x$ fixes its terminal voltage through \eqref{eq:actuator-law}; its separately integrated electrical and force--velocity work belongs to that earlier interval. The observation interval assumes a current regulator that realizes \eqref{eq:actuator-path}. Its tracking, switching storage and sensing cost are idealized by the stated terminal law and logic load, and require measurement in hardware.

## Regenerative and dissipative receiving paths

Assume, illustratively, that a converter routes a constant fraction $\eta=4/5$ of the actuator's electrical export $P_e$ into a bias-coil terminal and exports $(1-\eta)P_e$ as heat. Here $P_e=P_r$ by \eqref{eq:actuator-path}; with other actuator parameters the electrical export must be recomputed first. Let $L_b=1/10\ \mathrm H$, $R_b=1\ \Omega$, $i_b(0)=1/100\ \mathrm A$, and define positive coil voltage $u_b$ by $L_b\dot i_b+R_bi_b=u_b$, $u_bi_b=\eta P_e$. This terminal conversion law has an illustrative efficiency; physical tracking and bandwidth remain to be measured.

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
Here the finite link loss follows from its port law $V_di_d=P_0$ and capacitor equation. The controller boundary now contains the actuator winding, bias coil and link. Its external input is mechanical reaction, its charger is off, and its exports are actuator copper, converter, bias-winding and logic heat. The actuator's electrical export and the converter input cancel only after their separate integrals. Combining plant and controller also cancels mechanical reaction. The independently evaluated combined endpoint change is
\begin{equation}
 \Delta(E_p+E_a+E_b+E_d)
 =-\frac{1641}{1600000}+\frac{\log2}{5000}\ \mathrm J.
 \label{eq:combined-actuator}
\end{equation}
It equals the six heat integrals: the two plant losses, actuator copper, converter loss, bias copper and logic. The ideal current regulator is included in the converter terminal law, with the stated $P_0$ as its assumed sensing/logic demand; any additional rail current or switching store must enlarge this ledger.

Figure \ref{fig:transducer} shows which transfers are internal only after the two ledgers are combined.

![Schematic of separate plant, controller and combined boundaries. The reaction port carries positive work into the controller on the source-off example; actuator, bias-coil and DC-link changes are independent endpoint observations.](figures/transducer-ledger.pdf){#fig:transducer width=100%}

\FloatBarrier

The dissipative alternative sends all $P_e$ to a dump element, with $\eta=0$ and the same actuator current and force. Then $i_b=e^{-10t}/100\ \mathrm A$ and $\Delta E_b=-3/800000\ \mathrm J$, while plant and actuator trajectories are identical. It predicts dump export $9/16000\ \mathrm J$; the regenerative path predicts converter export $9/80000\ \mathrm J$ plus the distinct coil heat in \eqref{eq:bias-work}. Actuator copper loss is the same in both. Bias-terminal voltage/current and both coil endpoints distinguish these paths even when the plant motion does not.

The sign can be predicted for every constant receiving efficiency $0\leq\eta\leq1$ under this same law. Substituting $u_bi_b=\eta P_e$ gives
\begin{equation}
 (i_b^2)'+20i_b^2=\frac{3\eta}{10}e^{-20t},\quad
 i_b^2=e^{-20t}\left(\frac1{10000}+\frac{3\eta}{10}t\right),\quad
 \Delta E_b=\frac{3\eta\log2}{8000}-\frac3{800000}\ \mathrm J.
 \label{eq:bias-efficiency}
\end{equation}
The coil input is independently $W_b=\int_0^T u_bi_b\dd t=9\eta/16000\ \mathrm J$. Its copper work, independently integrating $-i_b^2$, is $-3/800000+3\eta\log2/8000-9\eta/16000\ \mathrm J$. Converter heat is $-(1-\eta)9/16000\ \mathrm J$. Evaluating the two coil endpoints gives a positive change precisely when $\eta>1/(100\log2)$. Both endpoint substitution and the separate integrals reduce to \eqref{eq:bias-gain} at $\eta=4/5$. The actual electrical export, receiver power and auxiliary supply demands must be observed before applying this conditional threshold.

The derived observation ranges are within $\pm6\ \mathrm V$ including the DC link, $\pm1/5\ \mathrm A$, $\pm1/5\ \mathrm N$, $\pm1/50\ \mathrm m$ and $\pm1/5\ \mathrm{m/s}$ on a window shorter than $1/10\ \mathrm s$. Amplitudes alone do not establish control response. Differentiation gives $u_b'(0)=-1452\ \mathrm{V/s}$ and $i_b'(0)=119/10\ \mathrm{A/s}$; these are the maximum absolute slews on this interval. The affine factor under the square root changes by its initial value in $1/2400\ \mathrm s$. Actuator requirements are $|\dot i_a|\leq3/2\ \mathrm{A/s}$ and $|\dot u_a|\leq1\ \mathrm{V/s}$. These exact values set finite response requirements for a candidate regulator and synchronized probes. Tracking error is assessed from measured force and current, not from the force command. Section \ref{sec:uncertainty} bounds its effect on signed work.

Physical efficiency, sensor/logic power, saturation and switching bandwidth remain unmeasured. Thermal observations require identified heat capacities or calorimetric boundaries; repeated preparations add their own work if repetition increases the signal. If $g_e,g_m$ depend on changing $i_b$, their dynamics must be retained and \eqref{eq:plant-path} must be checked in that enlarged model.

For the wider finite bias-dependent supply models, four accuracy questions remain unresolved: thermal endpoint convergence, agreement of independently evaluated signed-power quadratures, interval energy residuals, and integrated DC-link subledgers. These limitations include stable finite paths as well as growing finite windows. A complete-interval combined balance or an exact coil identity does not settle the separate interval and link checks. The present closed forms have zero numerical integration residual; their exactness supplies no convergence result for those different models.

The physical question is whether independently measured reaction, actuator electrical export, bias power and finite-supply changes reproduce the positive coil change with all subboundaries resolved. A signed remainder beyond calibrated uncertainty remains an open result alongside the observed coil increase.

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

## A causal compound reference and its supply

For several coaxial inertias $J_j$ with elastic potentials depending only on relative angles, let $\omega_j$ be their rates and $\tau_j$ the external shaft torques. Pairwise internal spring forces follow from their constitutive laws; pairwise damping is $d_{jk}(\omega_j-\omega_k)$. Summing the individual equations after multiplying by $\omega_j-\Omega$ combines the spring powers into $\dot U$ and retains the damping products as signed losses, giving
\begin{equation}
 \dot E_\Omega=\sum_j\tau_j(\omega_j-\Omega)
 -\dot\Omega\sum_jJ_j(\omega_j-\Omega)
 -\sum_{j<k}d_{jk}(\omega_j-\omega_k)^2,
 \label{eq:compound-frame}
\end{equation}
where $E_\Omega=\sum_jJ_j(\omega_j-\Omega)^2/2+U$. The sum here explicitly assumes only those internal potentials. A spring grounded to a moving frame introduces the corresponding base-displacement dependence and its support work. Constraints must be imposed on the equations and their allowed velocities before multiplying by flows.

When $\Omega$ is the rate of a carrier inside the compound system, coupled forces determine its acceleration. The following active construction retains that causal dependency. Let $C$ be a positive diagonal matrix of node capacitances, $L$ a symmetric positive-definite winding matrix, $R$ a diagonal nonnegative resistance matrix and $B$ an incidence matrix with $B^T\mathbf1=0$. All node capacitors connect to a physical return R at voltage $r$. Their voltages are $w$, winding currents are $i$, and absolute node voltages are $v=w+r\mathbf1$. Separate floating actuators supply node currents $I(v,i,t)$ and compensation currents $-C\mathbf1\dot r$ from R. KCL and winding laws give
\begin{equation}
 C\dot w=I(v,i,t)-Bi-C\mathbf1\dot r,\qquad
 L\dot i=B^Tw-Ri.
 \label{eq:compound-circuit}
\end{equation}
Hence $C\dot v=I(v,i,t)-Bi$ and $L\dot i=B^Tv-Ri$. To follow a selected node $h$ through a differentiable reference command $\sigma(t)$, use
\begin{equation}
 \dot r=\dot\sigma v_h+\sigma[C^{-1}(I-Bi)]_h,
 \qquad r(0)=\sigma(0)v_h(0).
 \label{eq:compound-feedback}
\end{equation}
Then $r=\sigma v_h$ exactly. The right-hand side uses the current state and commanded currents, rather than a prerecorded trajectory or a differentiated noisy observation. Existence of the stated state evolution requires the chosen current laws to be well posed.

The mechanical counterpart can be defined independently with rates $\omega=v/\alpha$, inertia matrix $J=\alpha^2C$, modal elastic coordinates $\xi=Li/\alpha$, stiffness $K=\alpha^2L^{-1}$ and external torques $\tau=\alpha I$. Its laws are $J\dot\omega=\tau-BK\xi$ and $\dot\xi=B^T\omega-(R/\alpha^2)K\xi$. A nonzero winding resistance thus corresponds here to a series viscous relaxation of the modal elastic coordinate. These are declared element laws, distinct from assuming energy constancy. They give $r/\alpha=\Omega=\sigma\omega_h$ and stores
$E_\Omega=\tfrac12(\omega-\Omega\mathbf1)^TJ(\omega-\Omega\mathbf1)+\xi^TK\xi/2=w^TCw/2+i^TLi/2$.

The receiver ports are separately $w_jI_j$, $-C_jw_j\dot r$ and $-R_ki_k^2$. The first two correspond to $\tau_j(\omega_j-\Omega)$ and $-J_j(\omega_j-\Omega)\dot\Omega$. Their individual integrals precede cancellation of internal winding/capacitor powers. The complete floating network draws zero net current at the return-driver output, by KCL. The driver still has $I_d=C_d\dot r$, $u_d=r+R_dI_d$, store $C_dr^2/2$, source power $u_dI_d$ and resistor power $-R_dI_d^2$.

Supply each floating actuator and the driver command through an ideal bidirectional converter from a finite capacitor rail $C_s$ at voltage $V_s>0$. If $P_j$ is a converter's signed output power, its constitutive ideal law is input current $P_j/V_s$. Include a controller shunt $G_q$ with power $G_qV_s^2$. Rail KCL, with $q_s=V_s^2$, gives the exact solution
\begin{equation}
 q_s(t)=e^{-\kappa t}\left[q_s(0)-\frac2{C_s}
 \int_0^t e^{\kappa s}\sum_jP_j(s)\,\dd s\right],
 \quad \kappa=2G_q/C_s.
 \label{eq:compound-rail}
\end{equation}
Every rail work is independently $-\int P_j\dd t$ or $-\int G_qq_s\dd t$; its endpoint store is $C_sq_s/2$. The construction is admissible only while $q_s>0$. For affine fixed-connection state laws and polynomial reference commands, the powers are finite polynomial--exponential expressions, integrable by \eqref{eq:matrix-work} with finite generating states. This settles the active compound state map under ideal conversion assumptions. Real converter efficiency, control bandwidth and sensor costs require additional measured ports.

## A complete polynomial receiver control

Configuration XIII makes the compound statement explicit. In SI numerical coordinates on $0\leq t\leq1\ \mathrm s$, choose two capacitors $C_1=C_2=1/10\ \mathrm F$, one lossless winding $L=1/10\ \mathrm H$, $B=(1,-1)^T$, and define
\begin{equation}
 a(t)=2t-6t^2+4t^3,\quad A(t)=t^2(1-t)^2,\quad
 v=(a,0)^T,\quad i=10A,\quad r=v_1=a.
 \label{eq:compound-polynomial}
\end{equation}
Here $A'=a$; the indicated voltage and current units attach to their numerical expressions. Winding KVL gives $\dot i=10a$ and KCL fixes node commands $I_1=a'/10+i$, $I_2=-i$ before any work is calculated. Equation \eqref{eq:compound-feedback} with $\sigma=1,h=1$ generates the return. The relative capacitor voltages are $(0,-a)$ and compensation currents are $(-a'/10,-a'/10)$. Thus the two nonzero receiver powers are
$P_2=10aA$ at node 2 and $P_{\Omega2}=aa'/10$ at its compensation source; both node-1 powers vanish. Independently,
\begin{equation}
 W_2(0,t)=5A(t)^2,\qquad W_{\Omega2}(0,t)=a(t)^2/20,
 \quad E_{\rm rec}(t)=5A(t)^2+a(t)^2/20.
 \label{eq:compound-polynomial-work}
\end{equation}
Both endpoint stores and both full-interval works are zero. The node-2 works on the two half intervals are $+5/256$ and $-5/256\ \mathrm J$, so this is a nontrivial compound reversal with finite internal storage.

Receiver event coverage is exact in this family. Factoring $a,A,a'$ gives every power zero; equality of the two nonzero power magnitudes reduces to $a=0$ or $100A=\pm a'$. Substituting $y=t(1-t)$ reduces the latter equations to $100y^2=\pm(2-12y)$. Their admissible roots, together with all power zeros, give the complete partition
\begin{equation}
 \left\{0,\frac12,1,\frac{3-\sqrt3}{6},\frac{3+\sqrt3}{6},
 \frac12-\frac{\sqrt{31-2\sqrt{59}}}{10},
 \frac12+\frac{\sqrt{31-2\sqrt{59}}}{10}\right\}.
 \label{eq:compound-events}
\end{equation}
The equation $100y^2+2-12y=0$ has negative discriminant and no real root. Signs and the maximizing receiver-port magnitude are constant on each open complementary interval. The identically zero node-1 powers remain recorded; they add no omitted isolated roots. This certificate concerns these receiver powers, not every driver diagnostic or arbitrary dissipative trajectory.

Use XI's driver $C_d=1/200\ \mathrm F$, $R_d=3/4\ \Omega$, now with $u_d=a+3a'/800$, and a $C_s=1\ \mathrm F$ rail initially at $5\ \mathrm V$. Set $G_q=0$ and ideal converter efficiency one for this control. Direct integration gives
\begin{align}
 \mathcal J(t)&:=\int_0^t a'(s)^2\,\dd s
 =144t^5/5-72t^4+64t^3-24t^2+4t,\nonumber\\
 W_d(0,t)&=a(t)^2/400+3\mathcal J(t)/160000,\nonumber\\
 W_{R_d}(0,t)&=-3\mathcal J(t)/160000,\qquad
 q_s(t)=25-2\left[5A(t)^2+21a(t)^2/400+3\mathcal J(t)/160000\right].
 \label{eq:compound-driver-work}
\end{align}
The rail expression also follows directly from \eqref{eq:compound-rail}. Since $|a|\leq1/2$, $0\leq A\leq1/16$ and $0\leq\mathcal J\leq4/5$, the bracket is at most $26137/800000<1/20\ \mathrm J$ in the stated units; the rail stays positive. At $t=1$, the driver store returns to zero, its source supplies $3/200000\ \mathrm J$, its resistor exports the same amount, and the rail loses $3/200000\ \mathrm J$. The receiver's zero signed work has not eliminated the finite driver cost. Nonunit conversion and standby demand remain separately measurable additions.

## A dissipative control with complete event coverage

Dissipation also admits a complete exact certificate in a declared family. Extend XIII by setting its winding resistance to $R=1/10\ \Omega$, retaining $i=10A$, and commanding $v=(b,0)^T$, $r=b$, where $b=a+A$. Winding KVL gives $L\dot i=a=b-Ri$, and KCL fixes $I_1=b'/10+i$, $I_2=-i$. The receiver powers, derived from those laws, are
\begin{equation}
 P_2=10bA,\qquad P_{\Omega2}=bb'/10,\qquad P_R=-10A^2.
 \label{eq:dissipative-powers}
\end{equation}
Put $\mathcal K(t)=t^5/5-2t^6/3+6t^7/7-t^8/2+t^9/9$, so $\mathcal K'=A^2$ and $\mathcal K(0)=0$. The three independent integrals and constitutive store are
\begin{equation}
 W_2=5A^2+10\mathcal K,\quad
 W_{\Omega2}=b^2/20,\quad W_R=-10\mathcal K,\quad
 E_{\rm rec}=5A^2+b^2/20.
 \label{eq:dissipative-works}
\end{equation}
Both endpoint stores vanish on $[0,1]\ \mathrm s$, while the separately integrated works are $1/63$, $0$ and $-1/63\ \mathrm J$. These replace the lossless receiver's zero full-interval node work.

Every receiver power zero or equality of magnitudes belongs to the roots of
\begin{equation}
 A,\ b,\ b',\ 100A-b',\ 100A+b',\ a,\ a+2A,
 \quad bb'-100A^2,\ bb'+100A^2.
 \label{eq:dissipative-events}
\end{equation}
This follows by factoring each power and each pairwise sum and difference. For example $P_2\pm P_{\Omega2}=b(100A\pm b')/10$, and $P_2\pm P_R=10A(b\mp A)$. Node-1 powers remain identically zero. The table specifies the entire interior root set by exact rational isolating intervals; each indicated interval contains exactly one algebraic root.

| Polynomial | $V(0^+),V(1^-)$ | Interior root locations |
|:-----------------------------|:-------------------|:---------------------------------------------|
| $b$ | $1,0$ | $(56/100,57/100)$ |
| $b'$ | $2,0$ | $(24/100,25/100)$; $(81/100,82/100)$ |
| $100A-b'$ | $3,1$ | $(11/100,12/100)$; $(90/100,91/100)$ |
| $100A+b'$ | $2,2$ | none |
| $a$ | $1,0$ | $1/2$ exactly |
| $a+2A$ | $1,0$ | $(61/100,62/100)$ |
| $bb'-100A^2$ | $4,3$ | $(19/100,20/100)$ |
| $bb'+100A^2$ | $3,2$ | $(83/100,84/100)$ |

: Exact Sturm variation counts after removing endpoint factors. $A=t^2(1-t)^2$ adds only the endpoints $0,1$. The nine distinct interior roots and the two endpoints give the complete receiver partition.

For reproducibility, start with each endpoint-factor-free polynomial $p_0$, put $p_1=p_0'$, and recursively take $p_{j+1}=-\operatorname{rem}(p_{j-1},p_j)$. $V(q)$ counts sign changes after zero entries are omitted. Rational polynomial division gives the displayed endpoint variations and a decrease of one on each listed isolating interval. Each polynomial has constant greatest common divisor with its derivative, so its interior roots are simple. The intervals are disjoint; factors shared by different powers, and the double endpoint factors of $A$, remain explicit. Sturm's root count leaves no additional interior root; the root-count and isolation method is treated by [Basu, Pollack and Roy (2006)][basu]. Each sign and pairwise magnitude ordering is consequently fixed on every open complementary interval. Order the nine interior roots as $\tau_1<\cdots<\tau_9$, with $\tau_0=0$, $\tau_{10}=1$. On the ten open intervals, the maximizing port magnitudes occur in the order
\begin{equation}
 \Omega2,\ 2,\ 2,\ 2,\ R,\ R,\ 2,\ 2,\ 2,\ \Omega2.
 \label{eq:dissipative-maxima}
\end{equation}
The sign triples $(P_2,P_{\Omega2},P_R)$ are $(+,+,-)$ on the first three intervals, $(+,-,-)$ on the next two, $(-,+,-)$ on the next two, and $(-,-,-)$ on the last three. Exact rational evaluation between the disjoint root intervals establishes these orders; root completeness then extends each order throughout its interval. At $\tau_1,\tau_9$ the maximizing tie is $\{2,\Omega2\}$, at $\tau_4=1/2$ and $\tau_6$ it is $\{2,R\}$, at $\tau_5$ only $R$ maximizes, and at the remaining interior events only port 2 maximizes. All powers, including the identically zero node-1 powers, tie at the two endpoints. The other pairwise ties remain specified by \eqref{eq:dissipative-events}. This certificate covers this dissipative receiver's declared powers; a different driver or nonlinear family has its own event functions.

The same finite driver uses $u_d=b+3b'/800$, and the same ideal $1\ \mathrm F$, $5\ \mathrm V$ rail supplies every floating branch and the command. Independent integration of $b'^2=(a'+a)^2$ gives $\int_0^1b'^2\dd t=86/105$. Thus driver command and resistor works are $+43/2800000$ and $-43/2800000\ \mathrm J$, with zero driver stores at both endpoints. For a partial interval define the exact polynomial
\begin{equation}
 \mathcal J_b(t)=\frac{16t^7}{7}+8t^6-\frac{44t^5}{5}
                -26t^4+\frac{124t^3}{3}-20t^2+4t.
 \label{eq:dissipative-driver-integral}
\end{equation}
Differentiation gives $\mathcal J_b'=b'^2$, and $\mathcal J_b(0)=0$. The driver input is $b^2/400+3\mathcal J_b/160000$, while its resistor work is $-3\mathcal J_b/160000$. Rail KCL gives
\begin{equation}
 q_s(t)=25-2\left[5A^2+10\mathcal K+21b^2/400
                    +3\mathcal J_b/160000\right].
 \label{eq:dissipative-rail}
\end{equation}
Here $|b|\leq9/16$, $A\leq1/16$, $\mathcal K\leq1/630$ and $\int_0^t b'^2\dd s\leq86/105$. The bracket is at most $41957759/806400000<1/10\ \mathrm J$, so $q_s>124/5\ \mathrm{V^2}$. The rail endpoint loses $1/63+43/2800000\ \mathrm J$, equal to the two independently integrated heat exports. The receiver work, driver work and rail change remain distinct observables.

## Finite sensor, actuator and converter states

Finite response and loss also have explicit constitutive models. A supplied sensor buffer with input effort $\xi$, output capacitor voltage $z_s$, resistance $R_s^{\rm obs}>0$ and capacitance $C_s^{\rm obs}>0$ obeys $I_s^{\rm obs}=(\xi-z_s)/R_s^{\rm obs}$ and $C_s^{\rm obs}\dot z_s=I_s^{\rm obs}$. Its store is $C_s^{\rm obs}z_s^2/2$ and its separately signed powers are $\xi I_s^{\rm obs}$ and $-R_s^{\rm obs}(I_s^{\rm obs})^2$. Nonloading transduction from the observed quantity to $\xi$ is an additional assumption; physical probe loading requires its own port.

A floating current actuator with winding $L_a>0$, resistance $R_a\geq0$, supplied effort $e_a$ and receiver voltage $w_j$ obeys
\begin{equation}
 L_a\dot j=e_a-w_j-R_aj,\qquad
 e_a=w_j+R_aj+\frac{L_a}{\tau_a}(j_{\rm cmd}-j),
 \quad\tau_a>0,
 \label{eq:finite-reference-actuator}
\end{equation}
within its unsaturated voltage range. Its own store is $L_aj^2/2$, and its powers are $e_aj$, $-w_jj$ and $-R_aj^2$. The command can use sensed states; the displayed local feedback is a constitutive law with finite response $\dot j=(j_{\rm cmd}-j)/\tau_a$. A voltage limit changes the actual state law and must be retained at that event.

For a bidirectional converter, a stated efficiency $0<\eta_c\leq1$ specifies rail input $P_{\rm in}=P_{\rm out}/\eta_c$ for positive output and $P_{\rm in}=\eta_cP_{\rm out}$ for negative output. Its own three powers are $P_{\rm in}$, $-P_{\rm out}$ and $-(P_{\rm in}-P_{\rm out})$; they are integrated separately on both signs. The finite rail then uses these actual inputs in \eqref{eq:compound-rail}. Sensor, actuator, driver and rail endpoints belong to their own boundaries. Affine unsaturated commands on a fixed sign interval admit the exact matrix integrals of Appendix \ref{sec:matrix}. Nonlinear tracking, voltage limits and physical sensor/feedback costs require their separately specified laws and event coverage.

These constructions distinguish the existence of a finite nonideal model from identification of its hardware behavior. Bounded dissipative certificates and conditional preparation limits remain established mathematical results. The open physical question concerns correspondence of the actual signed works and stores when those finite driver and measurement effects are present.

## Constraint paths, rigid reduction and a reference-jump obstruction

An energized locking control shows the event issue exactly. Two otherwise free rotors connected by a finite viscous coupling $d$ have fixed total angular momentum and relative rate $\delta\omega(t)=\delta\omega_0e^{-dt/J_e}$, $J_e=J_1J_2/(J_1+J_2)$. Their external damping work is
\begin{equation}
 W_d=-\int_0^T d(\delta\omega)^2\dd t
 =-\frac{J_e(\delta\omega_0)^2}{2}(1-e^{-2dT/J_e}).
 \label{eq:locking}
\end{equation}
For $J_1=J_2=1\ \mathrm{kg\,m^2}$, initial rates $(1,0)\ \mathrm{rad/s}$ and $dT/J_e=\log2$, final rates are $(3/4,1/4)\ \mathrm{rad/s}$, initial kinetic store $1/2\ \mathrm J$, final store $5/16\ \mathrm J$, and $W_d=-3/16\ \mathrm J$. The exact locked limit instead has rates $(1/2,1/2)$ and store $1/4\ \mathrm J$. A lossless relative-motion receiver could retain the difference energy rather than heating it; that is a different finite path with an added state and transfer port. A compound lock or electrical clamp requires this choice to be made for every constraint, including its drive and reference paths.

A zero-net-work control also requires signed interval resolution. With configuration XI's $J$, zero reference acceleration and $\tau=J(1-2t)$ on $[0,1]\ \mathrm s$, the exact rate is $\omega=t-t^2$. Integrating $\tau\omega$ gives $+1/320\ \mathrm J$ on $[0,1/2]$ and $-1/320\ \mathrm J$ on $[1/2,1]$, with both endpoint stores zero. Under delivery efficiency $\eta_s$ and recovery efficiency $\eta_r$, a rail supporting these two signs has net work $(1/320)(1/\eta_s-\eta_r)\ \mathrm J$, before standby loss. Zero signed receiver work therefore does not determine zero rail work. This polynomial cell establishes all its power zeros directly; it does not establish root completeness for a coupled compound trajectory.

The finite active construction, locking path and polynomial event certificate are bounded results. A conditional rigid reduction can also be derived from constitutive equations. For a winding pair write $L=L_0\left(\begin{smallmatrix}h^2&kh\\kh&1\end{smallmatrix}\right)$, $R=R_0\operatorname{diag}(h^2,1)$, normalized currents $p=hi_1$, $q=i_2$, and modes $s=p+q$, $d=p-q$. Choose $L_0=\ell/\epsilon$, $k=1-\epsilon^2$, $R_0=r_0\epsilon^2$ and all node capacitances proportional to $\epsilon$, with $\ell,r_0,h>0$ and $0<\epsilon\leq1$. Matched constant winding drives $u_1/h=u_2=V$ and compatible $s(0)=0$, $d(0)=d_0$ give
\begin{equation}
 L_+=\ell(2-\epsilon^2)/\epsilon,\quad L_-=\ell\epsilon,\quad
 s(t)=\frac{2V}{R_0}(1-e^{-R_0t/L_+}),\quad
 d(t)=d_0e^{-R_0t/L_-}.
 \label{eq:rigid-family}
\end{equation}
The source and copper integrals are explicit. Put $a_+=R_0/L_+$, $a_-=R_0/L_-$, $b=2V/R_0$ and $F_T(a)=(1-e^{-aT})/a$, with $F_T(0)=T$. Integrating the two source products $u_1i_1=Vp$, $u_2i_2=Vq$ and the separate copper products gives
\begin{align}
 W_{1,2}&=\frac V2\{b[T-F_T(a_+)]\mathbin{\pm}d_0F_T(a_-)\},\nonumber\\
 W_{R,1,2}&=-\frac{R_0}{4}\{b^2[T-2F_T(a_+)+F_T(2a_+)]
 +d_0^2F_T(2a_-)\nonumber\\
 &\hspace{35mm}\mathbin{\pm}2bd_0[F_T(a_-)-F_T(a_++a_-)]\}.
 \label{eq:rigid-work}
\end{align}
Upper signs belong to winding 1. Initial and final magnetic stores are independently $(L_+s^2+L_-d^2)/4$ at the corresponding states, and substitution gives zero residual. On $0\leq t\leq T$, the exact inequality $0\leq1-e^{-x}\leq x$ gives $|s|\leq2|V|T/L_+$ and $|d-d_0|\leq|d_0|R_0T/L_-$. The common current and copper works therefore vanish in the limit, the differential current tends to $d_0$, and both the magnetic store and scaled capacitor stores at bounded voltage tend to zero. This matched-drive, compatible-state reduction does not assert convergence for arbitrary preparation: fixed nonzero $s(0)$ instead gives divergent magnetic energy. Exact singular constraints, such as the null-vector voltage condition at $\det L=0$, must be imposed before eliminating states.

A vanishing common current can instead retain finite prepared energy. Keep the same family and set $s(0)=s_0=c\sqrt\epsilon$ with a fixed nonzero current scale $c$. Direct state evaluation gives
\begin{equation}
 E_+(0)=\frac{L_+s_0^2}{4}
       =\frac{\ell c^2(2-\epsilon^2)}4
       \longrightarrow\frac{\ell c^2}{2}>0.
 \label{eq:finite-common-store}
\end{equation}
The exact transported state is $s(t)=b+(s_0-b)e^{-a_+t}$, with the same $d(t)$. Define the elementary integrals
\begin{align}
 J_s&=bT+(s_0-b)F_T(a_+),\nonumber\\
 J_{ss}&=b^2T+2b(s_0-b)F_T(a_+)+(s_0-b)^2F_T(2a_+),\nonumber\\
 J_{dd}&=d_0^2F_T(2a_-),\qquad
 J_{sd}=d_0\{bF_T(a_-)+(s_0-b)F_T(a_++a_-)\}.
 \label{eq:prepared-modal-integrals}
\end{align}
They integrate $s,s^2,d^2,sd$, respectively, as direct differentiation verifies. The separate source and copper works therefore become
\begin{equation}
 W_{1,2}=\frac V2\{J_s\mathbin{\pm}d_0F_T(a_-)\},\qquad
 W_{R,1,2}=-\frac{R_0}{4}\{J_{ss}+J_{dd}\mathbin{\pm}2J_{sd}\}.
 \label{eq:prepared-modal-work}
\end{equation}
Initial and final stores are still evaluated from $(L_+s^2+L_-d^2)/4$. At $s_0=0$ these formulas recover \eqref{eq:rigid-work}; no preparation term has been dropped.

For an explicit finite preparation with $d_0=0$, prescribe $s=s_0(t+T_p)/T_p$ on $[-T_p,0]$, with both winding currents initially zero. Their separately imposed voltages satisfy $u_1/h=u_2=(L_+\dot s+R_0s)/2$. Each source integral is $L_+s_0^2/8+R_0s_0^2T_p/12$, and each copper integral is $-R_0s_0^2T_p/12$. The independent final store is $L_+s_0^2/4$. At fixed preparation duration its maximum matched terminal effort is $(L_++R_0T_p)|s_0|/(2T_p)$. A fixed ceiling $V_{\max}$ therefore restricts the finite family; since $L_+\geq\ell/\epsilon$, the necessary bound is $\epsilon\geq[\ell|c|/(2T_pV_{\max})]^2$. Exact zero $\epsilon$ is a mathematical limit, while finite winding voltages and both preparation works define the apparatus comparison.

Configuration XIV sets $\ell=1/10\ \mathrm H$, $r_0=1\ \Omega$, $h=1$, $c=1/5\ \mathrm A$, $\epsilon=1/4$ and $T_p=1\ \mathrm s$. Thus $L_+=31/40\ \mathrm H$, $R_0=1/16\ \Omega$, $s_0=1/10\ \mathrm A$, and each preparation source supplies $49/48000\ \mathrm J$ while each copper channel exports $1/19200\ \mathrm J$. The winding store rises from zero to $31/16000\ \mathrm J$. Subsequently set both winding terminal voltages to zero, retaining their conductor paths, and observe for $T=62\log2/5\ \mathrm s$. Each source work is zero, each copper work is $-93/128000\ \mathrm J$, and the independently evaluated final store is $31/64000\ \mathrm J$. The source-off residual is zero after these separate integrals.

For the full $\epsilon$ family with $V=0$, a fixed observation time instead gives $E_+(T)=E_+(0)e^{-2a_+T}$ and $a_+\to0$. The finite store remains while current vanishes. A duration $T=(\log2)/a_+$ gives one quarter of that store and exports the other three quarters through the two identified resistances. Fixed duration and this varying duration are different physical paths. A reduced current limit alone determines neither preparation work nor remaining store. Correspondence must compare both, along with every retained signed port.

A physical reference jump has a separate obstruction. For a linear change $r_-\to r_+$ over $\delta>0$, the finite driver has constant $I_d=C_d\Delta r/\delta$ and separately integrated works
\begin{equation}
 W_{R_d}=-\frac{R_dC_d^2(\Delta r)^2}{\delta},\qquad
 W_d=\frac{C_d}{2}(r_+^2-r_-^2)
       +\frac{R_dC_d^2(\Delta r)^2}{\delta}.
 \label{eq:reference-jump}
\end{equation}
For any absolutely continuous transition with the same endpoints, Cauchy--Schwarz gives $\int_0^\delta R_dC_d^2\dot r^2\dd t\geq R_dC_d^2(\Delta r)^2/\delta$. At fixed positive $R_d,C_d$ and nonzero $\Delta r$, no finite-work instantaneous limit exists. For XI's driver, a $1\ \mathrm V$ change from zero in $1/100\ \mathrm s$ gives resistor work $-3/1600\ \mathrm J$, source work $7/1600\ \mathrm J$ and capacitor change $1/400\ \mathrm J$. These are finite predictions, not an instantaneous apparatus setting.

The remaining compound questions concern measured converter and sensor costs, wider connection laws and state/port correspondence outside the declared preparation and drive families. The dissipative certificate above is complete for its receiver; event completeness for another nonlinear driver or constitutive family is a separate mathematical task. Reference-driver and receiver supplies must be instrumented separately, with mechanical shaft torque and rate where correspondence is asserted. A measured work mismatch must retain its sign and boundary even when each device has a closed individual ledger; an unexplained energy remainder is additionally retained through \eqref{eq:measured-residual}.

# What terminal observations identify
\label{sec:identification}

The transfer questions above require identified states, component laws and uncertainty. These five inherited observation questions specify which internal quantities can be recovered and which remain inaccessible.

## Contact versus a compliant support

For hammer and anvil angles $\theta_h,\theta_a$, positive inertias $J_h,J_a$, contact torque $\tau_c=k_c(\theta_h-\theta_a)+d_c(\dot\theta_h-\dot\theta_a)$ and support torque $\tau_j=k_j\theta_a+d_j\dot\theta_a$, the equations are
\begin{equation}
 J_h\ddot\theta_h=u-\tau_c,\qquad
 J_a\ddot\theta_a=\tau_c-\tau_j.
 \label{eq:two-inertia}
\end{equation}
They give a generic fourth-order hammer equation. Rational frequency-domain relations below describe zero-state transfer, or steady sinusoidal response at $s=\ii\omega$; arbitrary preparations add initial-state terms. With $Z_c=k_c+d_cs$ and $Z_a=J_as^2+k_j+d_js$, elimination gives
\begin{equation}
 \frac{U}{\Theta_h}=J_hs^2+\frac{Z_cZ_a}{Z_c+Z_a},\qquad
 \frac{\Theta_a}{\Theta_h}=\frac{Z_c}{Z_c+Z_a}.
 \label{eq:contact-inference}
\end{equation}
The terminal observes a composite dynamic stiffness. If a broader rational support is allowed, different admissible decompositions of that composite must be distinguished before assigning internal coefficients. Positivity, a known inertial model and a sufficiently rich frequency domain can impose additional constraints; static ambiguity alone is not a theorem of ambiguity on every frequency domain.

With known $J_h$ and measured $Z_e=U/\Theta_h-J_hs^2$ and $H_a=\Theta_a/\Theta_h$, the same equations give a constructive inverse:
\begin{equation}
 Z_c=\frac{Z_e}{1-H_a},\qquad Z_a=\frac{Z_e}{H_a}.
 \label{eq:contact-inverse}
\end{equation}
Indeed $1-H_a=Z_a/(Z_c+Z_a)$, so substitution proves both expressions. They require defined responses and nonzero denominators; errors are amplified near $H_a=0$ or $1$. In the stated spring--damper family, a nonzero real frequency determines $k_c=\operatorname{Re}Z_c$, $d_c=\operatorname{Im}Z_c/\omega$, $k_j=\operatorname{Re}Z_a+J_a\omega^2$ and $d_j=\operatorname{Im}Z_a/\omega$ when $J_a$ is known. Additional frequencies check that family. Recovering the composite $Z_a$ does not identify an arbitrary internal support realization. The distinction between a realization and its observable input--output part is the one formalized by [Kalman (1963)][kalman].

The inverse has an exact uncertainty bound. Write $Z=Z_e$, $H=H_a$, with absolute errors at most $\epsilon_Z,\epsilon_H$. When $|H|>\epsilon_H$ and $|1-H|>\epsilon_H$, subtraction of the two rational inverses and the triangle inequality give
\begin{align}
 |\widehat Z_c-Z_c|&\leq
 \frac{\epsilon_Z|1-H|+|Z|\epsilon_H}
 {|1-H|(|1-H|-\epsilon_H)},\nonumber\\
 |\widehat Z_a-Z_a|&\leq
 \frac{\epsilon_Z|H|+|Z|\epsilon_H}
 {|H|(|H|-\epsilon_H)}.
 \label{eq:contact-inverse-error}
\end{align}
Indeed the two error numerators are $\delta Z(1-H)+Z\delta H$ and $\delta ZH-Z\delta H$. Lower bounds on the denominator magnitudes yield \eqref{eq:contact-inverse-error} without linearizing the errors. Calibrated magnitude envelopes replace unknown true values in an experiment. These bounds apply to the composite support; its internal realization still requires a specified family or further sensors.

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

The coordinates can be varied physically: choose $a=J_a$, $b=d_j$, $c=k_j$ and $\eta=d_c/d_j$. Holding $J_a=1\ \mathrm{kg\,m^2}$ and $d_j=1\ \mathrm{N\,m\,s/rad}$, configuration III's three settings require $(k_j,d_c)=(1,1),(1/4,1),(1,2)$ in their corresponding SI units. These knobs set the coordinates; the law \eqref{eq:weak-coefficient} remains a hypothesis about the inferred coefficient. For coefficient observations $b_1,b_2,b_3$ at the exact settings, matrix inversion yields
\begin{equation}
 w_1=-5b_1+4b_2+b_3,\qquad
 |\delta w_1|\leq5\epsilon_1+4\epsilon_2+\epsilon_3.
 \label{eq:coefficient-bound}
\end{equation}
Here $|\delta b_j|\leq\epsilon_j$. Equal candidate uncertainty intervals for $w_1=1/100$ and $0$ separate if the right-hand side is below $1/200$. With uncertain positive coordinates and positive candidate weights, the exact prediction interval has endpoints $w_0+w_1\eta_-+w_2\eta_-^2/\rho_+$ and $w_0+w_1\eta_++w_2\eta_+^2/\rho_-$. These component-calibration bounds enter before comparing coefficients; invertibility alone supplies no practical error bound.

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

The open acquisition requires calibrated multi-device complex impedance and independent shunt variation, with synchronized internal/terminal traces where an internal claim is made. Twelve resonators and three fixture/component variants define an illustrative finite scope, not a statistically derived sample size. Shunt subtraction identifies $Y-sC_0$ for each device. Transferability requires a separately specified law predicting its $L_m,R_m,C_m$ from independently controlled device properties, calibrated on one set and evaluated on other declared devices and frequencies. No such law follows from the shunt control alone. Fixture compensation and RF current/voltage definitions follow [Keysight Technologies (2026)][keysight]; temperature, aging and nonlinear behavior require their own domain.

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

A bounded positive statement follows directly: the split and equal-time predictions at a declared $t$ have disjoint voltage intervals of half-width $\epsilon_V$ if
\begin{equation}
 |a(e^{-t/\tau_1}-e^{-t/\tau_2})|>2\epsilon_V.
 \label{eq:polarization-separation}
\end{equation}
For the stated example, $\epsilon_V<(1/\sqrt2-1/2)/2\ \mathrm V$ suffices when parameters and preparation are exact. Their uncertainties widen the prediction intervals. Recovery of an unknown order requires, in addition, a maximum candidate order, a lower bound on visible amplitudes, separated active time constants and a specified observation/noise domain; the two-alternative result asserts none of these globally.

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

# Measurements that discriminate the retained alternatives
\label{sec:measurements}

The comparisons below give observables for every retained question. Their types distinguish an exact identity to validate, structural nonidentifiability, competing constitutive laws, physical transfer alternatives and acquisition of a missing law. An omitted port or a coordinate relabeling is an accounting control, not a second prepared physical apparatus. A comparison supports one declared law when its calibrated observations agree with that prediction, exclude the competing predictions and retain both endpoint states and actual event sides. Overlapping intervals leave the comparison unresolved. Disagreement with both laws retains the signed work and store differences while the constitutive law or boundary is investigated. A nonzero energy remainder is a separate outcome, quantified below.

## Exact bounds for work and endpoint uncertainty
\label{sec:uncertainty}

Let true effort and flow be $e,f$ and measurements be $e+\delta e,f+\delta f$, with deterministic bounds $|\delta e|\leq\epsilon_e(t)$ and $|\delta f|\leq\epsilon_f(t)$. Expanding their product and applying the triangle inequality gives, without a small-error approximation,
\begin{equation}
 |\widehat W-W|\leq\int_{t_0}^{t_1}
 \left(|e|\epsilon_f+|f|\epsilon_e+\epsilon_e\epsilon_f\right)\dd t
 =:\epsilon_W.
 \label{eq:work-uncertainty}
\end{equation}
Known amplitude envelopes can replace the unknown $|e|,|f|$ on the right. On a smooth interval with $|\dot f|\leq M_f$, a relative clock error $\epsilon_t$ adds at most $M_f\epsilon_t$ to the flow-error bound. At a jump, use separate event-side bounds and a bounded-power integral over the uncertain event-time window; a smooth derivative bound cannot cross an unspecified discontinuity. Any hardware integration error is an additional bound, whereas the closed-form predictions have exactly zero numerical integration residual.

For a capacitor, suppose $C\leq C_{\max}$, $|v|\leq V_{\max}$, and absolute component and voltage errors are at most $\epsilon_C,\epsilon_v$. Direct expansion of $Cv^2/2$ gives the endpoint bound
\begin{equation}
 |\widehat E-E|\leq\frac12\left[
 \epsilon_CV_{\max}^2+(C_{\max}+\epsilon_C)
 (2V_{\max}\epsilon_v+\epsilon_v^2)\right].
 \label{eq:endpoint-uncertainty}
\end{equation}
Inductors use the same expression with $L,i$; mutual stores require their full quadratic form. Known correlations can tighten interval bounds, but independence is not presumed. For independently evaluated measurements, define
\begin{equation}
 \widehat r_E=\widehat E(t_1)-\widehat E(t_0)-\sum_\ell\widehat W_\ell,
 \qquad B_E=B_{E_1}+B_{E_0}+\sum_\ell B_{W_\ell}.
 \label{eq:measured-residual}
\end{equation}
All works use the same explicit interval and their own signed effort--flow products. Acquisition and integration uncertainty enter the port bounds. The interval $[\widehat r_E-B_E,\widehat r_E+B_E]$ tests whether zero is compatible with that measured ledger. A wholly positive interval means more stored energy, or a smaller decrease, than the audited net input accounts for; a wholly negative interval means a deficit relative to that input. Preserve its magnitude, sign, preparation, event conditions and completed checks when it remains unexplained. An omitted mechanism with unknown magnitude stays named and unevaluated; it receives no post hoc allowance chosen to cover the remainder. A separately justified bound may be added only under its stated physical assumptions. Model disagreement with a residual compatible with zero remains a different result.

If predictions for an observable differ by $\Delta_y$, their intervals of half-widths $B_1,B_2$ are disjoint when $B_1+B_2<\Delta_y$. The following sufficient budgets use equal combined half-width $B_y$ and exact nominal parameters; parameter and model uncertainty must be included in that budget.

| Comparison | Observable separation $\Delta_y$ | Sufficient $B_y$ |
|:------------------------------------|:------------------------------------|:-----------------------------------|
| II contact/support | Anvil angle $1/6\ \mathrm{rad}$ | $<1/12\ \mathrm{rad}$ |
| III weak coefficient | $1/100$ | $<1/200$ |
| IV shunt control | Imaginary admittance $1\ \mathrm S$ | $<1/2\ \mathrm S$ |
| V hidden preparation | One branch voltage $1/2\ \mathrm V$ | $<1/4\ \mathrm V$ |
| VI absorber | Stress amplitude $1/2\ \mathrm{MPa}$ | $<1/4\ \mathrm{MPa}$ |
| I retained versus prompt release | Residual store $e^{-\pi}/4\ \mathrm J$ at $T_r$ | $<e^{-\pi}/8\ \mathrm J$ |
| VII prepared versus relaxed | Final store $1/2\ \mathrm{mJ}$ | $<1/4\ \mathrm{mJ}$ |
| VIII closest channel predictions | Work $9/32\ \mathrm{mJ}$ | $<9/64\ \mathrm{mJ}$ |
| IX two opening paths | Final capacitor voltage $1\ \mathrm V$ | $<1/2\ \mathrm V$ |
| X regenerative versus dump | Bias-store change $3\log2/10000\ \mathrm J$ | $<3\log2/20000\ \mathrm J$ |
| XI compensation on/off | Receiver store $1/5\ \mathrm J$ | $<1/10\ \mathrm J$ |
| XI two supply efficiencies | Compensation rail work $1/20\ \mathrm J$ | $<1/40\ \mathrm J$ |
| XII equal-duration paths | Old-return work $\delta_A>0$ from \eqref{eq:overlap-separation} | $<\delta_A/2$ |
| Tangential sliding control | Drive work $1/10\ \mathrm J$ | $<1/20\ \mathrm J$ |
| XIII lossless/dissipative extension | Full-interval node work $1/63\ \mathrm J$ | $<1/126\ \mathrm J$ |
| XIV prepared/relaxed winding | Final magnetic store $31/64000\ \mathrm J$ | $<31/128000\ \mathrm J$ |

: Exact design budgets for separating conditional predictions, not achieved instrument accuracies.

The release-law comparison instead uses restitution separation $\min(e_F-e_D,e_C-e_F)$ in configuration I; its combined half-width must be less than half that value. Pure prompt destinations differ by $U_-$ in at least one receiver channel. Matched-flight two-impact deletion versus zero differs by $e^{-\pi}+e^{-2\pi}\ \mathrm J$, conditional on fresh contact states. The LC controls differ by $E_0$ in capacitor energy, while canonical mutual-sign reversal differs by $2/15\ \mathrm A$ in $i_2$ at $t=\pi/200\ \mathrm s$. Each uses the same half-separation rule. Unknown wider material or arc laws have no assigned universal separation; their acquisition precedes an energy comparison.

Acoustic energy requires calibrated $\int\!\int p v_n\dd A\dd t$; calorimetry requires heat-flow or identified thermal-store endpoints; fracture work requires force and fracture displacement. All use a common observation interval that also retains unrelaxed material and fixture stores. A microphone voltage or temperature trace without that conversion cannot close an energy partition.

\Needspace{12\baselineskip}

## Release law, destination and continuation

| Release question and comparison type | What is held or changed | Predictions that separate the readings |
|:-------------------------------------|:-------------------------------------------|:-------------------------------------------|
| Destination; physical transfer alternatives | Hold I's incident state; observe strain and receiver energy through $T_r=\log2$ after detachment | Retained strain gives store $e^{-\pi}/4\ \mathrm J$ and dashpot transfer $3e^{-\pi}/4\ \mathrm J$; prompt completion gives zero residual store and transfer $e^{-\pi}\ \mathrm J$ |
| Separation criterion; constitutive laws | Hold $m,d,k,v_0$; resolve force, deformation and velocity through release | $(t,e)=(\pi/2,e^{-\pi/2})$, $(\pi,e^{-\pi})$, or $(\pi/4+\pi/(2\sqrt2),e^{-\pi/4})$ |
| Repeated restitution/destination; conditional laws | Observe incoming states, receiver work, residual strain/heat and signed flight drive | Fresh-state force-zero deletion totals $e^{-\pi}+e^{-2\pi}\ \mathrm J$; compression-only damping gives zero deletion and different speeds |
| Material memory; constitutive alternatives | Change flight duration while recording flight drive and pre-engagement strain | At $T_f=\log2\ \mathrm s$, I retains $e^{-\pi}/4\ \mathrm J$ versus zero after prompt completion |
| Tangential work; conditional sliding laws | Hold normal load, speed and duration; measure drive and tangential work separately | $(W_d,W_t)=(1/10,-1/10)\ \mathrm J$ versus $(0,0)$ at the same kinetic endpoints |
| Wider material behavior; acquisition | Third engagement and independent geometry/damping changes; identify plasticity, adhesion and thermal memory | Each missing relation has its own finite dependency in Section \ref{sec:contact}; a constant-law third deletion is $e^{-3\pi}\ \mathrm J$ |

: The same force/motion instrument can support several comparisons, but destination, release criterion, repeated restitution and wider material behavior have separate closure requirements.

An unchanged gap affects flight timing but not the constant-law contact recurrence. A different measured recurrence after accounting for actual incident velocity distinguishes the unchanged-law reading from material memory or a changed geometry; it does not by itself identify which one. Friction is separated with tangential force and slip, plasticity with permanent deformation and its force history, adhesion with tensile work, motor ripple with drive torque and rate, and thermal/acoustic transfer with calibrated receiver boundaries. Unknown additional laws have no universal numerical prediction; their conditional values require constitutive measurements. The exact zero-deletion and positive-deletion alternatives above remain distinct, finite controls while those laws are identified.

\Needspace{12\baselineskip}

## Singular paths, switching and transformer returns

| Switching question and comparison type | Boundary readout and controlled change | Exact conditional predictions |
|:-------------------------------------|:------------------------------------------|:--------------------------------------------|
| Preparation/coscaling; physical preparations | Observe VII's endpoints and resistor work within its voltage rating | $E^+=1/2\ \mathrm{mJ}$, $W_R=-3/2\ \mathrm{mJ}$ versus zero for relaxed preparation; limiting works follow \eqref{eq:singular-work} |
| Prepared switching; physical paths | Hold VIII's prepared voltages and final state; interchange channels | $(W_A,W_B)=(-3/4,-3/16)$ versus $(-3/16,-3/4)\ \mathrm{mJ}$ |
| Partition; settled scalar result, device law open | Compare sequential/overlapping paths within the conductance ceiling | Sequential pair above versus $(-15/32,-15/32)\ \mathrm{mJ}$; equal endpoints |
| Switch/clamp law; finite laws and acquisition | Record winding, switch, clamp and receiver powers and both event-side states | IX clamp: $(v_C^+,i_2^+)=(-1,0)$ in V/A, $W_c=1/1500-\pi^2/2000\ \mathrm J$; short path: $(0,\pi/20)$, $W=-3\pi^2/8000\ \mathrm J$ |
| Joint limits/orientations; physical paths | Change finite $C_p$, duration and sign of $M$ at known preparation | Capacitor fraction $1$ at $\theta=\pi/2$, $0$ at $\theta=\pi$; canonical secondary signs reverse with $M$ |
| Transformer return; complete finite paths | Hold XII's preparation, source and total duration $3h$; change overlap to immediate new return | Old-return work changes by $-\delta_A<0$; all eight differences and endpoint stores follow \eqref{eq:commutation-comparison} |

: Each work is measured on its named branch. Equality of their total or of the terminal waveform does not establish equality of their partitions.

The prepared-network comparison must cover the stated component and preparation families, including charge and linkage observations separately, before a singular physical path is assigned. The two-capacitor proof already settles path dependence within its scalar model; hardware closure concerns the measured voltage-dependent switch laws and added stores. The two finite clamp models neither identify an arc nor establish a full release topology. Arc ignition/restrike and clamp release require actual branch conductance and both event-side states on the relevant finite operating interval. Finite ratio measurements cannot establish an entire continuous singular surface without an analytic bound; \eqref{eq:parasitic} supplies such an exact result only for its stated lossless cell.

For XII, $[i_s-i_1+\mu i_2-G_kv_a]/v_a=g_e$ supplies a direct overlap observation where $v_a$ is bounded away from zero. Combined conductance uncertainty below $1/2\ \mathrm S$ separates its overlap and no-overlap laws. Old-return work additionally has the strict separation $\delta_A$ at equal source duration, with budget $B_A<\delta_A/2$. Its eight-port ledger tests the complete connection; the return-capacitor and isolated tap-loop examples are subcircuit controls. A coordinate change is an accounting control, and a both-returns-open interval still requires an additional physical path. Switch-control supplies remain measured external ports beyond the ideal graph.

\Needspace{12\baselineskip}

## Controlled supply and accelerating reference

| Question and comparison type | Independently instrumented quantities | Exact conditional predictions |
|:---------------------------------|:------------------------------------------|:---------------------------------------------|
| Bias-coil transfer; receiver alternatives | X's measured force/velocity, actuator $u_ai_a$, bias $u_bi_b$, link power and all endpoints | Regenerative $\Delta E_b=3\log2/10000-3/800000\ \mathrm J$ versus dump $-3/800000\ \mathrm J$; actuator copper $27/320000\ \mathrm J$ in both |
| Reference correspondence; bounded identity and supply alternatives | XI/XIII receiver and driver supplies, shaft torque/rate, finite rail | XI receiver $1/5\ \mathrm J$ versus zero; rail input $1/5$ or $1/4\ \mathrm J$. Lossless XIII driver input $3/200000\ \mathrm J$ |
| Dissipative reference; exact event control | Add XIII's $1/10\ \Omega$ winding resistance with the specified commands; retain all power signs | Node work $1/63\ \mathrm J$, winding work $-1/63\ \mathrm J$, driver input $43/2800000\ \mathrm J$ |
| Hidden modal preparation; finite stores | XIV's separate winding preparation, source-off copper works and endpoints; compare relaxed preparation | Initial store $31/16000\ \mathrm J$, final $31/64000\ \mathrm J$, versus zero in the relaxed control |

: Supply costs and state correspondence require different measurements. A receiver balance alone determines neither converter efficiency nor the compound driver.

The transducer's force must be observed independently of its command, and actuator, bias, thermal and DC-link residuals must be evaluated separately. Each unresolved signed remainder is retained through \eqref{eq:measured-residual}. A positive coil change is compared with measured reaction and all supply paths. For the fixed-coupling receiver law, \eqref{eq:bias-efficiency} supplies the conditional sign threshold; a bias-dependent plant needs its own measured gains and resolved interval/subledger accuracy. The compound state map and both XIII receiver event certificates are settled within their declared laws; actual converter costs and other nonlinear event families retain their separate scope. XIV distinguishes retained winding energy from an erased preparation even as the common current tends to zero. A finite $1\ \mathrm V$ reference change with XI's driver predicts the works in \eqref{eq:reference-jump}; shrinking duration at fixed resistance increases required work. Signed positive and negative intervals are retained even when receiver net work is zero.

\Needspace{25\baselineskip}

## Identification and correspondence

| Question and comparison type | Measured comparison | Exact prediction or alternative |
|:-------------------------------------|:----------------------------------------|:------------------------------------------|
| Damped analogy; identity | I's independent mechanical and electrical preparation, free and reset works, with both body ports | Source works $(23/30,0,23e^{-\pi}/30)\ \mathrm J$ in both devices; compare through the mapped scale |
| Contact/support; structural ambiguity and inverse | Hold II's torque/hammer angle; add anvil response and use \eqref{eq:contact-inverse} dynamically | Anvil $1/2$ versus $2/3\ \mathrm{rad}$ at the same hammer angle |
| Weak coefficient; model alternatives | Change III to $(\rho,\eta)=(1,2)$ with calibrated coordinates and covariance | $151/50$ versus $301/100$; separation $1/100$ |
| Resonator; shunt identity and device acquisition | Change the known shunt; independently predict motional parameters on other devices | IV gives $1+\ii$ versus $1+2\ii\ \mathrm S$; the transferable motional law needs separate specification |
| Polarization; structural null and bounded discrimination | Observe V's branch voltages at $\log2$; then split time constants | $(1/2,-1/2)\ \mathrm V$ versus $(0,0)$; split terminal contrast $1/2-1/\sqrt2\ \mathrm V$ |
| Absorber; resolved structural result, calibration open | Hold VI's force/frequency; measure coupling strain and section area | Reaction zero in both; stress amplitude $1$ versus $1/2\ \mathrm{MPa}$ |

: Comparison types and finite observables for the six inherited questions. Omitting preparation or reset readings is an accounting failure, not an alternative trajectory.

For the damped analogy, forces/torques and motions, not homogeneous equation coefficients alone, must be transported through preparation and reset. The contact experiment must vary support and contact independently, first within a declared finite constitutive family; failure of added anvil data to resolve a frequency-dependent support requires a support sensor or a narrower model, not an assertion of full identification. The coefficient experiment must retain temporal correlation and calibration covariance when evaluating the $1/100$ separation. A successful comparison on the declared support does not prove that support globally minimal.

The resonator task remains an acquisition across physical devices, calibrated fixtures and independently changed shunts. The normalized example predicts a discriminant but supplies no substitute traces. Polarization order recovery requires independently prepared branches, a finite time-constant separation domain and actual noise bounds. The absorber's bounded inability to infer stress from terminal reaction is already resolved; calibrated strain, section area and material conversion address the remaining practical extension.

# Relation to earlier work

[*Third- and Higher-Order ODEs*][main] supplies the broader distinction between coefficient constructions, state elimination and physical realization. The present results develop its open questions by attaching explicit preparations, event paths, recipient channels and calibrated observations. The complete finite port correspondence in \eqref{eq:analogy}, the distinct contact release laws and the two-channel work partition each identify information absent from a scalar trajectory.

[Wettstein, Grauberger and Matthiesen (2021)][wettstein] relate hammer-mechanism behavior to a changing sequence of contacts and embodiment relations. That modeling context motivates retaining contact and support coordinates through engagement. The exact release destination and repeated constitutive law here require their own measurements. [Bible (2002)][bible] describes the conventional crystal motional branch and shunt capacitance used in \eqref{eq:resonator}; that component description does not establish a transferable coefficient law across arbitrary devices. [Keysight Technologies (2026)][keysight] explains impedance methods and fixture compensation. Those measurement distinctions support the calibrated complex-port comparison, while uncertainty and internal-state identification remain specific to the apparatus and model class.

[Kalman (1963)][kalman] supplies the general realization and observability distinction; the present contact inverse and prepared polarization controls specify what additional channels identify in particular models. [Willems (1972)][willems] provides the storage/supply framework for interconnected systems; the separately integrated event paths here identify which physical ports that framework needs. [Schwager and Pöschel (2007)][schwager] distinguish repulsive-contact termination from a continued linear-dashpot collision. The retained material state and receiver comparisons in Section \ref{sec:contact} address the additional destination question. These established principles provide context for the explicit constructions, rather than an assignment of any unmeasured work.

# Conclusions

The physical destination of the force-zero contact store remains open. Configuration I leaves $e^{-\pi}\ \mathrm J$ at detachment: deleting that state without an assigned event port gives the signed deficit $-e^{-\pi}\ \mathrm J$. Prompt export and retained material relaxation predict different observations, with $e^{-\pi}/4\ \mathrm J$ remaining after $\log2\ \mathrm s$ in the latter. Strain, receiver work and both event-side states distinguish them. Repeated contacts must carry that residual preparation or include a measured reset; plasticity, adhesion, geometry and thermal memory retain distinct constitutive requirements.

Switching redirects individual transfers. Equal capacitor endpoints accompany $(-3/4,-3/16)$ or reversed channel works in millijoules. XII's complete transformer return paths hold source duration fixed and differ by the strictly positive old-return work separation $\delta_A$, with sufficient measurement half-width below $\delta_A/2$. Their states and eight separate port integrals are specified; actual switch, clamp, gate and parasitic laws remain to be identified. Prepared singular limits likewise retain their impulse or relaxation works. In XIV a finite winding preparation stores $31/16000\ \mathrm J$ and leaves $31/64000\ \mathrm J$ after its declared source-off interval. Vanishing common current in the wider family can retain a nonzero store.

The source-off bias-coil increase is positive in X: $\Delta E_b=3\log2/10000-3/800000\ \mathrm J$. The fixed-coupling plant and separate receiver predict the conditional efficiency threshold $\eta>1/(100\log2)$, with finite actuator storage and copper loss retained. The open realization question concerns the actual bias-dependent couplings, conversion and regulation costs. Thermal endpoints, signed-power quadratures, interval residuals and DC-link subledgers of the wider finite-supply models retain their accuracy limitations. Independent force, electrical and thermal observations determine which signed transfers accompany the coil increase.

An accelerating-reference counterpart requires separately supplied compensation and driver work. XI receives $1/5\ \mathrm J$; lossless XIII returns to zero receiver store and zero signed receiver work while its driver requires $3/200000\ \mathrm J$. The dissipative extension instead has node work $1/63\ \mathrm J$, opposite winding heat and driver input $43/2800000\ \mathrm J$, with complete exact receiver event coverage. Finite nonideal driver models and conditional preparation limits are bounded results. Actual supply costs, wider connection laws and unrestricted correspondence of all states and works remain physical questions. The reference-change work bound specifies the divergent cost of shrinking duration at fixed positive driver resistance and capacitance.

The inherited observation questions remain integral to these transfers. Damped preparation, free motion and reset give source works $23/30$, zero and $23e^{-\pi}/30\ \mathrm J$. Added anvil response identifies the contact and composite support within a declared model, with explicit inverse-error bounds. Weak coefficients and split polarization modes have finite separation conditions; transferable resonator laws still require independently varied devices. The bounded absorber result remains resolved: zero reaction coexists with stress amplitudes $1$ and $1/2\ \mathrm{MPa}$ in VI. Calibration and wider constitutive families remain separate tasks.

Each energy comparison retains both endpoint stores, every independently integrated signed port and its calibrated uncertainty. A measured residual interval wholly above or below zero records an unresolved gain or deficit relative to the audited input. Its magnitude, sign, preparation, event conditions and completed checks remain explicit while the missing physical relation is investigated.

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
| Retained material state | Integrate $-d_r\dot z^2$ and evaluate remaining strain energy | Detachment map, thermal retention and re-engagement |
| Identification | Static force balance, nonzero design determinant, exact hidden difference mode | Covariance, noise, model-family choice and calibrated stress |
| Singular RC | Integrate $-v^2/R$ before evaluating both capacitor endpoints | Physical approach and voltage constraints at zero capacitance |
| Two capacitors | Integrate each accumulated-action interval separately | Measured conductance, control supply and additional states |
| Clamp | Substitute all three states in \eqref{eq:clamp-state}; integrate $-V_ci_1$ | Real opening, arc/restrike and release destinations |
| Complete return | Derive all three matrices and each port quadratic form from one graph | Actual gate slew, switch supply and additional parasitics |
| Controlled plant | Substitute \eqref{eq:plant-path}; integrate each loss and reaction | Bias-dependent gains and actual actuator tracking |
| Auxiliary actuator | Substitute current/voltage, integrate copper and both terminal works | Regulator response and additional rail consumption |
| Bias and link | Differentiate $i_b^2$ and $V_d^2$; integrate each controller port | Converter efficiency, sensing, thermal material and supply hardware |
| Reference and compound | Derive feedback from KCL; integrate both polynomial receivers and driver heat; certify all receiver roots | Hardware conversion, wider connection/driver laws and unrestricted correspondence |
| Hidden common mode | Integrate separate winding preparation, source and copper powers; evaluate both magnetic endpoints | Which finite preparation and limiting duration describes the apparatus |
| Unexplained remainder | Propagate independent endpoint and work bounds without fitting recipient fractions | Any signed residual beyond those bounds remains open |
| Reference change | Integrate driver source/resistor and prove the duration bound | Other driver laws and joint component limits |
| Measurement bounds | Expand effort--flow and endpoint products without linearization | Actual calibration, timing and constitutive uncertainties |

: The exact constructions have zero numerical integration residual. Named omitted mechanisms remain unevaluated model residuals.

Every figure is either a schematic or the exact closed form given in the text. All tabulated works and endpoints follow by algebra and integration of those forms. No decimal residual, finite-precision failure or coordinate magnitude has been used as physical evidence. The bounded structural and prescribed-cell conclusions remain bounded; resolving an inherited local question does not replace its practical measurement extension.

\Needspace{16\baselineskip}

# References {-}

1. Nilre, H., and Herlin, B. C. (2026). [*Third- and Higher-Order ODEs: Coefficient families, physical realizations, identification, and initial data*][main]. Companion manuscript, latest PDF on GitHub.
2. Wettstein, A., Grauberger, P., and Matthiesen, S. (2021). [Modeling dynamic mechanical system behavior using sequence modeling of embodiment function relations: case study on a hammer mechanism][wettstein]. *SN Applied Sciences* **3**, article 128. DOI: 10.1007/s42452-021-04149-8.
3. Bible, S. (2002). [Crystal Oscillator Basics and Crystal Selection for rfPIC and PICmicro Devices][bible]. Microchip Technology, Application Note AN826, DS00826A, pp. 1--14.
4. Keysight Technologies (2026). [*Impedance Measurement Handbook: A Guide to Measurement Technology and Techniques*][keysight]. Application note 5950-3000, 6th edition, published February 28, 2026.
5. Kalman, R. E. (1963). [Mathematical Description of Linear Dynamical Systems][kalman]. *Journal of the Society for Industrial and Applied Mathematics, Series A: Control* **1**(2), 152--192. DOI: 10.1137/0301010.
6. Willems, J. C. (1972). [Dissipative Dynamical Systems Part I: General Theory][willems]. *Archive for Rational Mechanics and Analysis* **45**, 321--351. DOI: 10.1007/BF00276493.
7. Schwager, T., and Pöschel, T. (2007). [Coefficient of restitution and linear--dashpot model revisited][schwager]. *Granular Matter* **9**, 465--469. DOI: 10.1007/s10035-007-0065-z.

8. Basu, S., Pollack, R., and Roy, M.-F. (2006). [*Algorithms in Real Algebraic Geometry*][basu]. 2nd edition, Algorithms and Computation in Mathematics **10**. Springer, Berlin, Heidelberg. DOI: 10.1007/3-540-33099-2.

[main]: https://github.com/hobnilre/physics-ode-3rd-deg/blob/main/third-and-higher-order-odes.pdf
[wettstein]: https://doi.org/10.1007/s42452-021-04149-8
[bible]: https://ww1.microchip.com/downloads/en/appnotes/00826a.pdf
[keysight]: https://www.keysight.com/us/en/assets/7018-06840/application-notes/5950-3000.pdf
[kalman]: https://doi.org/10.1137/0301010
[willems]: https://doi.org/10.1007/BF00276493
[schwager]: https://doi.org/10.1007/s10035-007-0065-z

[basu]: https://doi.org/10.1007/3-540-33099-2
