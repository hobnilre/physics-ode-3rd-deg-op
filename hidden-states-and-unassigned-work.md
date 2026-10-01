---
title: "Hidden States and Unassigned Work"
subtitle: "Physical questions and signed work behind higher-order coefficients"
author: "Hob Nilre & Bo C. Herlin"
date: "2026-09-26"
abstract: |
  Higher-order coefficient laws raise physical questions about which internal states observations identify and which stores and transfers they leave undetermined. A rotary impact driver provides a continuous comparison: hammer, anvil and torque observations distinguish contact from joint dynamics, independent component changes test a fixed local law, and torque-zero release can retain positive contact storage. We derive the local inverse, release alternatives and signed event accounts under explicit preparation and constitutive assumptions. Calibrated prediction sets separate distinguishable alternatives from exact terminal ambiguity and inadequate resolution. Endpoint stores and separately integrated port works retain the sign of any unexplained residual. Twelve physical questions are stated with their established and unresolved scope; complete supporting models, uncertainty calculations and finite implementation studies are retained in the appendices. The proposed measurements distinguish exact model results from constitutive acquisition and hardware correspondence.
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

# Physical questions behind a coefficient law
\label{sec:introduction}

A rotary impact driver turns a coefficient law into a recognizable physical question. Its rotating hammer meets the anvil's engagement faces; the anvil, chosen bit or socket and tightened joint transmit and resist the blow. The contact and joint can contribute different dynamics even when one hammer trace fits a scalar equation. At release, the same model can leave elastic energy in the contact. The questions are which observations identify those dynamics and which retained states or measured transfers describe the event.

[*Third- and Higher-Order ODEs*][main] constructs the coefficients, proves their support and higher-order recurrences, and establishes their identification and realization limits. This companion develops the physical comparisons and signed accounts for its twelve marked questions. Each model below specifies its own components, preparation, ports and assumptions. The impact driver is the principal example; electrical and other mechanical systems supply complementary controls. For each comparison, choose the physical part whose law is being identified, its attachment and input, and the terminal or internal observation that can distinguish it. The main article presents the core coefficient construction and retains its complete proofs and applications in appendices; here the observations test whether those laws belong to the proposed contact, joint or electrical branch and predict the connected system.

The damped correspondence question asks whether mechanical and electrical models transport preparation, relaxation and reset ports as well as their equations [OP-LR50-01]. The impact-driver identification question asks which hammer, anvil, contact-torque and support observations separate contact coefficients from a frequency-dependent joint [OP-LR08-01]. At torque-zero release, a spring--damper contact retains $U_c=d_c^2\dot\delta_-^2/(2k_c)>0$ for nonzero relative speed. Here $k_c$ is contact stiffness, $d_c$ is damping, and $\delta$ is relative angular deformation; a dot denotes a time derivative and the subscript $-$ denotes the instant before release. Removing that store without an event transfer gives a negative residual; its retained-material, acoustic, thermal, fracture or fixture destination remains unidentified [OP-LR03-01]. The constitutive release criterion, flight work and memory carried into later engagements are parts of that physical comparison.

The next questions concern the information carried by observations. Coefficient identification asks whether independent component coordinates and realistic correlated uncertainty distinguish weak contributions that coincide on a restricted path [OP-LR31-01]. Calibrated resonator observations must establish a transferable rational law across devices and independently changed shunts [OP-LR12-01]. A quiet terminal raises a separate bound question: how much prepared energy can remain hidden when coupling and preparation are uncertain, including multiple nearly cancelling and nonideal modes [OP-LR23-01]? An exact single-branch resistor account can be complete while that broader observation question remains open.

Polarization branches ask how effective order can be recovered from noisy data and arbitrary branch preparations [OP-LR01-04]. Equal time constants can hide an independently relaxing difference state. For the tuned absorber, terminal reaction's inability to identify internal coupling stress is resolved within its bounded normalized structural scope; calibrated internal observations, raw-unit identification and wider physical models remain separate questions [OP-LR58-01]. A controlled transducer asks whether its actual bias and supply realize the specified couplings and source-off coil increase with independently resolved actuator, coil, DC-link and thermal accounts [OP-LR59-02]. The fixed-coupling receiving-coil control and a nonlinear bias-dependent plant are different realizations.

Other questions concern the connections and supplies that realize a law. Transformer questions distinguish changing a voltage origin from attaching an actual ground bond, probe return or parasitic capacitance. The physical attachments alter individual signed works, endpoint stores and potentially the number of states [OP-TRF-01]. Whether calibrated simultaneous voltage and current integrals and independent endpoint observations agree with those declared finite models remains a hardware question [OP-TRF-07]. The attachment construction below supplies exact conditional predictions for tapped and isolated graphs; it supplies no measured discrepancy.

An accelerating-reference counterpart requires physical compensation and a driver. Finite mechanical and electrical realizations must be compared through preparation, loaded evolution, reference changes and reset, with their separately supplied works and independently evaluated stores [OP-TRF-12]. Bounded active constructions, dissipative event certificates and conditional reduction results are established within their laws. Converter and sensor behavior, broader preparation and nonlinear event families, and unrestricted physical correspondence retain their separate scope.

Contact laws, prepared singular reductions and switching controls develop the states and boundaries needed by these questions. Equal capacitor endpoints can accompany unequal individual switch works; a vanishing terminal coordinate can conceal finite prepared storage. The measurements in Appendix \ref{sec:measurements} retain these distinct alternatives, finite apparatus domains and calibrated uncertainty. Identical terminal predictions are an identification result; an additional internal channel can make them distinguishable.

The main text follows contact and joint identification through release and the interpretation of measurements. Complete supporting systems and implementation accounts appear in the appendices; Appendix \ref{app:measurement} includes the configuration guide.

Identification asks which states or coefficients are determined. Acquisition asks which additional observations can determine them. A signed account asks which independently evaluated stores and transfers explain an interval. Implementation asks whether measured components realize the declared laws. These are different question dispositions: a resolved ambiguity or bounded no-return theorem does not resolve its wider hardware or constitutive parent. In particular, the bounded absorber result remains resolved; the insulated thermal obstruction and the two-preparation finite-error obstruction below are likewise resolved only within their declared contracts.

# Boundaries, ports and exact work
\label{sec:ledger}

The release comparison needs a common convention for stored energy and transferred work. For each system let $x$ contain its independent physical states. Its constitutive store $E(x)$ is evaluated at both ends of the declared interval. A port has effort $e_\ell$ and conjugate flow $f_\ell$, with positive product into that boundary. The definitions are
\begin{equation}
 W_\ell(t_0,t_1)=\int_{t_0}^{t_1}e_\ell(t)f_\ell(t)\,\dd t,
 \qquad r_E=E(x(t_1))-E(x(t_0))-\sum_\ell W_\ell.
 \label{eq:ledger}
\end{equation}
Thus $r_E$ compares the evaluated change in storage with the separately integrated inward works. A positive residual means that the storage change exceeds those works; a negative residual means that it falls below them. The sign alone does not identify a missing state or transfer.

Electrical ports use $vi$, mechanical ports use $Fv$ or $\tau\omega$. A thermal export uses $-T_b\dot S_{\rm out}$, where $T_b$ is the boundary temperature and $\dot S_{\rm out}$ is entropy carried outward by heat, excluding internal entropy production. Acoustic export is $-\int p v_n\,\dd A$ with outward normal velocity $v_n$. A resistor outside the stored subsystem contributes $-v(v/R)$, and a damper contributes $-(dv)v$. These are separate integrals, even when their sum has a simpler expression. Whenever a resistor is included physically but only reactive storage is retained, its thermal storage is explicitly neglected; otherwise electrical dissipation first changes its thermal state and need not equal immediate exterior heat flow.

At a connection event, $x(t_e^-)$ and $x(t_e^+)$ denote the states immediately before and after the event; their evolution can obey different laws or constraints. A finite interval resolving the event determines each work. A singular work is the limit of those integrals if it exists. Deleting a constitutive store and writing an event term equal to its negative closes a mathematical ledger, but supplies no effort, flow or physical recipient. That term must remain distinguished from a measured transfer.

For a finite mass, $m\dot v=F$ gives $\int Fv\,\dd t=m[(v^+)^2-(v^-)^2]/2$ by integrating the product. This equals $J(v^-+v^+)/2$ when $J=m(v^+-v^-)$; it does not define a product of an unspecified delta force with a discontinuous velocity. A fixed support can exchange momentum while its work is zero. A moving support needs its own force--velocity integral.

Closed-form integrations evaluated below are exact within their declared models. Unevaluated matrix-function and time-ordered work expressions remain exact definitions; their numerical evaluation and physical uncertainty are not assigned zero error. A closed ideal ledger has $r_E=0$ by direct substitution after the separate integrals. The physical model residual $r_{\rm model}$ includes omitted material memory, switch-control supply, heat storage, exterior fields or release destinations, as named for each construction. Its sign and magnitude remain unevaluated unless a declared additional law determines them. This use of storage and supplied work is consistent with [Willems (1972)][willems]; the physical ports and stores still have to be identified for each realization.

Figure \ref{fig:boundaries} separates the observed port from hidden states and event transfers.

![Schematic of an observed physical system. The terminal trace constrains a projection of the state. Separate preparation, release and internal-observation paths remain necessary.](figures/boundaries.pdf){#fig:boundaries width=100%}

\FloatBarrier

# Identifying contact and joint dynamics
\label{sec:contact-identification}

A rotary impact driver repeatedly accelerates a hammer, engages its faces with an anvil, loads the output, and releases for the next blow. The chosen bit or socket and tightened joint belong to the declared output boundary. Assign rigidly co-moving output mass to $J_a$; assign attachment twist and dissipation to the support law only when those deformations are resolved there. A separate attachment inertia instead adds its own state. No component is counted twice. The impact-wrench mechanism supplies the hammer–anvil correspondence used here [Wettstein, Grauberger and Matthiesen (2021)][wettstein].

Apply hammer torque $u$ and observe hammer and anvil angles $\theta_h,\theta_a$. Take positive inertias $J_h,J_a$ and positive stiffnesses and damping constants $k_c,d_c,k_j,d_j$ on the active-contact interval. The subscripts $c$ and $j$ denote contact and the grounded joint/support, respectively. With contact torque $\tau_c=k_c(\theta_h-\theta_a)+d_c(\dot\theta_h-\dot\theta_a)$ and support torque $\tau_j=k_j\theta_a+d_j\dot\theta_a$, the equations are
\begin{equation}
 J_h\ddot\theta_h=u-\tau_c,\qquad
 J_a\ddot\theta_a=\tau_c-\tau_j.
 \label{eq:two-inertia}
\end{equation}
They give a generic fourth-order hammer equation. Write $D=\mathrm d/\mathrm dt$ and let $s$ be its transform variable; at angular frequency $\omega$, $s=\ii\omega$ with $\ii^2=-1$. Upper-case $U,\Theta_h,\Theta_a$ denote transformed signals or their steady sinusoidal amplitudes. The rational relations below describe zero-state transfer, with all initial states zero, or steady sinusoidal response; arbitrary preparations add initial-state terms. Dynamic stiffness is torque divided by angular displacement at the specified port. With local dynamic stiffnesses $\mathcal K_c=k_c+d_cs$, $\mathcal K_j=k_j+d_js$ and $\mathcal K_a=J_as^2+\mathcal K_j$, elimination gives
\begin{equation}
 \frac{U}{\Theta_h}=J_hs^2+\frac{\mathcal K_c\mathcal K_a}{\mathcal K_c+\mathcal K_a},\qquad
 \frac{\Theta_a}{\Theta_h}=\frac{\mathcal K_c}{\mathcal K_c+\mathcal K_a}.
 \label{eq:contact-inference}
\end{equation}
These are torque/angle dynamic stiffnesses. The corresponding torque/angular-velocity impedance is $\mathcal K/s$ where defined, and the hammer mobility is $s/(J_hs^2+\mathcal K_e)$ with $\mathcal K_e=\mathcal K_c\mathcal K_a/(\mathcal K_c+\mathcal K_a)$. The terminal observes a composite dynamic stiffness. If a broader rational support is allowed, different admissible decompositions of that composite must be distinguished before assigning internal coefficients. Positivity, a known inertial model and a sufficiently rich frequency domain can impose additional constraints; static ambiguity alone is not a theorem of ambiguity on every frequency domain.

The anvil-to-hammer angle ratio supplies a second observation of the same assembly. With known $J_h$ and measured $\mathcal K_e=U/\Theta_h-J_hs^2$ and $H_a=\Theta_a/\Theta_h$, the same equations give a constructive inverse:
\begin{equation}
 \mathcal K_c=\frac{\mathcal K_e}{1-H_a},\qquad
 \mathcal K_a=\frac{\mathcal K_e}{H_a},\qquad
 \mathcal K_j=\frac{\mathcal K_e}{H_a}-J_as^2.
 \label{eq:contact-inverse}
\end{equation}
Indeed $1-H_a=\mathcal K_a/(\mathcal K_c+\mathcal K_a)$, so substitution proves the first two expressions; subtracting the known anvil inertia gives the joint law. They require defined responses and nonzero denominators; errors are amplified near $H_a=0$ or $1$. In the stated spring--damper family, a nonzero real frequency determines $k_c=\operatorname{Re}\mathcal K_c$, $d_c=\operatorname{Im}\mathcal K_c/\omega$, $k_j=\operatorname{Re}\mathcal K_a+J_a\omega^2$ and $d_j=\operatorname{Im}\mathcal K_a/\omega$ when $J_a$ is known. Additional frequencies check that family. Recovering the composite $\mathcal K_a$ does not identify an arbitrary internal support realization. The distinction between a realization and its observable input--output part is the one formalized by [Kalman (1963)][kalman].

The inverse has an exact uncertainty bound. Write $K=\mathcal K_e$, $H=H_a$, with absolute errors at most $\epsilon_K,\epsilon_H$; hats denote estimates obtained from the measured responses. When $|H|>\epsilon_H$ and $|1-H|>\epsilon_H$, subtraction of the two rational inverses and the triangle inequality give
\begin{align}
 |\widehat{\mathcal K}_c-\mathcal K_c|&\leq
 \frac{\epsilon_K|1-H|+|K|\epsilon_H}
 {|1-H|(|1-H|-\epsilon_H)},\nonumber\\
 |\widehat{\mathcal K}_a-\mathcal K_a|&\leq
 \frac{\epsilon_K|H|+|K|\epsilon_H}
 {|H|(|H|-\epsilon_H)}.
 \label{eq:contact-inverse-error}
\end{align}
Indeed the two error numerators are $\delta K(1-H)+K\delta H$ and $\delta KH-K\delta H$. Lower bounds on the denominator magnitudes yield \eqref{eq:contact-inverse-error} without linearizing the errors. Calibrated magnitude envelopes replace unknown true values in an experiment. At known $J_a$, the same absolute bound as for $\mathcal K_a$ applies to $\mathcal K_j$; uncertainty in $J_a$ adds $\omega^2\epsilon_{J_a}$ at $s=\ii\omega$. These bounds apply to the composite support; its internal realization still requires a specified family or further sensors.

The local ambiguity at one complex frequency is also explicit. Writing $\mathcal K_e=\mathcal K_c\mathcal K_a/(\mathcal K_c+\mathcal K_a)$ and $H_a=\Theta_a/\Theta_h$, differentiation gives
\begin{equation}
 \delta \mathcal K_e=\frac{\mathcal K_a^2\delta \mathcal K_c+\mathcal K_c^2\delta \mathcal K_a}{(\mathcal K_c+\mathcal K_a)^2}.
 \label{eq:contact-null}
\end{equation}
For nonzero $\mathcal K_c,\mathcal K_a,\mathcal K_c+\mathcal K_a$, the perturbation $\delta \mathcal K_a=-(\mathcal K_a/\mathcal K_c)^2\delta \mathcal K_c$ leaves that terminal observable unchanged to first order, while $\delta H_a=\mathcal K_a\delta \mathcal K_c/[\mathcal K_c(\mathcal K_c+\mathcal K_a)]$ is generally nonzero. A parameterized passive model constrains which such perturbations extend over the full frequency interval. Consequently the combined observation Jacobian, its covariance-weighted sensitivity and independent-frequency prediction must be checked for the declared family, rather than inferred from this local null alone.

The prepared-motion obstruction is exact as well. Let $k_c,d_c>0$ and
$\Delta=k_c^2-k_cd_cd_j/J_a+d_c^2k_j/J_a=0$.
Two solutions with the same drive can differ by
\begin{equation}
 \delta\theta_h=0,\qquad
 \delta\theta_a=Ae^{-k_ct/d_c},\qquad
 \delta\tau_c=0.
 \label{eq:hidden-anvil-observation}
\end{equation}
Indeed $k_c\delta\theta_a+d_c\delta\dot\theta_a=0$, and substitution into the anvil equation leaves $J_ak_c^2-d_jk_cd_c+k_jd_c^2=J_a\Delta=0$. Both hammer motion and contact torque are identical, while anvil motion differs. For example, normalized $J_h=J_a=k_c=d_c=k_j=1$, $d_j=2$ satisfy these conditions with positive components. An anvil-angle separation $|A|e^{-k_ct/d_c}$ greater than the combined angle-error bound distinguishes the preparations at that time; a hammer-only comparison cannot. The extra observation is therefore part of identification, rather than an energy outcome used to select coefficients.

Configuration II makes the simplest ambiguity exact. At static torque $u=1\ \mathrm{N\,m}$, both $(k_c,k_j)=(2,2)$ and $(3,3/2)\ \mathrm{N\,m/rad}$ give $\theta_h=1\ \mathrm{rad}$. The corresponding $\theta_a$ values are $1/2$ and $2/3\ \mathrm{rad}$, and contact deformations are $1/2$ and $1/3\ \mathrm{rad}$. Contact and support stores are respectively $(1/4,1/4)$ and $(1/6,1/3)\ \mathrm J$. Static power is zero; these endpoint stores do not assign the earlier preparation work.

The physical two-body boundary contains both kinetic stores and both springs. Its independently signed external powers are $u\dot\theta_h$, $-d_c(\dot\theta_h-\dot\theta_a)^2$ and $-d_j\dot\theta_a^2$. A movable support at angle $z$ replaces the second deformation by $\theta_a-z$ and adds inward support power $-\tau_j\dot z$. A support inertia and another spring give their own second-order state equation and can raise the full order to six. Measuring the anvil alone then does not guarantee identification of $z$ or of an arbitrary rational support.

For phase-resolved identification, maintain engagement under a declared preload and use a small imposed sinusoidal torque with synchronized hammer and anvil angles. Verify the linear amplitude and frequency domain, including calibrated channel phase. Use peak phasors with $e^{\ii\omega t}$; transient preparation must have decayed or be independently separated before applying the steady-response inverse. A blow instead includes engagement, prepared states and release. Transferring the identified contact or joint law to that transient requires an independent domain check. One informative nonzero frequency can identify the four spring--damper constants under the assumptions above; it cannot identify an unrestricted rational law or its internal realization.

The finite closure question is a rank and uncertainty statement for specified contact and support families, followed by prediction under independently changed support and contact conditions. The bounded normalized-map results do not imply universal raw-unit identifiability. Calibrated contact torque, anvil motion and, where required, support motion distinguish the alternatives in \eqref{eq:contact-inference}. The mechanism-level need to represent changing contacts is consistent with [Wettstein, Grauberger and Matthiesen (2021)][wettstein]; that study supplies neither a universal release law nor the destination considered here.

Which measurements separate contact dynamics from the frequency-dependent joint against which the impact driver strikes? This is the principal application-specific identification question. A practical discriminating setup is a low-energy torsional impact between two instrumented disks and an interchangeable compliant support. Two encoders provide synchronized hammer and anvil angles, with rates reconstructed within their calibrated response band; a calibrated transducer observes contact torque at the declared interface. A support-torque channel adds a direct observation of joint loading. Choose the slow contact so its discrimination frequencies lie inside the common calibrated amplitude and phase band, and include rate-reconstruction error in the uncertainty. Hold inertia and contact geometry fixed while changing support stiffness, then change contact compliance independently. Agreement of hammer motion with disagreement in anvil motion rejects a claimed internal reconstruction. Trigger offset, probe loading, anti-alias response, colored uncertainty and fixture variation must enter the comparison. For a selected commercial driver, record the bit or socket allocation, sensor location, contact-duration range and usable calibrated bandwidth anew; the slow rig does not establish these. A fully synchronized industrial impact measurement is a stronger, separately unfulfilled requirement.

## One continuous coefficient-prediction comparison
\label{sec:impact-protocol}

Use the same two-disk boundary through calibration, prediction and release. Allocate the hammer disk to $J_h$ and all rigidly co-moving anvil/attachment parts to $J_a$; place measured attachment deformation in the joint law. Fix the support reference or record its motion explicitly. Measure applied torque $u$, both angles and contact torque, and independently calibrate inertia and channel loading. Maintain contact under a stated preload and determine the spring--damper constants from \eqref{eq:contact-inverse}, using several frequencies to test the family and \eqref{eq:contact-inverse-error} to propagate the calibrated complex-response errors. A separate support-torque channel checks the inferred joint law. Preparation transients must be retained or separated within that same domain.

Freeze the law and choose three independent physical settings before the final observations: a reference setting, a changed joint stiffness with the same contact, and a changed contact damping with the reference joint. The coefficient prediction is the complete forced equation
\begin{equation}
 \begin{aligned}
 P(D)\theta_h&=(J_aD^2+(d_c+d_j)D+k_c+k_j)u,\\
 P(s)&=J_hJ_as^4+[J_h(d_c+d_j)+J_ad_c]s^3\\
 &\quad+[J_h(k_c+k_j)+J_ak_c+d_cd_j]s^2\\
 &\quad+(d_ck_j+k_cd_j)s+k_ck_j.
 \end{aligned}
 \label{eq:impact-protocol-polynomial}
\end{equation}
In descending derivative order, from $D^4$ to $D^0$, an independent change $\Delta k_j$ predicts coefficient changes $(0,0,J_h\Delta k_j,d_c\Delta k_j,k_c\Delta k_j)$ and forcing changes by $\Delta k_j u$. For $\Delta d_c$ they are $(0,(J_h+J_a)\Delta d_c,d_j\Delta d_c,k_j\Delta d_c,0)$ and forcing changes by $\Delta d_c\dot u$. Hold all other physical quantities and the normalization rule fixed. If reference scales themselves change, rescale both sides anew. These formulas predict changes without fitting the final setting.

For each setting propagate the measured physical preparation through \eqref{eq:two-inertia}; its output and contact-torque predictions use the same state. A prediction set collects all observations allowed by the law and its stated uncertainty. Generate a joint prediction set from component calibration, correlated channel errors, support motion, sensor loading, phase/bandwidth, differentiated-rate errors and trigger timing. Distinguish laws only when their prediction sets are disjoint on the chosen observation. A nominal full-rank matrix is insufficient. The coordinate experiment in Appendix \ref{sec:coefficient-identification} supplies an explicit correlated-path failure and independent-coordinate recovery; its hypothetical weak coefficient is not asserted to equal every coefficient in \eqref{eq:impact-protocol-polynomial}. Unknown exponents require their own support and recovery assumptions.

Carry the held-engaged law to a slow impact only after its deformation, rate, preload and temperature domain has been checked. Engagement and release change topology, so transport physical states and recompute one-sided jets: the angle derivatives generated by the appropriate equations on each side of the event. A hammer-only comparison cannot separate the exact pair in \eqref{eq:hidden-anvil-observation}; the predicted anvil separation and its error bound can. Finally evaluate the contact store at release and compare candidate recipients as the separate question in Section \ref{sec:contact}. An energy result does not revise the coefficient selection.

The admissible outcomes are prediction on the independent setting, separation of another declared law, insufficient observational separation, or failure of the model/uncertainty specification. This is a complete conditional protocol; no apparatus success is asserted. Applying it to a selected commercial driver requires its own attachment allocation, calibrated contact regime and bandwidth.

# Contact release and repeated engagement
\label{sec:contact}

Identifying the engaged contact law leaves a further question: which event ends that law, and what becomes of its stored deformation? We first compare release rules in a free normal collision, where relative motion has a closed form. This comparison uses a different boundary from the grounded rotary driver. The torque-zero store identity is then applied locally to that driver in Section \ref{sec:release-open}, with its motor and joint transfers retained.

## Three constitutive laws with different endpoint predictions

For a free normal collision of masses $m_1,m_2>0$, the center-of-mass motion separates from relative compression $\delta\geq0$. Here $\delta$ is a length, and $m=m_1m_2/(m_1+m_2)$ is the reduced mass: the opposite contact forces give $\ddot\delta=-F_c(1/m_1+1/m_2)$. The relative boundary contains $K=m\dot\delta^2/2$ and $U=k\delta^2/2$, with contact stiffness $k>0$ and damping $d>0$. On active contact its law is $m\ddot\delta=-F_c$, initially $\delta=0$, $\dot\delta=v_0>0$. Contact damping exports power $-(d\dot\delta)\dot\delta$; external relative drive and fixture powers, when present, are separately $f_d\dot\delta$ and $f_b\dot\delta$. They vanish during the free contact considered here. The two-body center-of-mass kinetic energy is evaluated separately and remains unchanged because the external force sum is zero.

For $F_c=k\delta+d\dot\delta$ with $a=d/(2m)$, $\omega_0=\sqrt{k/m}$ and $\omega_d=\sqrt{\omega_0^2-a^2}>0$, force balance gives
\begin{equation}
 \delta(t)=\frac{v_0}{\omega_d}e^{-at}\sin\omega_dt,
 \qquad \dot\delta(t)=v_0e^{-at}
 \left(\cos\omega_dt-\frac a{\omega_d}\sin\omega_dt\right).
 \label{eq:contact-solution}
\end{equation}
The restitution coefficient is the outgoing relative speed divided by the incoming speed $v_0$. Let $\zeta=a/\omega_0\in(0,1)$. The first force zero occurs at
$t_F=2\arccos\zeta/\omega_d$, with restitution $e_F=e^{-at_F}$, velocity $-e_Fv_0$ and deformation $d e_Fv_0/k$. The first deformation zero is $t_D=\pi/\omega_d$ and gives $e_D=e^{-at_D}$. Between $t_F$ and $t_D$ the linear force is tensile. A unilateral law must therefore specify which event ends the model.

The distinction between these collision endpoints for a linear dashpot is developed by [Schwager and Pöschel (2007)][schwager]. That constitutive distinction determines restitution within the selected law; it does not identify a physical recipient for an omitted elastic state.

A third law acts with damping only in compression:
$F_c=k\delta+d\max(\dot\delta,0)$ for $\delta>0$, followed by separation at $\delta=0$. It follows \eqref{eq:contact-solution} until maximum compression $t_P=\arccos\zeta/\omega_d$, then an undamped spring rebound for $\pi/(2\omega_0)$. Its restitution is $e_C=e^{-at_P}$. This is a different constitutive law, not an instruction to clip a tensile force while retaining an unchanged store balance.

For contact configuration I, choose $m=1\ \mathrm{kg}$, $d=2\ \mathrm{N\,s/m}$, $k=2\ \mathrm{N/m}$ and $v_0=1\ \mathrm{m/s}$. Thus $a=\omega_d=1\ \mathrm{s^{-1}}$, $\omega_0=\sqrt2\ \mathrm{s^{-1}}$, and $F_c=2e^{-t}\cos t\ \mathrm N$ before any change of law.

\Needspace{12\baselineskip}

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

## The unresolved store at contact release
\label{sec:release-open}

For the rotary impact driver, use relative angle $\delta=\theta_h-\theta_a$, contact torque $k_c\delta+d_c\dot\delta$ and contact store $U_c=k_c\delta^2/2$. The force-zero derivation above then gives the torque-zero store and deletion residual with $k,d$ replaced by $k_c,d_c$. Motor, joint and fixture transfers remain separately oriented ports. No release law or destination follows from the coefficient representation alone.

Assigning $W_{\mathrm{release}}=-U_c(t_e^-)$ makes an augmented mathematical ledger close. It specifies the transfer that would be needed; it does not identify that transfer. Four exclusive counterfactual accounts can assign the whole amount to acoustic radiation, heat, fracture or fixture motion. They are alternatives, not four simultaneous works, and cannot be summed or averaged into an identified partition. A mixed physical destination requires separately evaluated channel works and a remaining unassigned part. A finite release path must supply each effort--flow product, including acoustic pressure times volume flow, support torque times angular speed, or a specified thermal or fracture transfer.

For several deleted contact stores, the event contribution is exactly
\begin{equation}
 r_{E,\mathrm{gates}}=-\sum_jU_c(t_j^-).
 \label{eq:release-sequence}
\end{equation}
Motor work, damper work and fixture transfer on the intervening finite intervals are integrated separately. A fixed fixture has zero work and can still supply the impulse needed in the momentum account. At deformation-zero release the elastic store is zero, but the Kelvin--Voigt force may already have become tensile. A compressive-only law needs its own state and release definition; force clipping alone does not specify what happens to stored deformation. A nonlinear contact with torque $k_c\delta+k_3\delta^3+d_c\dot\delta$ has potential $U_c=k_c\delta^2/2+k_3\delta^4/4$, since its deformation derivative is the elastic torque. It gives the corresponding event deficit $-U_c(t_e^-)$ under the same deletion assumptions. Restitution above unity requires evaluating any prepared spring change and active-port work on the stated interval rather than deciding its interpretation from the restitution value alone.

A slower compliant torsional contact with measured torque, angles and spring deflection can first distinguish retained deformation from an imposed state deletion. Ordinary encoders and a torque sensor can resolve that limited question without measuring a short acoustic pulse. Fixture transfer requires synchronized support torque and speed. Full acoustic, thermal or fracture attribution requires its own calibrated transfer measurement; a microphone amplitude or temperature change alone does not determine the corresponding work. Let $A_{\mathrm{out}}$ be the positive outward work magnitude obtained from independent signed channel integrals, and let $E_{\mathrm{ret}}\geq0$ be an independently evaluated retained store replacing the deleted coordinate. If the other event-side stores remain unchanged, the remaining residual is
\begin{equation}
 r_{E,e}=E_{\mathrm{ret}}-U_c(t_e^-)+A_{\mathrm{out}}.
 \label{eq:release-measurement}
\end{equation}
All additional measured store changes must be included if that continuity assumption fails. Apply the uncertainty enclosure in Appendix \ref{sec:residual-outcomes} to determine whether a deficit remains. The destination and criterion stay open when no such independent account is available; difficulty measuring them does not remove the problem.

For a finite observation window $[t_e-h_-,t_e+h_+]$, with positive $h_-,h_+$, record both event sides and integrate the regular drive, support and loss powers separately on each side. Retain contact transfers only in the corresponding subsystem accounts. A bound $|P_\ell|\leq M_\ell$ gives a work bound $M_\ell\delta t$ for an uncertain interval endpoint displaced by at most $\delta t$; a separately justified impulse retains its own uncertainty. Apply the state-error enclosure of Appendix \ref{sec:instrument-bounds} to the spring deflection and stiffness. Resolving $U_c(t_e^-)>0$ at torque zero is the first attainable outcome. A full destination account additionally requires retained-state changes and each outward channel; a measured temperature rise alone does not determine thermal work across the chosen boundary.

The first accessible comparison uses the slow torsional rig of Section \ref{sec:contact-identification}. Synchronized encoders give $\delta$ and its rate within the calibrated band; the torque transducer locates the zero-torque event. Independently calibrated contact stiffness and measured pre-release deformation determine $k_c\delta^2/2$. Resolve a positive lower bound on this store after propagating stiffness, angle and event-timing uncertainty, then follow retained deformation and torque–motion work through release. A support-transfer measurement additionally needs support torque and motion: a fixed support can exert torque while doing zero work.

## Restitution through more than one contact

Repeated contact tests whether the same release law can be reused with a new incoming state. The first recurrence below assumes a fresh contact state at every engagement; the retained-material alternative then shows which extra state must be carried through flight.

Write $e$ for the restitution coefficient of the selected law. The same release waveform repeated with incident velocity $v_n$ scales displacement and force by $v_n/v_0$ and each work by its square. If flight returns the same speed magnitude and the same contact law remains valid, then $v_n=e^{n-1}v_0$. For force-zero release,
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

\Needspace{20\baselineskip}

| Constitutive extension | Finite comparison and missing relation |
|:----------------------------|:-----------------------------------------------------------|
| Plasticity | Fix incident state and contact geometry; measure permanent deformation and its force history to identify the irreversible deformation law and retained store. |
| Adhesion | Compare a prescribed finite opening at fixed material condition; identify tensile force versus separation and its signed work. |
| Motor ripple | Hold the declared flight endpoints; compare synchronized drive torque and rate with the constant-acceleration work before attributing changed incident speed to contact memory. |
| Acoustic and thermal memory | Compare two flight durations at the same release state; retain material/fixture endpoints and integrate calibrated receiver channels on both windows. |
| Further engagements and geometry | Carry the measured strain and thermal state into a third contact, then change one gap, area or damping parameter while measuring the resulting contact law. |

: Separate finite dependencies for the wider repeated-contact question. The sliding law and retained-strain law provide explicit controls; the other relations must be identified before their work predictions are assigned.

The open release question is which constitutive gate and continuation reproduce the measured restitution, retained strain and receiver works at each engagement. A measured release residual from \eqref{eq:release-residual} remains signed and unresolved when those channels and their uncertainty do not account for it.

# What the measurements establish
\label{sec:measurement-conclusions}

The impact comparison separates identification of a local law from its physical interpretation. First declare the contact, joint, input, observation and preparation. Calibrate their component and sensor parameters, then predict independently specified changes with the same laws. The inverse in Section \ref{sec:contact-identification} is conditional on that constitutive family and informative observations. Refitting each configuration or frequency cannot establish transferability.

Different preparations can have identical terminal histories. Additional anvil motion can distinguish the contact example; internal branch voltages and strain distinguish the polarization and absorber controls in Appendix \ref{sec:identification}. The absorber's bounded normalized structural non-identifiability is a resolved result. Wider raw-unit identification and hardware inference retain their own assumptions. It would be incorrect to replace exact terminal ambiguity by invented different terminal predictions.

For two alternatives, retain all calibrated parameter and preparation uncertainty in their prediction sets. Discrimination requires disjoint error neighborhoods; nominally different curves alone are insufficient. Appendix \ref{sec:measurements} gives the exact separation budgets, correlation qualifications and finite observations for every retained question. Those budgets are requirements on a proposed comparison, not achieved instrument accuracies. The slow torsional rig carries the main impact comparison; a commercial tool requires separate correspondence and bandwidth calibration.

Signed work supplies a further comparison after the model and trajectory have been declared. Evaluate each endpoint store independently and integrate each port's signed effort--flow product over the same interval. If the resulting estimate is $\widehat r_E$ and its justified total uncertainty bound is $B_E$, the interval $[\widehat r_E-B_E,\widehat r_E+B_E]$ determines whether zero is compatible with that measured account. A wholly positive or negative interval retains an unresolved gain or deficit with its actual sign and event conditions. Appendix \ref{sec:uncertainty} derives the product and endpoint bounds; an omitted mechanism receives no post hoc allowance chosen to cover a remainder.

At contact release, retained material, prompt recipients and a changed constitutive release law require their own distinguishing observations. A terminal fit does not determine those destinations. The same principle governs the transformer attachments in Appendix \ref{sec:transformer} and the finite controllers in Appendix \ref{sec:transducer}: actual connections and supplies add physical states and transfers. The complete accounts remain with those models. No work outcome chooses the coefficient family, derivative order or event law.

# Conclusions

The rotary impact driver connects coefficient identification to a concrete release question. Hammer motion and contact torque can agree while anvil motion differs; an internal angle observation and independent joint/contact changes discriminate within the declared family. At torque-zero release, positive contact storage remains. Deleting it without an event port gives a negative residual. Retained material relaxation, prompt export and a changed release law predict different observations. The finite-window comparison must carry both event sides, independent receiver works and any preparation passed into the next engagement.

Choosing which physical law to identify, and at which attachment, makes these measurements a test of local coefficient synthesis. Held-engaged hammer/anvil phasors give an exact contact/joint inverse within the declared family and uncertainty bounds; impact events retain their separate preparation and validity conditions. Electrical admittance isolates a known parallel shunt, while moving it across a different boundary changes the predicted terminal response. Independent component changes test whether the same local laws predict the assembly.

The same distinction between observable response and complete physical state recurs in the other questions. Independent coordinates separate coefficient contributions; multi-device resonator acquisition tests transferability. Equal polarization time constants and a quiet RC terminal hide prepared stores. The finite-coupling bound requires a coupling lower bound or an independent preparation bound; multiple cancelling and nonideal modes retain a wider unresolved scope. The absorber's bounded structural result is resolved, while calibrated stress inference and wider physical models require their own observations.

Finite connections and supplies change the realized equations and their port accounts. Explicit ground and probe paths add capacitive states and signed works; one calibrated graph must predict both selected configurations before its hardware comparison is claimed. The growing constant-coupling plant, the regenerative receiving-coil control and the nonlinear bias-dependent supply are different models with separate endpoint and work predictions. A physical moving reference requires compensation sources, driver and rail states. Equal receiver endpoints or zero net receiver work do not determine their costs. Prepared singular limits and exact event certificates retain their stated laws and preparation domains.

These are the physical questions accompanying the constructions in [*Third- and Higher-Order ODEs*][main]. Their closure requires the declared independent observations, not a coefficient choice made from the energy result. Every work is integrated from its own effort and flow; endpoint stores come independently from component states. A measured residual interval wholly above or below zero remains an unresolved gain or deficit with its sign, magnitude, preparation, event conditions and completed checks. Exact model balances supply conditional predictions, not measured closure.

# Guide to the appendices {-}

The appendices retain the complete derivations, additional cases and physical accounts. Each can be entered from the corresponding result in the main text.

| Appendix | Complete treatment |
|:-------------------------|:----------------------------------------------------|
| Appendix \ref{app:observations} | Terminal identification and hidden preparations |
| Appendix \ref{app:correspondence} | Correspondence, preparation and connection paths |
| Appendix \ref{app:transformers} | Transformer attachments and signed work |
| Appendix \ref{app:controllers} | Controlled transducers and supplied references |
| Appendix \ref{app:implementation} | Finite implementations, events and service |
| Appendix \ref{app:measurement} | Measurement uncertainty, comparison guide and verification |

\clearpage
\appendix

# Terminal identification and hidden preparations
\label{app:observations}

These models establish which additional coordinates and observations distinguish coefficient laws, internal stores and stresses beyond the main impact comparison.

## What terminal observations identify
\label{sec:identification}

The physical comparisons require identified states, component laws and uncertainty. The following constructions distinguish recovery within a declared family from hidden preparation, insufficient resolution and acquisition of a missing physical law.

### Independent coordinates and correlated uncertainty
\label{sec:coefficient-identification}

The target coefficient must first be assigned to a declared local contact or joint law, or to a specified eliminated observation equation. State its derivative convention, normalization, physical input and measured response. Independently changing the selected component while keeping the surrounding model fixed tests that assignment; refitting every block after each change does not.

Let $a,b,c>0$ be inertial, damping and stiffness references. The dimensionally admissible coefficients
\begin{equation}
 A_{r,k}=a^{k-1+r}b^{2-k-2r}c^r
 =S\tau^k\rho^{-r},\quad S=b^2/a,\quad\tau=a/b,\quad\rho=b^2/(ac)
 \label{eq:coefficients}
\end{equation}
have the dimensions required to multiply the $k$th derivative. At fixed $\rho$, changing $r$ only rescales a column in coefficient identification. In a two-coordinate contact model a normalized coefficient can take the form
\begin{equation}
 B(\rho,\nu)=w_0+w_1\nu+w_2\nu^2/\rho.
 \label{eq:weak-coefficient}
\end{equation}
Here $B$ is the coefficient divided by its dimensional reference; $\nu>0$ is an independently varied damping ratio. Here $\nu=d_c/d_j=\eta^{-1}$, where the coefficient-synthesis article uses $\eta=d_j/d_c$; the reciprocal coordinate is explicit to prevent transferring powers with the wrong sign. Configuration III has $w=(1,1/100,1/2)$. The alternative $\widetilde w=(101/100,0,1/2)$ agrees at every point with $\nu=1$. At $(\rho,\nu)=(1,1),(4,1),(1,2)$, the design determinant is $3/4$ and the first model predicts $151/100,227/200,151/50$. The alternative predicts $301/100$ at the last point. Independent variation therefore creates an exact separation of $1/100$ there.

For two observations with variance $\sigma^2$ and correlation $\gamma$, the uncertainty variance of their difference is exactly $2\sigma^2(1-\gamma)$. More generally, a linear contrast $c^Ty$ has variance $c^T\Sigma c$, with the full spatial and temporal covariance $\Sigma$. These expressions follow by expanding the covariance of the sum; positive-definiteness requires $|\gamma|<1$ in the nonsingular two-channel case. With bounded contrast error $\epsilon$, predictions separated by $1/100$ have disjoint error intervals when $2\epsilon<1/100$. A covariance alone does not supply a deterministic bound without a distributional assumption.

This is a finite discrimination result for a declared support. A device may require another support or another observation operator. Calibration, coefficient estimation, model choice and the final independent condition must use separate information. The remaining question concerns realistic covariance and weak contributions on independently varied physical coordinates, not a change in energy when a coefficient becomes difficult to estimate.

The coordinates can be varied physically: choose $a=J_a$, $b=d_j$, $c=k_j$ and $\nu=d_c/d_j$. Holding $J_a=1\ \mathrm{kg\,m^2}$ and $d_j=1\ \mathrm{N\,m\,s/rad}$, configuration III's three settings require $(k_j,d_c)=(1,1),(1/4,1),(1,2)$ in their corresponding SI units. These knobs set the coordinates; the law \eqref{eq:weak-coefficient} remains a hypothesis about the inferred coefficient. For coefficient observations $b_1,b_2,b_3$ at the exact settings, matrix inversion yields
\begin{equation}
 w_1=-5b_1+4b_2+b_3,\qquad
 |\delta w_1|\leq5\epsilon_1+4\epsilon_2+\epsilon_3.
 \label{eq:coefficient-bound}
\end{equation}
Here $|\delta b_j|\leq\epsilon_j$. Equal candidate uncertainty intervals for $w_1=1/100$ and $0$ separate if the right-hand side is below $1/200$. With uncertain positive coordinates and positive candidate weights, the exact prediction interval has endpoints $w_0+w_1\nu_-+w_2\nu_-^2/\rho_+$ and $w_0+w_1\nu_++w_2\nu_+^2/\rho_-$. These component-calibration bounds enter before comparing coefficients; invertibility alone supplies no practical error bound.

The unresolved question is whether independent coordinates and realistic correlated uncertainty make the weak coefficient contributions identifiable. Interchangeable resistors and capacitors on an ordinary low-frequency circuit provide inexpensive independent parameter changes, while simultaneous voltage and current channels provide an empirical covariance estimate. Holding $\rho$ fixed supplies a deliberate null control; changing it independently of a second ratio can remove that particular proportionality. The chosen support and voltage/current observation map still require a full rank and uncertainty check. The first attainable result is separation of specified competing laws on independently chosen conditions. Recovering every weak contribution requires the stronger support-wide sensitivity condition; a complete physical account additionally needs the internal states and ports. Failure despite adequate sensitivity indicates an inadequate model or an incorrect uncertainty specification. Terminal measurements alone do not identify internal stresses.

### A shunt state and a transferable resonator law
\label{sec:resonator-identification}

A motional series branch $(R_m,L_m,C_m)$ in parallel with $C_0$ obeys, at complex frequency $s$,
\begin{equation}
 Y(s)=sC_0+\frac{sC_m}{L_mC_ms^2+R_mC_ms+1}.
 \label{eq:resonator}
\end{equation}
This follows from Kirchhoff's current law with common voltage $v$, motional current $i_m$, charge $q_m$, and state laws $\dot q_m=i_m$, $L_m\dot i_m=v-R_mi_m-q_m/C_m$, $i=C_0\dot v+i_m$. It is the conventional motional-plus-shunt description discussed by [Bible (2002)][bible]. A voltage-driven experiment prescribes the shunt voltage; a finite source impedance restores that capacitor as an independent state of the connected system.

The input-current channel observes total $i$, not motional $i_m$, and the voltage channel observes the common voltage at the two parallel terminals. Identifying the motional branch therefore needs its own current observation or subtraction of the independently calibrated shunt current. With that attachment fixed, choosing admittance exposes the local change exactly:
\begin{equation}
 Y_b-Y_a=s\Delta C_0,\qquad
 Z_b-Z_a=-s\Delta C_0 Z_aZ_b.
 \label{eq:shunt-identification}
\end{equation}
The second identity follows from $Z=1/Y$ where both ratios are defined. Reciprocation creates no independent data: transport the complex gain/phase uncertainty and common calibration errors through it. Near a zero, use the undivided voltage/current relation or the other defined ratio.

At $\omega_s=1/\sqrt{L_mC_m}$ the motional admittance is $1/R_m$, hence a changed shunt capacitance predicts $\Delta\operatorname{Im}Y=\omega_s\Delta C_0$. Configuration IV uses illustrative low-frequency values $R_m=1\ \Omega$, $L_m=1\ \mathrm H$, $C_m=1\ \mathrm F$, with $C_0=1$ or $2\ \mathrm F$. At $\omega_s=1\ \mathrm{rad/s}$, the two impedances are $(1-\ii)/2$ and $(1-2\ii)/5\ \Omega$. A series-only reading gives $1\ \Omega$ in both cases. These are exact component controls, not quartz parameter values.

For peak voltage $V$ at resonance over one period $T=2\pi/\omega_s$, separately integrating $vi$, $-R_mi_m^2$ and the shunt product $vC_0\dot v$ gives
\begin{equation}
 W_{\rm source}=\frac{TV^2}{2R_m},\qquad
 W_{R_m}=-\frac{TV^2}{2R_m},\qquad
 \int_0^T vC_0\dot v\,\dd t=0.
 \label{eq:rf-work}
\end{equation}
Each component returns to its initial periodic state, but its instantaneous store varies. At $V=1\ \mathrm V$ in configuration IV the source and loss works are $\pi$ and $-\pi\ \mathrm J$. The imaginary admittance, rather than the equal period work, distinguishes the shunts.

The open acquisition requires calibrated multi-device complex impedance and independent shunt variation, with synchronized internal/terminal traces where an internal claim is made. Twelve resonators and three fixture/component variants define an illustrative finite scope, not a statistically derived sample size. Shunt subtraction identifies $Y-sC_0$ for each device. Transferability requires a separately specified law predicting its $L_m,R_m,C_m$ from independently controlled device properties, calibrated on one set and evaluated on other declared devices and frequencies. No such law follows from the shunt control alone. Fixture compensation and RF current/voltage definitions follow [Keysight Technologies (n.d.)][keysight]; temperature, aging and nonlinear behavior require their own domain.

One device at fixed $\rho$ identifies only the combined coefficient at each $k$. Independent devices or controlled components are required to infer exponent dependence. The practical unresolved question is whether calibrated multi-device impedance measurements support a transferable coefficient law. A low-power VNA measurement of several resonators with independently varied shunt capacitance supplies an accessible complex observable and a controllable second coordinate. Fixture calibration and compensation are essential, as described by [Keysight (n.d.)][keysight]. The predicted alternatives are a common rational state model versus coefficients that change with fixture or amplitude. Such a measurement does not establish nonlinear, temperature or aging behavior, and no acquisition is asserted here.

#### Moving a shunt changes the synthesized system
\label{sec:shunt-location}

Use the same bare coil $Z_w=R+sL$, $R,L>0$, another linear series block $Z_e$ and capacitor $C_p>0$ in two connections. Hold the external drive and voltage/current measurement terminals fixed. A capacitor across the coil alone has local admittance $Z_w^{-1}+sC_p$; add $Z_e$ in series after taking its reciprocal. A capacitor across both blocks instead adds $sC_p$ to $(Z_e+Z_w)^{-1}$. Thus
\begin{equation}
 Z_{\rm local}=Z_e+\frac{Z_w}{1+sC_pZ_w},\qquad
 Z_{\rm whole}=\frac{Z_e+Z_w}{1+sC_p(Z_e+Z_w)}.
 \label{eq:shunt-location}
\end{equation}
This is a physical attachment change, independent of whether the final response is expressed as impedance or admittance. Voltage and current amplitudes and relative phase give its complex observable. Use an ordinary low-frequency RLC realization whose responses and fixture lie inside the calibrated band; any RF device needs its own bandwidth and loading assessment.

At $s=\ii\omega$ with finite, defined responses, exact components and absolute complex-response error bounds $\epsilon_{\rm local},\epsilon_{\rm whole}$, the prediction disks are disjoint if
\begin{equation}
 |Z_{\rm local}-Z_{\rm whole}|>
       \epsilon_{\rm local}+\epsilon_{\rm whole}.
 \label{eq:shunt-location-separation}
\end{equation}
This is the triangle-inequality separation condition, not a claim that the two placements separate at every frequency. Component and fixture uncertainty enlarge the prediction sets; shared calibration errors require the joint comparison of Appendix \ref{sec:coefficient-identification}. If they overlap, another frequency, an independent component change or a local voltage/current channel can supply information. Conditions used to estimate the law remain separate from those used to test its prediction. Period work is still the separately integrated physical product; it does not choose a placement or a coefficient.

### Hidden prepared energy under finite coupling
\label{sec:hidden-coupling}

Place a series RC branch behind an ideal transformer with secondary-to-primary voltage ratio $\nu>0$, and add a terminal conductance $G_{0}>0$. Orient primary branch current into the transformer and secondary current $j$ toward the RC load, so that $v_s=\nu v_p$ and $i_{p,\mathrm{branch}}=\nu j$. For capacitor voltage $x$, the initialized realization is
\begin{equation}
 j=\frac{\nu v_p-x}{R},\qquad C\dot x=j,\qquad
 i_p=G_0v_p+\nu j,\qquad R,C>0.
 \label{eq:hidden-rc-state}
\end{equation}
Eliminating $x$ with zero initial state gives the admittance
\begin{equation}
 Y(s)=G_{0}+\frac{\nu^2sC}{1+sRC},\qquad
 h=\frac{\nu^2}{R},\qquad \delta_{h}=\frac h{G_{0}+h}.
 \label{eq:hidden-rc}
\end{equation}
For $x(0)=V_0$, the terminal current additionally contains $-\nu V_0e^{-t/(RC)}/R$. The poles and initialized response therefore follow from the same orientation. With primary-to-secondary ratio $n=1/\nu$, reflecting a fixed secondary admittance divides it by $n^2$.

As $\nu\to0$, both the driven branch contribution and its terminal initial-state signal vanish. The endpoint of \eqref{eq:hidden-rc-state} is a decoupled terminal with a closed internal RC discharge loop, not an ordinary finite-turns transformer. An open series RC branch would not have the same discharge. Enclose the capacitor and exclude the two heat reservoirs: the inward powers are $v_pi_p$, $-G_0v_p^2$, and $-Rj^2$. Integrating them separately gives their sum $\int_0^T xj\,\dd t=C[x(T)^2-x(0)^2]/2$, agreeing with the independently evaluated store $Cx^2/2$. In the decoupled endpoint with $v_p=0$, the sole nonzero transfer and endpoint store are
\begin{equation}
 W_{R}(0,T)=-\int_{0}^T\frac{V_{0}^2e^{-2t/(RC)}}R\,\dd t
 =-\frac{CV_{0}^2}{2}(1-e^{-2T/(RC)}),\quad
 E(T)=\frac{CV_{0}^2}{2}e^{-2T/(RC)}.
 \label{eq:hidden-discharge}
\end{equation}
Exact terminal cancellation therefore does not imply absence of an internal prepared mode. The changing store in \eqref{eq:hidden-discharge} is accounted for by the independently integrated resistor work, even though the terminal work is zero. Its relevance to a higher-order realization is that eliminated internal coordinates can carry the same hidden change.

#### Measuring a changing store behind a quiet terminal
\label{sec:hidden-measurement}

How tightly can terminal uncertainty bound hidden prepared energy when coupling and preparation are only partly known? With $v_p=0$, known finite $\nu>0$ and the state law \eqref{eq:hidden-rc-state},
\begin{equation}
 |i_p(0)|=\frac{\nu|V_0|}{R},\qquad E(0)=\frac{CV_0^2}{2},\qquad
 |i_p(0)|\leq\epsilon_i\quad\Longrightarrow\quad
 E(0)\leq\frac{CR^2\epsilon_i^2}{2\nu^2}.
 \label{eq:hidden-energy-bound}
\end{equation}
Here $\epsilon_i$ bounds the true initial current after calibration and timing uncertainty, not merely the displayed reading. The bound follows by eliminating $|V_0|$. If $C\leq C_{\max}$, $R\leq R_{\max}$ and $\nu\geq\nu_{\min}>0$, the corresponding bound is $C_{\max}R_{\max}^2\epsilon_i^2/(2\nu_{\min}^2)$. Without a positive coupling lower bound or an independent preparation bound, there is no uniform finite ceiling: choosing $|V_0|=R\epsilon_i/\nu$ preserves the terminal limit while the store grows as $\nu^{-2}$. Those arbitrarily large states belong to the ideal parameter family; finite voltage and preparation limits must be supplied for an actual device.

A low-voltage RC branch with an independently calibrated finite coupling permits ordinary capacitor-voltage, resistor-voltage/current and terminal-current measurements. Prepare a specified $V_0$, establish the operation-side state after switching, and observe a finite interval $[0,T]$ with $v_p=0$. For the boundary enclosing the capacitor and ideal coupling, source work is zero and the resistor power is $-v_Rj=-Rj^2$. Integrating it gives \eqref{eq:hidden-discharge}; evaluate $CV_0^2/2$ and $Cx(T)^2/2$ independently from the endpoint voltages. The exact residual is zero for this declared discharge. A measured residual exceeding its independently bounded uncertainty remains open, while a resolved capacitor change with an unresolved terminal signal establishes the narrower hidden-state result. Probe loading supplies an additional port if it is appreciable in the declared model.

The equal-and-opposite polarization preparation in Appendix \ref{sec:polarization} offers a low-frequency emulator of terminal cancellation with separately accessible stores. Multiple nearly cancelling modes, nonideal transformers, preparation limits, sensor loading and finite observation bandwidth still need bounds. A resolved single-branch account does not close those broader questions.

#### A three-state loop with a directly measurable hidden store
\label{sec:hidden-loop}

A closed loop containing an inductor, a series resistance $R_\Sigma\geq0$ and two series-connected parallel RC sections gives a direct control for that observation question. With identical $R,C>0$, no applied voltage and consistently oriented section voltages,
\begin{equation}
 L\dot i=-R_\Sigma i-v_1-v_2,\qquad
 C\dot v_j=i-v_j/R,\quad j=1,2.
 \label{eq:hidden-loop-state}
\end{equation}
The compatible preparation and exact response are
\begin{equation}
 (i(0),v_1(0),v_2(0))=(0,V_0,-V_0),\qquad
 i=0,\quad v_1=V_0e^{-t/(RC)},\quad v_2=-V_0e^{-t/(RC)}.
 \label{eq:hidden-loop-motion}
\end{equation}
There are three independent physical states. The driven pair $(i,v_1+v_2)$ has two states; $v_1-v_2$ relaxes independently and is absent from the loop-current transfer. A branch-voltage observation generally retains all three initialized modes. Unequal time constants couple the difference back to the terminal observation. Thus a quiet terminal does not remove the third state.

Enclose the inductor and both capacitors, excluding heat reservoirs, on the smooth operating interval $[0,T]$. The separate inward resistor powers are $-R_\Sigma i^2$ and $-v_jj_{R,j}$, where $j_{R,j}=v_j/R$. Direct integration and independent endpoint evaluation give
\begin{align}
 W_\Sigma&=0,&
 W_{R,j}&=-\int_0^T\frac{v_j^2}{R}\,\dd t
 =-\frac{CV_0^2}{2}(1-e^{-2T/(RC)}),\nonumber\\
 E_0&=CV_0^2,& E_1&=CV_0^2e^{-2T/(RC)},\nonumber\\
 r_E&=E_1-E_0-W_\Sigma-W_{R,1}-W_{R,2}=0.
 \label{eq:hidden-loop-work}
\end{align}
The two nonzero works and decreasing stores are invisible to a terminal-only account. This exact model resolves their destination; it does not report an unexplained gain. Preparation is a separate interval. Closing the loop at zero inductor current with continuous capacitor voltages has no impulse under these laws; actual switch and probe transfers need their own account.

For the illustrative component choices $R=1\ \mathrm{k}\Omega$, $C=1\ \mathrm{mF}$, $V_0=1\ \mathrm V$, and $T=1\ \mathrm s$, the initial store is $1/1000\ \mathrm J$ and each resistor work is $-(1-e^{-2})/2000\ \mathrm J$. Ordinary voltage channels and shunt-current measurements resolve the internal volt and milliampere scales over seconds. The open experimental alternatives are a resolved internal change with unresolved terminal signal, an independently closed resistor account, or a signed residual beyond the declared resolution. Only the last leaves the energy account unresolved.

An assumed calibration budget makes that distinction quantitative. Take capacitance estimates $\widehat C=1/1000\ \mathrm F$ with bounds $\epsilon_C=1/100000\ \mathrm F$, voltage error $\epsilon_v=1/1000\ \mathrm V$, resistor-current error $\epsilon_j=1/10^6\ \mathrm A$, and observed bounds $|\widehat v_j|\leq11/10\ \mathrm V$, $|\widehat j_{R,j}|\leq11/10000\ \mathrm A$ throughout the one-second interval. The channel and endpoint formulas in Appendix \ref{sec:instrument-bounds} give
\begin{equation}
 \epsilon_{\mathrm{cap}+R}
 =\frac{1652401}{50000000000}\ \mathrm J
 <\frac1{25000}\ \mathrm J,\qquad
 \epsilon_r\leq\epsilon_{\mathrm{cap}+R}+\epsilon_{\mathrm{rest}}.
 \label{eq:hidden-loop-resolution}
\end{equation}
This is the sum of four capacitor endpoint bounds and two resistor-work bounds, not an achieved apparatus specification. The independently determined $\epsilon_{\mathrm{rest}}$ must cover inductor endpoints, series-resistance work, timing, acquisition integration, probe loading and any event account. Terminal quietness does not set it to zero. Compare the predicted capacitor decrease $(1-e^{-2})/1000\ \mathrm J$ with its endpoint error, and compare the measured full residual with its separate total error. Deliberately unequal relaxation times provide the contrasting observation derived in \eqref{eq:polarization-separation}.

### Polarization preparations invisible at the terminal
\label{sec:polarization}

A coil feeding a polarization emulator has states $i,v_1,\ldots,v_N$ and equations
\begin{equation}
 L\dot i+R_\Sigma i+V_{\rm oc}+\sum_jv_j=0,
 \qquad C_j\dot v_j=i-v_j/R_j.
 \label{eq:polarization}
\end{equation}
Positive $i$ enters the emulator. A conducting interval ends at a downward current zero. For distinct active time constants $\tau_j=R_jC_j$, eliminating the branches gives generic order $N+1$ for $i$, while equal time constants combine at that observation. The storage boundary includes the coil and branch capacitors. Its external powers are $-V_{\rm oc}i$, $-R_\Sigma i^2$ and the separately retained $-v_j^2/R_j$; the DC source and all heat reservoirs are outside.

A permanently opened connection after the cutoff $t_c$ gives independent branch relaxation. A retained diode permits that same continuation only while its blocking condition holds:
\begin{equation}
 i=0,\qquad v_j(t)=v_j(t_c)e^{-(t-t_c)/\tau_j},\qquad
 V_{\rm off}(t)=V_{\rm oc}+\sum_jv_j(t_c)e^{-(t-t_c)/\tau_j}\geq0.
 \label{eq:polarization-blocking}
\end{equation}
Nonnegative branch voltages at cutoff suffice for continued blocking when $V_{\rm oc}\geq0$. Signed preparations can instead restart conduction. Let $V_{\rm oc}=V_b>0$, $(v_1(t_c),v_2(t_c))=(8V_b,-8V_b)$ and $(\tau_1,\tau_2)=(T_b,2T_b)$, with $T_b>0$. For $\vartheta=(t-t_c)/T_b$, the candidate blocked voltage is $V_b(1+8e^{-\vartheta}-8e^{-\vartheta/2})$. Setting $z=e^{-\vartheta/2}$ gives $1+8z^2-8z=0$ and the first crossing
\begin{equation}
 t_r-t_c=-2T_b\log\!\left(\frac{2+\sqrt2}{4}\right).
 \label{eq:polarization-restart}
\end{equation}
The derivative at this root is negative; continuation to $\vartheta=2\log2$ would give $V_{\rm off}=-V_b$. The cutoff itself is locally attainable from positive current because the conducting derivative there is $-V_b/L<0$. At the later guard failure the conducting equations resume from continuous branch voltages and $i=0$; once $V_{\rm off}<0$, $L\dot i=-V_{\rm off}>0$. A tangency that leaves the guard nonnegative does not restart conduction.

On an opened interval, or a blocked interval ending before guard failure, branch $j$ has signed resistor work $-C_jv_j(t_c)^2[1-e^{-2(T-t_c)/\tau_j}]/2$ and independently evaluated final store $C_jv_j(t_c)^2e^{-2(T-t_c)/\tau_j}/2$. A resumed conducting interval requires its own source, coil and branch integrals. The isolated comparison below deliberately opens the external path, so its observation interval is independent of the diode guard.

Each local branch law $C_j\dot v_j+v_j/R_j=i$ identifies a parallel RC block; the loop adds its voltage to those of the other series-connected blocks. Independently calibrated $R_j,C_j$ and branch-voltage observations specify the local information before composition. The recurrence in [*Third- and Higher-Order ODEs*][main] then predicts the complete current and forcing operators without refitting unaffected branches. A terminal fit alone need not assign a pole to an individual branch, and compatible prepared states remain necessary even after the terminal transfer is reduced.

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

Recovering order from noisy data with arbitrary branch preparations remains a practical open question. A low-voltage battery emulator made from a DC source and independently accessible RC branches allows ordinary shunt-current and capacitor-voltage measurements without uncertain electrochemistry. Prepare equal and opposite voltages on equal-time-constant branches: the terminal transient is unchanged while branch probes reveal relaxation. Split their time constants controllably and compare the uncertainty-scaled sensitivity with the covariance-weighted observation sensitivity. This distinguishes exact hidden freedom from inadequate resolution. It does not validate an actual battery's temperature- and age-dependent spectrum.

### Terminal reaction and internal absorber stress
\label{sec:absorber-identification}

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

# Correspondence, preparation and connection paths
\label{app:correspondence}

These complete controls follow physical correspondence through preparation and switching, retaining the finite paths and separate signed works.

## Damped correspondence through preparation and reset
\label{sec:analogy}

### A damped correspondence with a complete finite path

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

A distinct low-damping control sets $m=k=L=C=1$ in their SI units and $d=R=1/5$. The constant efforts $+1,0,-1$ on consecutive one-second intervals from zero preparation give exact states by composing $e^{Ft}$ and $\int e^{F(t-s)}b u\,\mathrm ds$, where $F=\left(\begin{smallmatrix}0&1\\-1&-1/5\end{smallmatrix}\right)$ and $b=(0,1)^T$. Each interval separately integrates $u\dot x$ and $-\dot x^2/5$, and evaluates $(x^2+\dot x^2)/2$ at both endpoints. The final state is retained; this finite opposite drive is not an exact reset. The electrical map with unit work scale carries the same three intervals and every individual port.

On a separate preparation interval $[-1,0]\ \mathrm s$, put $r=t+1$ and prescribe $x=3(r^3-r^2)/10\ \mathrm m$. The required force is $\ddot x+\dot x/5+x$. Independent polynomial integration gives source work $237/5000\ \mathrm J$, dashpot export $-3/1250\ \mathrm J$ and final kinetic store $9/200\ \mathrm J$, with $x(0)=0$, $\dot x(0)=3/10\ \mathrm{m/s}$. A change of observer coordinates supplies none of this work. This is a forced preparation of the declared oscillator, not a measured contact or a universal common-motion law.

## Prepared states and singular passive reductions
\label{sec:singular}

### Derive the constrained topology before its limit

A concrete passive two-store network consists of $R_C\parallel C$ in series with $R_L\parallel L$. Its terminal impedance is
\begin{equation}
 Z(s)=\frac{R_C}{1+sR_CC}+\frac{sLR_L}{R_L+sL}.
 \label{eq:passive-network}
\end{equation}
Kirchhoff's laws give branch states $C\dot v_C=i-v_C/R_C$ and $L\dot i_L=R_L(i-i_L)$. The branch terminal voltages are $v_C$ and $R_L(i-i_L)$. Thus the boundary of the capacitor and inductor has input power $[v_C+R_L(i-i_L)]i$, two separate resistor powers $-v_C^2/R_C$ and $-R_L(i-i_L)^2$, and store $Cv_C^2/2+Li_L^2/2$.

Setting $C=0$ in the branch equations first yields $v_C=R_Ci$; it does not permit an independent initial $v_C$. Setting $L=0$ imposes zero winding voltage; $L\to\infty$ at bounded voltage instead freezes the current over a finite interval and does not remove its preparation. The exact finite components must decide what happens to an incompatible state.

For an illustrative dimensionless evaluation with $R_C=R_L=L=1$, $C=\epsilon$ and $s=1$, \eqref{eq:passive-network} is $1/(1+\epsilon)+1/2\to3/2$. Along $R_C=C=\epsilon$, it is $\epsilon/(1+\epsilon^2)+1/2\to1/2$. At $\epsilon=1/4$, the exact values are $13/10$ and $25/34$. The units are restored with fixed resistance and time scales. These transfer limits follow from different physical families; neither computes an event work.

### A finite prepared family with vanishing charge

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

## Equal endpoints with unequal switch work
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

## Closed work integrals for a finite linear connection
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

## Charge observations, finite reconnection and reset order
\label{sec:charge-reconnection}

An exact two-cell control distinguishes charge magnitude from stored energy. With $C_1=1\ \mathrm F$, $C_2=19\ \mathrm F$, $L=20/19\ \mathrm H$, currents positive from cell 1 to cell 2, $\dot q_1=-i$, $\dot q_2=i$, $L\dot i=q_1/C_1-q_2/C_2$. Starting at $(q_1,q_2,i)=(10,0,0)$ in SI units gives
$$
 q_1=\tfrac12+\tfrac{19}2\cos t,\quad q_2=\tfrac{19}2(1-\cos t),\quad i=\tfrac{19}2\sin t.
$$
On $[0,\pi]\ \mathrm s$, the absolute charge sum rises from $10$ to $28\ \mathrm C$. Independently evaluated initial component stores are $(50,0,0)\ \mathrm J$ and final stores $(81/2,19/2,0)\ \mathrm J$. The separate powers $-(q_1/C_1)i$, $(q_2/C_2)i$, $(q_1/C_1-q_2/C_2)i$ integrate to $-19/2,19/2,0\ \mathrm J$. There is no external port or switching impulse. For a single isolated LC pair the analogous half-cycle reverses capacitor charge with zero net capacitor and inductor work over that full half-cycle, while the first quarter-cycle transfers $Cv_0^2/2$ between their stores. Detachment at nonzero current requires another event law.

Isolated parallel resistive exchange instead gives $Q=q_1+q_2$ constant, $\delta=v_1-v_2=\delta_0e^{-t/(RC_*)}$, $C_*=C_1C_2/(C_1+C_2)$, and
$$
 q_1=\frac{C_1(Q+C_2\delta)}{C_1+C_2},\quad
 q_2=\frac{C_2(Q-C_1\delta)}{C_1+C_2},\quad
 E_C=\frac{Q^2}{2(C_1+C_2)}+\frac{C_*\delta^2}{2}.
$$
The absolute sum is constant for equal signs and has derivative $-2|\delta|/R$ for opposite signs, with nonpositive one-sided derivatives at zeros. The resistor exports $-C_*\delta_0^2(1-e^{-2T/(RC_*)})/2$. If a receiver and switch resistor are in series, each receives its own fraction $R_j/(R_L+R_s)$ of this released store. With $C_1=1$, $C_2=2$, $R_L=R_s=1$, $\delta_0=1$, $T=1$ in SI units, each heat is $(1-e^{-3/2})/6\ \mathrm J$.

For two equal series cells and a receiver $R$, $s=v_1+v_2$ obeys $\dot s=-2s/(RC)$, while $\delta=v_1-v_2$ is constant. Unit $R,C$ and preparations $(1,1)$ and $(3,-1)\ \mathrm V$ give the same terminal voltage and current $2e^{-2t}$ in their SI units, but initial stores $1,5\ \mathrm J$. On $[0,1/4]\ \mathrm s$ each receiver work into the cell boundary is $-1+e^{-1}\ \mathrm J$ and final stores are $e^{-1},4+e^{-1}\ \mathrm J$. Thus this topology has an exact hidden preparation; terminal ambiguity is not a claim that reconnecting it leaves observations unchanged.

### Noncommuting states and commuting work partitions

For three grounded $1\ \mathrm F$ cells, let a $1\ \Omega$ edge act on cells 1--2 (A) or 2--3 (B). Each acts for $\log2/2\ \mathrm s$. Its state law is $\dot q=-aa^Tq$, with $a=(1,-1,0)^T$ or $(0,1,-1)^T$, and maps
$$
 M_A=\begin{pmatrix}3/4&1/4&0\\1/4&3/4&0\\0&0&1\end{pmatrix},\qquad
 M_B=\begin{pmatrix}1&0&0\\0&3/4&1/4\\0&1/4&3/4\end{pmatrix}.
$$
Starting from $(1,0,-1)\ \mathrm C$, A then B ends at $(3/4,-1/16,-11/16)\ \mathrm C$; B then A ends at $(11/16,1/16,-3/4)\ \mathrm C$. The maps do not commute. Independently integrating $(a^Tq)^2/(1\ \Omega)$ gives first-channel heat $3/16\ \mathrm J$ and second-channel heat $75/256\ \mathrm J$ in either order, while the channel identities exchange. Initial and final stores are $1$ and $133/256\ \mathrm J$; total heat is $123/256\ \mathrm J$. States are continuous at connection changes, without impulses.

This differs from the scalar two-cell reset. Starting at $(1,-1)\ \mathrm V$, either of two identical channels acts as $\dot v=-v/(1\ \mathrm s)$ for $\log2\ \mathrm s$; each channel shunts both cells with its stated unit resistors. Both orders end at $(1/4,-1/4)\ \mathrm V$. First and second channel heats are $3/4$ and $3/16\ \mathrm J$, with final store $1/16\ \mathrm J$. Scalar endpoint maps commute while separate channel works depend on order. Neither example proves a universal instantaneous partition.

### A finite shunt with complete sign coverage
\label{sec:finite-shunt-certificate}

Retain the first LC graph on $[0,2]\ \mathrm s$ and connect a $1\ \Omega$ shunt across cell 1 only on $[\pi/2,\pi/2+1/10]\ \mathrm s$. Let $g=1\ \mathrm S$ there and zero elsewhere. The laws are $\dot q_1=-i-gq_1/C_1$, $\dot q_2=i$, $L\dot i=q_1/C_1-q_2/C_2$. The invariant $q_1+q_2$ applies only when $g=0$; during the edge its derivative is $-q_1/(1\ \mathrm s)$. The candidate $q_1-q_2$ is not invariant. Physical cell orientations never change.

The reactive store obeys $\dot E=-g(q_1/C_1)^2$. Integrate that shunt export separately on each interval and evaluate all three store endpoints. If heat is retained, add its positive integral as a caloric store and remove the exported port. Reactive states remain continuous and modeled impulses zero. For the energized preparation $E\leq50\ \mathrm J$, weighted Cauchy--Schwarz gives $A_q^2\leq2(C_1+C_2)E_C\leq2000\ \mathrm{C^2}$. The separately admitted zero preparation stays zero.

The sign certificate covers every time. Before the edge, $q_1,q_2>0$ apart from the initial tangency $q_2(0)=0$, and $A_q=10\ \mathrm C$. The store bound gives $|q_1|\leq10$, $|q_2|<44$, $|i|<10$ in SI units, hence $|\dot i|<117/10\ \mathrm{A/s}$. Throughout the edge $i>833/100\ \mathrm A$ and $q_1>-3/2\ \mathrm C$. Until the first zero, $-21/2\ \mathrm{A}\leq\dot q_1<-833/100\ \mathrm A$ because $0\leq q_1\leq1/2\ \mathrm C$. The unique zero therefore lies strictly between $\pi/2+1/21$ and $\pi/2+1/16\ \mathrm s$. It cannot recross: at a zero $\dot q_1=-i<0$. Before it $\dot A_q=-q_1/(1\ \mathrm s)<0$; after it $\dot A_q=2i+q_1/(1\ \mathrm s)>379/25\ \mathrm A$. After opening, $i>22/5\ \mathrm A$ up to $2\ \mathrm s$, so $q_1<0$, $q_2>0$ and $\dot A_q=2i>0$. At edge entry the one-sided magnitude derivatives are $0$ and $-1/2\ \mathrm A$; at exit both are positive. The charge zero is a cusp minimum, not a tangency. This proves the sign count and the stated loose magnitude bound for this graph and these two preparations; it establishes no universal multiplication factor or hardware bound.

### Finite preparation and a loaded binary probe
\label{sec:finite-bank-probe}

A distinct finite graph resolves a bounded binary preparation question conditionally on its observation separation. Let node order be $(A,T,X_1,Y_1,X_2,Y_2)$ relative to a secondary return. Unit cells join $X_1-Y_1$ and $X_2-Y_2$; each node has $1/50\ \mathrm F$ parasitic. Three winding currents have
$$
 L=\begin{pmatrix}1&1/4&1/4\\1/4&1/4&1/8\\1/4&1/8&1/4\end{pmatrix}\mathrm H,
 \quad R=\operatorname{diag}(1/4,1/20,1/20)\ \Omega.
$$
The first winding is driven through its physical primary return with zero operating voltage; secondary incidence columns are $e_A-e_T,e_T$, and the primary column is zero. The source resistor is $1/5\ \Omega$, each copper resistor $1/20\ \Omega$. A unit receiver joins $X_1-Y_2$. Six finite connections join $A-X_1,T-X_1,X_1-X_2,Y_1-Y_2,Y_1-X_2,X_1-Y_1$. The first five vary between $1/10000$ and $20\ \mathrm S$; the last is the cell probe, between $1/1000000$ and $1/10\ \mathrm S$. Each contributes its incidence outer product to $G(t)$.

Use the electrical equations $L\dot i=B^Tv-Ri$, $C\dot v=-Bi-G(t)v-K^Ti_c(Kv)$, where $C=(1/50\ \mathrm F)I+(1\ \mathrm F)(a_1a_1^T+a_2a_2^T)$ and $a_j$ are cell incidences. Clamps on $A,T$ and both cells have threshold $4\ \mathrm V$ and slope $5\ \mathrm S$. The series command is $(0,0,0,0,1,0)$ through $1/4\ \mathrm s$, followed by $(0,0,1,1,0,1)$. Interpolate the conductance commands with $3r^2-2r^3$ across each $1/100\ \mathrm s$ edge; the first series connection rises from all-off on $[0,1/100]$. At $t=1\ \mathrm s$ commands turn off and $1/5\ \mathrm S$ node bleeders act through $t=2\ \mathrm s$. Each of six independent driver supplies feeds a $1/10000\ \mathrm F$ gate through $20\ \Omega$; these driver states and their powers are retained. The prescribed conductance law is not inferred from the separate gate voltage. That actuation relation remains a physical implementation question.

Prepare the node vectors $v^{(0)}=(0,0,2,1,1,0)$ and $v^{(1)}=(0,0,2,-1,-1,0)\ \mathrm V$, with zero winding currents and gates. Their cell stores are $1,5\ \mathrm J$ and each parasitic store is $3/50\ \mathrm J$. On $[-1,0]\ \mathrm s$, disconnect winding/selectors and use six independent unit-resistance chargers from zero voltage. With dimensional units understood, the constant source vector is $u_p=(I-e^{-C^{-1}})^{-1}v^{(j)}$ and $v(t)=(I-e^{-(t+1)C^{-1}})u_p$. Integrate each $u_{p,k}(u_{p,k}-v_k)$ and each negative resistor heat separately. Heat obeys $\dot H=P_{\rm heat}-H/(2\ \mathrm s)$, so its exact endpoint is the exponentially weighted heat integral; retain it at connection. The two thermal preparations need not agree.

The probe draws its actual conductance current and has a declared readout filter $\tau_f\dot y=a_1^Tv-y$, $\tau_f=1/50\ \mathrm s$, $y(0)=0$. This filter is an observation law; only the specified resistor is a physical load in this graph. Its electronics supply and realization are not established. In the inactive-clamp domain the complete observation has the time-ordered ten-coordinate map $y(t)=e_{10}^T\Phi(t,0)(i_0,v_0,0)^T$, including finite edges. The ideal series null is not transferred to this graph: finite off paths leak the hidden difference. A continuous pre-switch bound is
$$
 |\delta v_L(t)|\leq t\sqrt{c_L^TC^{-1}c_L}
 \sqrt{(G_{\rm off}d)^TC^{-1}(G_{\rm off}d)},\quad
 d=v^{(1)}-v^{(0)},\quad c_L=e_{X_1}-e_{Y_2}.
$$
It follows from passive incremental contraction and the Duhamel forcing of the formerly constant null direction. The preparation and topology, not a sampled terminal match, determine this bound.

At $t=7/20\ \mathrm s$, define the exact predicted gap $\Delta_y=|e_{10}^T\Phi(t,0)(0,d,0)^T|$. A midpoint classifier identifies which of the two known cell energies was prepared whenever $\Delta_y>1/10\ \mathrm V$ and each complete observation error is at most $1/20\ \mathrm V$. It then meets a $1/100\ \mathrm J$ binary target. This is an exact conditional criterion; a floating evaluation of $\Phi$ is not a certified continuous error enclosure. For cell/readout magnitude below $4\ \mathrm V$, gain error $1/100000$, offset and sample errors each $1/1000\ \mathrm V$, timing error $10^{-8}\ \mathrm s$ and filter-time error $10^{-7}\ \mathrm s$ contribute at most $4/100000+2/1000+400(10^{-8}+10^{-7})\ \mathrm V$; any map-evaluation/model allowance must also fit the budget. Arbitrary unknown states, sign recovery and hardware calibration are separate questions.

For both paths, integrate receiver, probe, every selector, clamp, copper, bleeder, gate supply, gate resistor and bath power on the same intervals, plus the six preparation sources. The reactive boundary exports resistor heat; the retained-thermal boundary includes it internally and exports receiver/probe/bath work. The probe's loading changes receiver work and endpoints and cannot be removed after evaluating its signal. The difference in receiver work is exactly $-\int_0^2[(c_L^Tv^{(1)}(t))^2-(c_L^Tv^{(0)}(t))^2]/(1\ \Omega)\,dt$, without a sign inferred from initial energy. Finite bleeder operation retains actual final stores. Neither the binary criterion nor paired finite works establishes exact reset or complete-service ranking.

## Four accessible ports and a finite compliant correspondence
\label{sec:four-terminal}

A loaded auxiliary shaft or terminal changes the attachment equations. Four accessible shafts do not supply four independent speeds. For positive teeth $Z_s,Z_p,Z_r$, with $Z_r=Z_s+2Z_p$, bilateral pitch constraints give
\begin{equation}
 \omega=\mathsf B\binom{u}{d},\qquad
 \mathsf B=\begin{pmatrix}1&1\\1&0\\1&-Z_s/Z_r\\1&-Z_s/Z_p\end{pmatrix},
 \quad u=\omega_c,\quad d=\omega_s-\omega_c.
 \label{eq:four-shaft-constraint}
\end{equation}
The shaft order is sun, carrier, ring, planet output. The output must attach to the rotating planet body, not its carrier-fixed bearing pin. The sun/carrier minor is nonzero. Absolute speed zeros are $u+d=0$, $u=0$, $Z_ru-Z_sd=0$, $Z_pu-Z_sd=0$; all six relative-speed zeros reduce to $d=0$. These statements include stationary and reversed shafts.

For a massless correctly phased leadout, steady axial free bodies give
$$
 \tau_r=(Z_r/Z_s)\tau_s-(Z_r/Z_p)\tau_o,\qquad
 \tau_c=-(1+Z_r/Z_s)\tau_s+(Z_r/Z_p-1)\tau_o,
 \qquad \mathsf B^T\tau=0.
$$
This follows from the sun and ring tangential forces, planet spin and carrier pin reaction, before any power sum. In dynamics the right side becomes $\mathsf B^T\mathsf M\mathsf B(\dot u,\dot d)^T$. For unit effective inertias and teeth $(24,18,60)$, $u=1+t$, $d=5/2+60t/11$ gives $\alpha=\tau=(71/11,1,-13/11,-69/11)$ in consistent SI units. Their torque sum is zero while all shafts accelerate. Each one-second work is $\tau_j\omega_j(0)+\tau_j\alpha_j/2$; independent kinetic endpoints give their sum. A zero total torque is not a zero-acceleration test.

### Physical returns and the loaded ideal law

Set $(V_j-V_O)=\alpha_v\omega_j$, $I_j=\tau_j/\alpha_v$ with $\alpha_v$ in $\mathrm{V\,s/rad}$. The reference $O$ is a physical external return. For $h_s=-Z_p/Z_s$, $h_r=Z_p/Z_r$, two ideal pairs give
\begin{align}
 V_S-V_C&=h_s(V_P-V_C),&V_R-V_C&=h_r(V_P-V_C),\\
 j_s&=-h_sI_S,&j_r&=-h_rI_R,\\
 I_P&=j_s+j_r,&I_C&=-(I_S+I_R+I_P).
 \label{eq:four-terminal-law}
\end{align}
Each winding's other endpoint is $C$; each external complete port returns to $O$. Only the unloaded case has $j_s+j_r=0$. Translating all voltages including $V_O$ changes coordinates; moving a physical return from $O$ to $C$ changes the experiment.

A common-flux ideal realization has raw taps $(S,C,R,P)=(Z_r(Z_s+Z_p),Z_sZ_r,Z_s(Z_r-Z_p),0)$. At the reference teeth they reduce to $(35,20,14,0)$, with section lengths $(15,6,14)$ from $S$ toward $P$. The actual section currents are $I_S$, $I_S+I_C$, $I_S+I_C+I_R=-I_P$. Thus its independent constraints are $35I_S+20I_C+14I_R=0$ and KCL, with voltages relative to $P$ proportional to the taps. Substituting KCL proves \eqref{eq:four-terminal-law}, including the zero-voltage case without dividing by a rate. Each constraint matrix has rank two. Multiplying all turns by the same positive integer preserves this ideal terminal relation but changes finite magnetic and geometric parameters. It does not identify the internal states of one core with those of two pairs.

With $O=0$, $\alpha_v=1\ \mathrm{V\,s/rad}$, constant voltages $(7/2,1,0,-7/3)\ \mathrm V$ and $I_S=2\ \mathrm A$, the exact controls are

| $I_P$ ($\mathrm A$) | $(I_S,I_C,I_R,I_P)$ ($\mathrm A$) | Separate one-second works ($\mathrm J$) |
|---|---|---|
| $0$ | $(2,-7,5,0)$ | $(7,-7,0,0)$ |
| $1$ | $(2,-14/3,5/3,1)$ | $(7,-14/3,0,-7/3)$ |
| $3$ | $(2,0,-5,3)$ | $(7,0,0,-7)$ |

: Loaded and unloaded ideal ports, all powers positive into the assembly.

For the middle row $j_s=3/2$, $j_r=-1/2\ \mathrm A$. Four unit terminal capacitances independently give $673/72\ \mathrm J$ at each endpoint; ideal windings have no storage coordinate. These are initialized steady constraint controls, not finite-core DC preparation claims. The corresponding mechanical controls have unit effective inertias, with carrier orbital mass counted once and planet/output spin combined once.

The other exact steady controls, with $\tau_s=2$, $\tau_o=1\ \mathrm{N\,m}$, all have torques $(2,-14/3,5/3,1)$. Their speeds are $(1,0,-2/5,-4/3)$ for carrier held; $(0,1,7/5,7/3)$ for sun held; $(7/4,1,7/10,0)$ for output held; $(1,1,1,1)$ for co-rotation; and $(-2,1,11/5,5)$ for counterrotation, in $\mathrm{rad/s}$. Multiplying each torque and speed gives its separate one-second work. A ring-held planet-drive control has $\tau_o=-1$, torques $(2,-28/3,25/3,-1)$ and works $(7,-28/3,0,7/3)\ \mathrm J$. Zero applied torques give zero work even with motion. At this geometry $\tau_r=0$ when $\tau_o=3\tau_s/4$ and $\tau_c=0$ when $\tau_o=3\tau_s/2$; these are sign boundaries, not singularities. A throughput ratio is undefined when all port powers vanish.

### Seven physical states with finite loading

Clamp $R$ to $O=0$, retain $v=(V_S,V_C,V_P)$ with $C=I\ \mathrm F$, and four winding currents. Define
\begin{align}
 B_f&=\begin{pmatrix}1&0&0&0\\-1&-1&-1&-1\\0&1&0&1\end{pmatrix},\\
 L&=\operatorname{diag}\left[
 \begin{pmatrix}9/16&-3/8\\-3/8&1\end{pmatrix},
 \begin{pmatrix}9/100&3/20\\3/20&1\end{pmatrix}\right]\mathrm H,
 \quad R_w=\operatorname{diag}(9/160,1/10,9/1000,1/10)\ \Omega,\\
 C\dot v&=(U,0,0)^T-Gv-B_fi,\qquad
 L\dot i=B_f^Tv-R_wi,\quad G=\operatorname{diag}(1,1/2,G_P).
 \label{eq:four-terminal-finite}
\end{align}
The source enters through $1\ \Omega$, the carrier receiver is $1/2\ \mathrm S$ and the planet receiver is $G_P$. Both inductance blocks are positive definite with coupling magnitude $1/2$. Begin from zero states and use $(U,G_P)=(1,1/4)$ on $[0,1]$, $(1,1/2)$ on $[1,2]$, $(1,1)$ on $[2,3]$, and $(0,1)$ on $[3,5]$ in SI units. All current paths remain connected; states are continuous and impulses zero, while powers have distinct event-side values.

For each constant interval augment $y=(v,i,1)$, write $\dot y=Ay$, and propagate $y_1=e^{A\Delta t}y_0$. Each separately declared quadratic port $P_k=y^TQ_ky$ has exact work $\int_0^{\Delta t}y_0^Te^{A^Tt}Q_ke^{At}y_0dt$, valid also when $A$ is singular. The external source power is $U(U-V_S)/(1\ \Omega)$; source heat, four copper losses and two receivers give $-(U-V_S)^2/(1\ \Omega)$, $-R_{wj}i_j^2$, $-V_C^2/(2\ \Omega)$ and $-G_PV_P^2$. The fixed ring clamp has zero power. Independently evaluate $E=v^TCv/2+i^TLi/2$ at every endpoint. Finite relaxation retains its actual final state; asymptotic decay does not imply exact reset at $t=5$.

A compliant mechanical realization follows from $v=\alpha_v\omega$, $z=Li/\alpha_v$, $J=\alpha_v^2C$, $K=\alpha_v^2L^{-1}$:
\begin{equation}
 J\dot\omega=\alpha_v(U,0,0)^T-\alpha_v^2G\omega-B_fKz,
 \qquad \dot z=B_f^T\omega-\frac{R_wKz}{\alpha_v^2}.
 \label{eq:four-terminal-mechanical}
\end{equation}
At unit scale each pair's elastic energy is $(z_1/h+z_2)^2/6+(z_1/h-z_2)^2/2$, $h=-3/4$ or $3/10$; its Hessian is the corresponding $L^{-1}$. The source is an external speed $\Omega_d=U/\alpha_v$ through viscous coefficient $\alpha_v^2/(1\ \Omega)$. Its motor-side power and coupling heat are separately integrated. At unit scale a $1\ \mathrm{kg}$ planet at radius $21/500\ \mathrm m$ contributes its orbital inertia to the unit carrier coefficient; the bare carrier is $1-(21/500)^2$, and planet/output spin is split into two halves of their unit coefficient. No inertia is counted again in a local constitutive law. This is a compliant system, not an exact realization of a rigid spatial gear.

If copper and source heat remain inside an insulated enlarged boundary, add $\dot H=(U-V_S)^2/(1\ \Omega)+\sum R_{wj}i_j^2$ and remove those exported-heat entries. Intermediate cooling and temperature-dependent coefficients need additional laws. Finite-core flux limits, magnetic nonlinearities, energized tap changing, spatial reactions and hardware correspondence remain unverified.

### Phasing and support work are local qualifications

For equal joint angles $0\leq\beta<\pi/2$, a correctly phased massless two-joint leadout gives $\theta_o=\theta_p$. More generally define the continuous lift $H_\beta(x)=\operatorname{atan2}(\sin x,\cos\beta\cos x)$ with $H_\beta(x+\pi)=H_\beta(x)+\pi$, $x=\theta_p-\phi$, and
$$
 \theta_o=\phi+H_{\beta_2}(H_{\beta_1}(x)+\gamma+\pi/2)-\pi/2.
$$
For correct phase $\tan F=(\cos\beta_2/\cos\beta_1)\tan x$; unequal angles require the corresponding changed support geometry. At equal angles with quadrature misphasing, $\chi=F'=c^2/(c^4\cos^2x+\sin^2x)$, $c=\cos\beta$, so $c^2\leq\chi\leq c^{-2}$ and $\omega_o=\omega_c+\chi(\omega_p-\omega_c)$. Counts include the endpoint ripple $[F(x_1)-x_1-F(x_0)+x_0]/(2\pi)$. A grounded phase command $\gamma=-\phi$ gives a carrier-relative secular count plus a two-phase endpoint ripple. One input period alone need not restore both phases. Its actuator power is $M(\partial\theta_o/\partial\gamma)\dot\gamma$, with its own physical supply.

For unit load, $\omega_c=1$, $x=t$, $\cos\beta_1=4/5$, $\cos\beta_2=3/5$, the massless linkage's planet, support and receiver powers are $2\chi$, $1-\chi$, $-(1+\chi)$ in watts. On $[0,\pi/4]\ \mathrm s$ their separate works are $2\arctan(3/4)$, $\pi/4-\arctan(3/4)$ and $-\pi/4-\arctan(3/4)\ \mathrm J$; on $[0,\pi]\ \mathrm s$ they are $2\pi,0,-2\pi\ \mathrm J$. The model has zero endpoint stores and no impulses. An added output inertia contributes support work $\omega_cI_o(\omega_p-\omega_c)[\chi-\chi^2/2]_{t_0}^{t_1}$, which vanishes only under the stated periodic endpoint conditions. Finite joint inertia, clearances, bearings and cross forces are not supplied by this speed map.

For multiple planets, axial free bodies leave force-sharing freedom. With equal bilateral tangential stiffness, zero tooth error and a common total mesh deflection, $F_{si}=\tau_s/(qr_s)+(\tau_{oi}-\bar\tau)/(2r_p)$, $F_{ri}=F_{si}-\tau_{oi}/r_p$, $R_{ti}=-F_{si}-F_{ri}$. At $q=3$, $\tau_s=2$ and the reference radii $(3/125,9/500,3/50)\ \mathrm m$, loads $(3,0,0)\ \mathrm{N\,m}$ give $F_s=(250/3,0,0)\ \mathrm N$; equal unit loads give $F_s=(250/9,250/9,250/9)\ \mathrm N$, each with $F_r=-F_s$. Both have $\tau_c=0,\tau_r=-5$ but distinct internal forces. Backlash, unilateral contact and a multi-output combiner require further models.

A slow comparison can hold the ring and compare unloaded and unit-loaded output under the constant commands in the table. Predicted carrier and ring reaction changes are $+7/3$ and $-10/3\ \mathrm{N\,m}$; receiver receipt is $7/3\ \mathrm J$ in one second. Independent speed/torque controls, synchronized channels and errors below the declared comparison gap are required. Illustrative targets are $1/20\ \mathrm{N\,m}$ per torque channel and $1/10\ \mathrm J$ for the work difference. A complete residual audit additionally retains all supplies, event timing, spin/orbit endpoints and losses. The electrical analogue needs finite pulses or AC within calibrated flux limits. Neither is a completed measurement.

# Transformer attachments and signed work
\label{app:transformers}

These constructions distinguish a reference change from an actual return, clamp or probe attachment, with the states and works required for each comparison.

## Winding opening, clamps and energized returns
\label{sec:transformer}

### A third-order clamp and its separate work integral

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

### Another finite removal path and the parasitic scale

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

### Loaded transformer and actual commutation

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

### Physical attachments add current paths and prepared states
\label{sec:physical-attachments}

A physical probe or return is an additional circuit branch. Its attachment changes the graph and can change the coefficients and observable states. Exchanging impedance and admittance descriptions of a fixed port does neither. Shared winding and return connections below require their coupled state equations; scalar two-terminal series--parallel composition alone does not describe this graph. The following finite graph retains both common-mode capacitances and an interwinding capacitance, so that their currents and endpoint stores are explicit. Node O is the physical primary-source return and chassis reference; the other node voltages are $v_A,v_B,v_C$. The source $u$ drives A through $R_s>0$, with core conductance $G_c\geq0$ from A to O. Winding 1 runs A to O. Winding 2 runs B to C for an isolated secondary ($\mu=0$), or B to A for a tapped connection ($\mu=1$). Its load $G_\ell\geq0$ and capacitor $C_d\geq0$ run from B to the physical receiver-return node C.

Capacitance $C_m>0$ connects A to B, while $C_B,C_C>0$ connect B and C to O. A finite return conductance $g_A$ connects A to C, another $g_O$ connects C to O, and a probe conductance $g_P$ connects B to O. All three are nonnegative. A change in one of them changes an actual effort--flow product. This model assumes constant linear capacitances and winding parameters on each interval; dielectric absorption, saturation and a moving chassis potential require their own laws.

With coordinate vectors $e_A,e_B,e_C$, put $d=e_B-e_C$, $q=e_A-e_C$, $v=(v_A,v_B,v_C)^T$, $i=(i_1,i_2)^T$, and define
\begin{align}
 \mathsf B_\mu&=(e_A,\ e_B-(1-\mu)e_C-\mu e_A),\nonumber\\
 \mathsf C_p&=
 \begin{pmatrix}
 C_m&-C_m&0\\
 -C_m&C_m+C_B+C_d&-C_d\\
 0&-C_d&C_C+C_d
 \end{pmatrix},\nonumber\\
 \mathsf G&=(R_s^{-1}+G_c)e_Ae_A^T+G_\ell dd^T
       +g_Aqq^T+g_Oe_Ce_C^T+g_Pe_Be_B^T.
 \label{eq:attachment-matrices}
\end{align}
Take the positive-definite winding matrix $\mathsf L$ from \eqref{eq:clamp-state} and $\mathsf R=\operatorname{diag}(R_1,R_2)$ with nonnegative winding resistances. Kirchhoff's laws give
\begin{equation}
 \mathsf L\dot i=\mathsf B_\mu^Tv-\mathsf Ri,\qquad
 \mathsf C_p\dot v=(u/R_s)e_A-\mathsf Gv-\mathsf B_\mu i.
 \label{eq:attachment-state}
\end{equation}
The capacitor quadratic form is
$C_m(v_A-v_B)^2+C_Bv_B^2+C_Cv_C^2+C_d(v_B-v_C)^2$.
It is strictly positive for nonzero $v$ under the stated positive-capacitance assumptions, and
$\det\mathsf C_p=C_m[C_BC_C+C_d(C_B+C_C)]>0$.
There are therefore five independent prepared states, compared with the three-state loaded model without these retained capacitive coordinates. A particular scalar observation can still cancel modes. Zero capacitances impose separate algebraic constraints; they cannot be substituted into this inverse while retaining five arbitrary initial coordinates.

Enclose the two winding stores and all four capacitor stores, with heat reservoirs outside and resistor thermal storage neglected. The source current is $i_s=(u-v_A)/R_s$, and the independently evaluated store is
\begin{equation}
 E=\tfrac12 i^T\mathsf Li+\tfrac12 v^T\mathsf C_pv.
 \label{eq:attachment-store}
\end{equation}
The nine inward port powers, each integrated separately, are
\begin{equation}
 \begin{gathered}
 ui_s,\quad -R_si_s^2,\quad -R_1i_1^2,\quad -R_2i_2^2,\quad -G_cv_A^2,\\
 -G_\ell(v_B-v_C)^2,\quad -g_A(v_A-v_C)^2,\quad -g_Ov_C^2,\quad -g_Pv_B^2.
 \end{gathered}
 \label{eq:attachment-powers}
\end{equation}
Multiplying the two state equations by $i^T$ and $v^T$ cancels their winding-node products. The remaining source term satisfies
$uv_A/R_s-v_A^2/R_s=ui_s-R_si_s^2$, proving that the sum of these nine powers is $\dot E$. This is a derived identity of the declared graph, not an assignment of a missing probe or chassis transfer from its remainder.

For fixed connections and constant $u$, let $x=(i^T,v^T)^T$ and augment $z=(x^T,1)^T$. Its exact generator is
\begin{equation}
 \mathsf K=
 \begin{pmatrix}
 -\mathsf L^{-1}\mathsf R&\mathsf L^{-1}\mathsf B_\mu^T&0\\
 -\mathsf C_p^{-1}\mathsf B_\mu&-\mathsf C_p^{-1}\mathsf G&
       \mathsf C_p^{-1}e_Au/R_s\\
 0&0&0
 \end{pmatrix},\qquad z(T)=e^{T\mathsf K}z_0.
 \label{eq:attachment-generator}
\end{equation}
Each power has its own symmetric matrix $H_\ell$ obtained from its stated effort and flow. Equation \eqref{eq:matrix-work} gives its exact value
$W_\ell=\mathcal W(\mathsf K,H_\ell,z_0,T)$.
Endpoint storage is separately $z(T)^TSz(T)$ with
$S=\tfrac12\operatorname{diag}(\mathsf L,\mathsf C_p,0)$.
These formulas give finite predictions for both $\mu$ values and each explicitly selected return or probe connection, including nonzero prepared currents and capacitor voltages.

Configuration XV uses the isolated graph, $L_1=L_2=1/10\ \mathrm H$, $M=1/20\ \mathrm H$, $R_1=R_2=1/10\ \Omega$, $R_s=100\ \Omega$, $G_c=g_A=g_O=0$, $G_\ell=1/1000\ \mathrm S$, and all four capacitances $1/1000\ \mathrm F$. Set $u=0$ on $[0,1]\ \mathrm s$ and prepare $i_1=i_2=0$, $v_A=v_B=v_C=1\ \mathrm V$. The initial store is exactly $1/1000\ \mathrm J$. Compare an absent probe, $g_P=0$, with the finite probe $g_P=1/1000\ \mathrm S$, using the same prepared state. Supplied preparation belongs to its own earlier interval; finite conductance insertion preserves the reactive states in this model. Actual gate storage and control work are additional measured quantities.

Let $\mathsf K_0,\mathsf K_1$ denote the two rational generators. If $h_B^Tz=v_B$, the probe's positive outward work in the attached case is the exact matrix-function value
\begin{equation}
 \delta_P=-\mathcal W(\mathsf K_1,-g_Ph_Bh_B^T,z_0,1\ \mathrm s)
 =g_P\int_0^{1\,\mathrm s}(h_B^Te^{t\mathsf K_1}z_0)^2\dd t>0.
 \label{eq:attachment-separation}
\end{equation}
The strict sign follows from continuity and $v_B(0)=1\ \mathrm V$. No work comparison between different paths is needed to establish it. The source work is zero in both cases because the specified source effort is zero; the source resistor remains attached and can receive energy.

| Observable in XV | Probe absent | Finite probe attached |
|:----------------------------|:-----------------------------|:----------------------------------|
| Initial probe current into its resistor | $0$ | $1/1000\ \mathrm A$ |
| Probe signed work into reactive boundary | $0$ | $-\delta_P<0$ |
| Final reactive store | $(e^{T\mathsf K_0}z_0)^TS(e^{T\mathsf K_0}z_0)$ | $(e^{T\mathsf K_1}z_0)^TS(e^{T\mathsf K_1}z_0)$ |
| Any other named work | $\mathcal W(\mathsf K_0,H_{\ell0},z_0,T)$ | $\mathcal W(\mathsf K_1,H_{\ell1},z_0,T)$ |

: Exact finite-attachment predictions at $T=1\ \mathrm s$. Every matrix and initial coordinate is specified by rational component values; the two final stores need not agree.

Separate voltage and shunt-current observations on the added branches distinguish a physical attachment from a coordinate relabeling. Work half-widths below $\delta_P/2$ suffice for the nominal probe-work comparison; parameter, preparation, bandwidth and event-timing uncertainty must be included in those widths. The initial-current contrast additionally requires the calibrated transient response, rather than an assumed instantaneous readout. Finite voltage/current scales provide an ordinary low-voltage comparison, without an asserted achieved uncertainty.

A conservative uniform requirement can be made explicit for XV. Keep the isolated graph and zero drive; allow $L_1,L_2\in[9/100,11/100]\ \mathrm H$, $M\in[9/200,11/200]\ \mathrm H$, $R_1,R_2\in[9/100,11/100]\ \Omega$, $R_s\in[90,110]\ \Omega$, and each of the four capacitances, the load conductance and the attached probe conductance within $[9/10000,11/10000]$ in their SI units. Keep $G_c=g_A=g_O=0$, zero initial currents and all three initial voltages in $[9/10,11/10]\ \mathrm V$. With currents scaled by $1\ \mathrm A$ and voltages by $1\ \mathrm V$, $\lambda_{\min}(\mathsf L)\geq7/200\ \mathrm H$ and $\lambda_{\min}(\mathsf C_p)\geq3/10000\ \mathrm F$. The latter follows from $C_m(e_A-e_B)(e_A-e_B)^T+C_Be_Be_B^T+C_Ce_Ce_C^T$, whose unit-coefficient smallest eigenvalue exceeds $1/3$; the load capacitor adds a positive term. These bounds in \eqref{eq:attachment-generator} give the deliberately loose $\|A\|_\infty\leq20000\ \mathrm{s^{-1}}$ for the five homogeneous physical coordinates. Therefore $\|x(t)-x(0)\|_\infty\leq(11/10)(e^{20000t}-1)$, and
\begin{equation}
 T_* =\frac{\log(31/22)}{20000}\ \mathrm s,\qquad
 \delta_P\geq\frac{9}{10000}\left(\frac9{20}\right)^2 T_*\ \mathrm W
 =\frac{729\log(31/22)}{80000000000}\ \mathrm J>0.
 \label{eq:attachment-uniform-bound}
\end{equation}
Indeed $v_B\geq9/20\ \mathrm V$ on this initial subinterval, which lies inside the one-second comparison. The absent-probe work is exactly zero. The sum of both prediction/measurement half-widths must be below this lower bound to guarantee uniform separation. It is a conservative sufficient requirement, not a claim of achieved instrument accuracy; a sharper enclosure could substantially relax it. Unmodeled probe dynamics must first be included in the graph.

For the independent hardware question, identify $\mathsf L$, capacitances, resistances, probe paths and the prepared states before the final comparison. Use those same parameter sets to predict both connections through \eqref{eq:attachment-generator}; allow their calibrated joint uncertainty, including the mutual sign, to generate prediction sets. Simultaneously measure each of \eqref{eq:attachment-powers} and both stores, including the interwinding voltage difference. A graph can disagree with observed waveforms while its measured full account closes, or leave a signed account residual beyond the enclosure in Appendix \ref{sec:uncertainty}. These are different outcomes. Saturation, dielectric memory, common-mode sensor loading, a moving chassis voltage and unmeasured initial flux require separately specified states or observations. Exact model identities provide no apparatus record and do not settle those physical questions.

How does the separately integrated source, winding and receiver work change when a physical return or probe is connected, and what residual survives the complete finite-state account? A low-voltage pair of coupled coils with a finite source resistor, load and output capacitor provides accessible winding voltages, shunt currents and capacitor endpoints. Hold the winding orientation, component values, initial currents and capacitor voltage fixed while changing a declared load or return. Integrate each of the seven powers accompanying \eqref{eq:loaded-transformer} over the same finite interval; evaluate both magnetic and electric endpoint stores independently. Current preparation or initial linkage must be measured, not inferred from the final work balance. Simultaneous low-frequency acquisition makes polarity, phase and resistor heating accessible with ordinary instruments.

Zero commanded source voltage and an opened conductor are different conditions. An opened winding needs a finite commutation path; it is not a substitution into the closed-circuit equations. An observed load-work increase may accompany greater source work, release of initially stored energy, or a resolved residual. Their signs and endpoint changes discriminate these alternatives. A probe-induced trajectory change is a physical loading result, whereas a common voltage-origin shift with zero total terminal current leaves total power unchanged. Neither the volt-second comparison nor a load-only integral answers the energy question.

Can independently calibrated winding and probe parameters predict those local works and endpoint states across the declared finite-return configurations? Keep parameter identification separate from the final conditions and retain the full joint uncertainty in $L_1,L_2,M$ when evaluating $i^T\mathsf Li/2$. Appendix \ref{sec:instrument-bounds} supplies channel-level bounds. Agreement within them supports this specified realization; a signed excess outside them remains an open result. Saturation, chassis current, thermal drift and an unmeasured initial flux remain distinct hypotheses requiring their own observations.

### A complete finite return commutation
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

For XII, the determinant argument establishes nominal positivity only. No positive lower bound over a calibrated component/preparation box is established here. Consequently $B_A<\delta_A/2$ is a nominal mathematical criterion, not a uniform instrument specification. Before claiming a practical comparison, bound the work functional over the same joint uncertainty set for both paths and require its minimum separation to exceed the sum of their half-widths. A box containing vanishing overlap duration or conductance has no positive uniform lower bound. The finite-component enclosure and the measured switch law remain explicit unresolved tasks; the exact nominal account remains valid.

The overlap conductance $g_e=1\ \mathrm S$, versus zero without overlap, supplies a separate topology check from synchronized $i_s,i_1,i_2,v_a$. The open physical question is which measured switch law reproduces these individual works, endpoint stores and any additional control-supply transfer. Both-returns-open operation requires another capacitive, clamp or arc path for nonzero $i_2$. Actual gate work and edge storage remain explicit additional ports and states in that experiment.

# Controlled transducers and supplied references
\label{app:controllers}

These independently supplied realizations retain the actuator, bias, driver, receiver and rail accounts needed to interpret their observable motion and work.

## A source-off transducer and a finite bias supply
\label{sec:transducer}

### Plant and controller are separate boundaries

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

### A derived low-force scale

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

### A reciprocal actuator with finite electrical storage

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

### Regenerative and dissipative receiving paths

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

The derived observation ranges are within $\pm6\ \mathrm V$ including the DC link, $\pm1/5\ \mathrm A$, $\pm1/5\ \mathrm N$, $\pm1/50\ \mathrm m$ and $\pm1/5\ \mathrm{m/s}$ on a window shorter than $1/10\ \mathrm s$. Amplitudes alone do not establish control response. Differentiation gives $u_b'(0)=-1452\ \mathrm{V/s}$ and $i_b'(0)=119/10\ \mathrm{A/s}$; these are the maximum absolute slews on this interval. The affine factor under the square root changes by its initial value in $1/2400\ \mathrm s$. Actuator requirements are $|\dot i_a|\leq3/2\ \mathrm{A/s}$ and $|\dot u_a|\leq1\ \mathrm{V/s}$. These exact values set finite response requirements for a candidate regulator and synchronized probes. Tracking error is assessed from measured force and current, not from the force command. Appendix \ref{sec:uncertainty} bounds its effect on signed work.

Physical efficiency, sensor/logic power, saturation and switching bandwidth remain unmeasured. Thermal observations require identified heat capacities or calorimetric boundaries; repeated preparations add their own work if repetition increases the signal. If $g_e,g_m$ depend on changing $i_b$, their dynamics must be retained and \eqref{eq:plant-path} must be checked in that enlarged model.

For the wider finite bias-dependent supply models, four accuracy questions remain unresolved: thermal endpoint convergence, agreement of independently evaluated signed-power quadratures, interval energy residuals, and integrated DC-link subledgers. These limitations include stable finite paths as well as growing finite windows. A complete-interval combined balance or an exact coil identity does not settle the separate interval and link checks. The present closed forms supply no numerical convergence result for those different models.

The physical question is whether independently measured reaction, actuator electrical export, bias power and finite-supply changes reproduce the positive coil change with all subboundaries resolved. A signed remainder beyond calibrated uncertainty remains an open result alongside the observed coil increase.

### Growing plant storage and a distinct bias-dependent law
\label{sec:growing-plant}

The next control has different coefficients and preparation from configuration X. Its growing plant store tests the separately supplied voltage actuator; the subsequent bias-dependent model is a third, nonlinear realization.
\label{sec:coupling-open}

An electrical winding and a mechanical oscillator form a natural third-order system:
\begin{equation}
 L\dot i=v_{s}-Ri-g_{e} v,\qquad \dot x=v,\qquad
 m\dot v=g_{m}i-dv-kx+F_{s},
 \label{eq:transducer}
\end{equation}
where $d=c+c_\ell$ may include internal and load damping. With
$Z_{e}=R+sL$, $Z_{m}=d+sm+k/s$,
\begin{equation}
 \binom{v_{s}}{F_{s}}=
 \begin{pmatrix}Z_{e}&g_{e}\\-g_{m}&Z_{m}\end{pmatrix}\binom i v,
 \quad \mathcal D=Z_{e}Z_{m}+g_{e}g_{m},
 \quad \frac v{v_{s}}=\frac{g_{m}}{\mathcal D},\quad
 \frac i{F_{s}}=-\frac{g_{e}}{\mathcal D}.
 \label{eq:transducer-port}
\end{equation}
The minus sign follows the chosen mechanical source orientation. Reciprocity has $g_{e}=g_{m}$ in consistent effort--flow units; the antisymmetric off-diagonal signs do not mean nonreciprocity. Its scalar characteristic polynomial is
\begin{equation}
 s\mathcal D=Lm s^3+(Rm+Ld)s^2+(Rd+Lk+g_{e}g_{m})s+Rk.
 \label{eq:growing-transducer-cubic}
\end{equation}
The cubic Routh condition applies to these complete coefficients. Positive reciprocal coupling with positive damping gives a passive stable realization; altering one coupling independently requires a new physical explanation.

For $E=Li^2/2+mv^2/2+kx^2/2$,
\begin{equation}
 \dot E=v_{s}i+F_{s}v-Ri^2-dv^2+(g_{m}-g_{e})iv.
 \label{eq:transducer-work}
\end{equation}
The last term is an unassigned coupling power for the sources and losses listed in \eqref{eq:transducer}. Enclose the winding, mass and spring and exclude the source and loss reservoirs. On a smooth interval $[t_0,t_1]$ without resets, integrate the four inward powers separately:
\begin{align}
 W_V&=\int_{t_0}^{t_1}v_si\,\dd t,&
 W_F&=\int_{t_0}^{t_1}F_sv\,\dd t,\nonumber\\
 W_R&=-\int_{t_0}^{t_1}(Ri)i\,\dd t,&
 W_d&=-\int_{t_0}^{t_1}(dv)v\,\dd t,\nonumber\\
 r_E^{\mathrm{listed}}&=E(t_1)-E(t_0)-W_V-W_F-W_R-W_d
       =\int_{t_0}^{t_1}(g_m-g_e)iv\,\dd t.
 \label{eq:coupling-residual}
\end{align}
When $d=c+c_\ell$, the last loss is split into the internal damper and load integrals before combination. A controller, bias reaction or revised constitutive law may account for the residual. Its signed work must be established independently. Assigning the rightmost integral to a named port does not establish the transfer. One-way coupling $g_m=0$, reversed $g_m=-g_e$ and attenuated $g_m=g_e/2$ remain distinct controls, with stability and port passivity assessed for their own parameters.

#### Zero named commands with unequal effective coupling

An illustrative finite-prefix solution makes the positive residual explicit. Choose
\begin{align}
 L&=1\ \mathrm H,&m&=1\ \mathrm{kg},& k&=1\ \mathrm{N/m},\nonumber\\
 R&=1\ \Omega,&d&=1\ \mathrm{N\,s/m},&
 g_e&=-2\ \mathrm{V\,s/m},\qquad g_m=3\ \mathrm{N/A},
 \label{eq:source-off-values}
\end{align}
and set $v_s=F_s=0$. With $\vartheta=t/(1\ \mathrm s)$, the prepared state and its evolution are
\begin{equation}
 i=e^\vartheta\ \mathrm A,\qquad x=e^\vartheta\ \mathrm m,
 \qquad v=e^\vartheta\ \mathrm{m/s}.
 \label{eq:source-off-trajectory}
\end{equation}
Substitution gives $L\dot i=-Ri-g_ev$ and $m\dot v=g_mi-dv-kx$ exactly, together with $\dot x=v$. In the dimensionless Laplace variable $z=s(1\ \mathrm s)$, the characteristic polynomial is
\begin{equation}
 z^3+2z^2-4z+1=(z-1)(z^2+3z-1).
 \label{eq:source-off-polynomial}
\end{equation}
The solution is an unstable finite prefix, with a specified initial state; it is not a periodic operating state. Preparation lies before $t=0$ and has no assigned work here. Its constitutive initial store is nevertheless included. No switching occurs on $[0,T]$, $T=(\log2)\ \mathrm s$.

Direct signed integration gives $W_V=W_F=0$ and
\begin{align}
 W_R=W_d&=-\int_0^{\log2}e^{2\vartheta}\,\dd\vartheta\ \mathrm J
         =-\frac32\ \mathrm J,\nonumber\\
 \int_0^T(g_m-g_e)iv\,\dd t
       &=5\int_0^{\log2}e^{2\vartheta}\,\dd\vartheta\ \mathrm J
       =\frac{15}{2}\ \mathrm J.
 \label{eq:source-off-works}
\end{align}
Independent state evaluation yields the following account.

| Quantity on $[0,(\log2)\ \mathrm s]$ | Exact value |
|:--------------------------------------------------|------------------:|
| Initial winding, kinetic and spring store combined | $3/2\ \mathrm J$ |
| Final combined store | $6\ \mathrm J$ |
| Store increase | $9/2\ \mathrm J$ |
| Electrical-source and mechanical-source works, each | $0$ |
| Resistor work into the boundary | $-3/2\ \mathrm J$ |
| Damper work into the boundary | $-3/2\ \mathrm J$ |
| Residual for the listed ports | $+15/2\ \mathrm J$ |

: Increasing declared storage with both listed drives zero. The coupling transfer remains unassigned for this model's listed ports.

The trajectory, individual integrals, polynomial and endpoint stores have exact checks. The missing physical coupling account remains open. A proposed implementation must identify how the unequal couplings arise and determine its additional work, stores and losses. This example fixes the magnitude and sign of that question without reporting a physical observation.

For a candidate realization, synchronized winding voltage/current and mechanical force/velocity provide the listed-port works; bias and DC-link channels provide separate candidate transfers. Independently calibrated $L,m,k$ and state measurements determine both endpoint stores. Retain \eqref{eq:coupling-residual} beside the expanded-boundary result, and apply the uncertainty criterion in Appendix \ref{sec:residual-outcomes}. Neither defining the controller work by subtraction nor choosing its parameters to cancel the residual identifies a physical account.

#### A separately instrumented coupling control
\label{sec:coupling-control}

A reciprocal transducer of coupling $g$, together with a series voltage actuator commanded by velocity, realizes an explicit candidate port. Let $u_c=Kv$ and
\begin{equation}
 L\dot i=v_s+u_c-Ri-gv,\qquad
 \dot x=v,\qquad m\dot v=gi-dv-kx+F_s.
 \label{eq:coupling-actuator}
\end{equation}
The reduced coefficients are $g_m=g$ and $g_e=g-K$. Taking $g=3\ \mathrm{N\,A^{-1}}$ and $K=5\ \mathrm{V\,s\,m^{-1}}$ reproduces the unequal coefficients above. The extra physical power is $u_ci$, positive into the plant and negative out of the actuator. Setting $v_s=0$ leaves that port active.

On the exact exponential trajectory and interval already specified, direct integration gives $W_c=\int u_ci\,\dd t=15/2\ \mathrm J$. The reduced listed-port residual remains $+15/2\ \mathrm J$; the enlarged plant account has zero residual under this declared actuator law. The output port was specified before the integral, not defined from the remainder. This is a realizable control hypothesis, not a measurement of the original apparatus. Measure actuator output voltage and current independently of its supply/DC-link channels, losses and endpoint stores. Equal output and supply work cannot be presumed.

Linearity permits an ordinary low-amplitude control: multiplying the original state by $\lambda=1/100$ gives displacement $1$ to $2\ \mathrm{cm}$, current $10$ to $20\ \mathrm{mA}$ and commanded voltage $1/20$ to $1/10\ \mathrm V$ on the same interval. Its plant store increases by $9/20000\ \mathrm J$ and the candidate output work is $3/4000\ \mathrm J$. These exact predictions assume the same coefficients and feasible initial preparation; actual signal-to-error ratios require calibration. Force, velocity, voltage and shunt-current channels can distinguish output transfer, supply depletion and unexplained residual without assigning any of them by subtraction. Finite actuator and sensor dynamics add states and may change the effective order and closed-loop stability.

#### Passivity and a finite supply remain separate questions

For real constants, the Hermitian dissipative part of the impedance matrix is
$\left(\begin{smallmatrix}R&(g_{e}-g_{m})/2\\(g_{e}-g_{m})/2&d\end{smallmatrix}\right)$.
After consistent port scaling it is positive semidefinite exactly when
\begin{equation}
 R\geq0,\qquad d\geq0,\qquad (g_{e}-g_{m})^2\leq4Rd.
 \label{eq:transducer-pr}
\end{equation}
Thus unequal coupling is not automatically a nonpassive terminal map; damping can satisfy this inequality. A model implemented with an active controller and a passive external map are compatible descriptions at different boundaries. Electrical linkage and mechanical momentum have different units and must not be added as a scalar stress measure.

A finite bias coil adds its own store, copper loss and source path. To make one conditional account explicit, let $I_*>0$ be a reference bias current and prescribe $g_e=\bar g_e i_b/I_*$, $g_m=\bar g_m i_b/I_*$. Define the reaction effort $A=(\bar g_m-\bar g_e)iv/I_*$, which has voltage units, and the plant transfer $P_a=i_bA$. For a nonnegative converter loss $\ell(P)=\epsilon_\ell P^2/(P_*+|P|)$, with $\epsilon_\ell\geq0$ and $P_*>0$, a candidate bias-winding equation is
\begin{align}
 L_b\dot i_b&=u_b-R_bi_b-A-v_\ell,&
 v_\ell&=\frac{\epsilon_\ell i_bA^2}{P_*+|i_bA|},\nonumber\\
 E_b&=\frac12L_bi_b^2,&
 \dot E_b&=u_bi_b-R_bi_b^2-P_a-\ell(P_a).
 \label{eq:bias-state}
\end{align}
Here $u_b$ is the converter voltage applied to the bias coil, and $v_\ell i_b=\ell(P_a)\geq0$. The formula is continuous at $i_b=0$: $v_\ell=0$ there, while the reaction effort $A$ may remain nonzero. The illustrative choice $\epsilon_\ell=1/50$, $P_*=1\ \mathrm W$ gives the stated loss law without asserting measured converter behavior. This supplies a declared dynamical hypothesis, not an identified physical supply.

Enclose the bias winding and exclude the plant, DC link and heat reservoirs. On a smooth source-off interval $[t_0,t_1]$ with $u_b=0$, its separately integrated inward works are
\begin{align}
 W_{\mathrm{reaction}}&=-\int_{t_0}^{t_1}A i_b\,\dd t,&
 W_{\mathrm{copper}}&=-\int_{t_0}^{t_1}(R_bi_b)i_b\,\dd t,\nonumber\\
 W_{\mathrm{converter}}&=-\int_{t_0}^{t_1}v_\ell i_b\,\dd t,&
 r_b&=\frac{L_b}{2}[i_b(t_1)^2-i_b(t_0)^2]
       -W_{\mathrm{reaction}}-W_{\mathrm{copper}}-W_{\mathrm{converter}}.
 \label{eq:bias-dependent-work}
\end{align}
The endpoint coil store increases in this candidate exactly when
\begin{equation}
 -\int_{t_0}^{t_1}P_a\,\dd t>
 \int_{t_0}^{t_1}R_bi_b^2\,\dd t+
 \int_{t_0}^{t_1}\ell(P_a)\,\dd t.
 \label{eq:bias-increase}
\end{equation}
It is the signed reaction, not the source-off label, that determines this prediction. Disabling an external charger does not imply $u_b=0$; retain $\int u_bi_b\,\dd t$ if the converter continues to drive. The constant-coupling exponential example is a different model from this bias-dependent system and is not silently reused as its trajectory.

Appendix \ref{sec:supply} supplies a finite DC link, sensor and thermal account with seven continuous states. Each state has its own endpoint evaluation and each transfer its own integral. The open question is whether a physical bias supply realizes these couplings and the source-off increase with consistent coil, DC-link, thermal and plant accounts. Measure coil current at both endpoints with independently calibrated $L_b$, winding voltage/current throughout the interval, and the separately accessible converter-output and DC-link pairs. Reaction effort requires an independently identified transduction law or a direct conjugate measurement; the coil remainder alone does not identify it. The measurable reciprocal control above does not settle this different nonlinear seven-state model. Interval balance, DC-link work and thermal endpoint consistency remain separate unresolved checks beyond the exact conditional identities. A small combined-path residual can conceal opposite local residuals and does not settle them. Thermal laws, saturation, hysteresis, switching slew, feedback, multi-axis coupling and calibrated cross-domain sensors remain additional physical requirements. Finite-prefix work identities do not give an unstable control a steady-state interpretation.

## An accelerating reference requires a supplied counterpart
\label{sec:reference}

### Relative kinetic storage and a physical capacitor

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

### Equal capacitor endpoints with different driver works
\label{sec:physical-reference}

The same capacitor-cell map permits an independently specified normalization and finite ramp comparison. Its compensation and driver ports remain distinct. Consider a physical capacitor cell: a node $V_A$ and driven reference $V_R$ bound a capacitor $C=J/\alpha^2$, where $J$ is an inertia and $\alpha$ converts angular velocity to voltage. Let $w=V_A-V_R$, $V_R=\alpha\Omega$, and install two actual current-source ports,
\begin{equation}
 I_\tau=\tau/\alpha,\qquad I_r=-C\dot V_R,\qquad
 C\dot w=I_\tau+I_r,\qquad E_C=\frac12Cw^2.
 \label{eq:reference-cell-unit}
\end{equation}
The compatible map $V_A=\alpha\omega$ gives $J\dot\omega=\tau$. The separately integrated capacitor powers are $wI_\tau=\tau(\omega-\Omega)$ and $wI_r=-J\dot\Omega(\omega-\Omega)$. These are declared source ports and reproduce the accelerating-frame terms exactly. Omitting $I_r$ defines a different physical cell. With $J=\alpha=1$ in consistent units, $\tau=0$, $\Omega=2t$ and zero initial velocities on $[0,1\ \mathrm s]$, the compensated cell has $w=-2t$, $W_\tau=0$, $W_r=2\ \mathrm J$, and independently $E_0=0$, $E_1=2\ \mathrm J$. The uncompensated floating cell instead has $w=0$ and zero store throughout. Each model has a zero full residual; they are different trajectories and different sources.

A separate finite reference driver obeys $C_d\dot r=j_d=(u-r)/R_d$, with $r=V_R$. Its capacitor and resistor are physical even when the ideal floating receiver draws zero net bias current. For a finite linear ramp on $[0,T]$, prescribe $r=r_-+\Delta r\,t/T$ and $u=r+R_dC_d\Delta r/T$. Enclosing only the driver capacitor gives the independently evaluated account
\begin{align}
 W_u&=\int_0^Tuj_d\,\dd t
 =C_dr_-\Delta r+\frac12C_d(\Delta r)^2
       +\frac{R_dC_d^2(\Delta r)^2}{T},\nonumber\\
 W_{R_d}&=-\int_0^TR_dj_d^2\,\dd t
 =-\frac{R_dC_d^2(\Delta r)^2}{T},\nonumber\\
 E_{d,0}&=\frac12C_dr_-^2,\qquad
 E_{d,1}=\frac12C_d(r_-+\Delta r)^2,\qquad
 r_d=E_{d,1}-E_{d,0}-W_u-W_{R_d}=0.
 \label{eq:reference-ramp-work}
\end{align}
There is no ideal event within the interval; extending the ramp requires an explicit adjoining drive. The cell's compensation-source work is separate from this driver account, not supplied for free by its bias node.

For $C_d=1\ \mathrm{mF}$, $R_d=100\ \Omega$, $r_-=0$ and $\Delta r=1\ \mathrm V$, a one-second ramp gives $j_d=1\ \mathrm{mA}$, $W_u=3/5000\ \mathrm J$, $W_{R_d}=-1/10000\ \mathrm J$, and $E_{d,1}=1/2000\ \mathrm J$. A half-second ramp gives $j_d=2\ \mathrm{mA}$, $W_u=7/10000\ \mathrm J$ and $W_{R_d}=-1/5000\ \mathrm J$, with unchanged capacitor endpoints. These finite voltage, current and timing choices are set before the work audit. Ordinary voltage and shunt channels directly distinguish duration-dependent works from duration-independent endpoint change. Independently observe the compensation-source outputs and their supplies when adding the receiver; their work is not the driver remainder.

The unit-scale reference-cell example also permits the distinct driver choice $C_d=1/200\ \mathrm F$, $R_d=3/4\ \Omega$, $r=2t$. It gives $j_d=1/100\ \mathrm A$, $W_u=403/40000\ \mathrm J$, $W_{R_d}=-3/40000\ \mathrm J$, and endpoint change $1/100\ \mathrm J$. None of these equals the receiver's $2\ \mathrm J$ compensation work. This separates three boundaries that a formal change of reference can conceal.

### A causal compound reference and its supply

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

### A complete polynomial receiver control

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

### A dissipative control with complete event coverage

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

### Finite sensor, actuator and converter states

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

### Constraint paths, rigid reduction and a reference-jump obstruction

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

## A finite bias supply and its separate store accounts
\label{sec:supply}

The constant-coupling cubic in \eqref{eq:growing-transducer-cubic} and a transducer with a finite bias supply are different dynamical systems. This appendix constructs one conditional seven-state model so that source-off coil growth, DC-link transfer and thermal change can be checked separately. The construction states the required port laws; it does not identify a physical implementation of the unequal coupling or settle an unexplained apparatus residual.

### State equations and finite control laws

Take the plant states $(i,x,v)$ from \eqref{eq:transducer}, the bias current $i_b$ from \eqref{eq:bias-state}, the DC-link voltage $V_b$, sensor voltage $z$ and thermal energy $E_\theta\geq0$. All capacitances and inductances are positive. Internal plant damping is $c\geq0$, load damping is $c_\ell\geq0$, and additional finite reset resistances and dampings are $R_r(t),c_r(t)\geq0$. On a declared smooth interval the plant equations are
\begin{align}
 L\dot i&=v_s-(R+R_r)i-\bar g_e(i_b/I_*)v,\nonumber\\
 \dot x&=v,\qquad
 m\dot v=\bar g_m(i_b/I_*)i-(c+c_r+c_\ell)v-kx+F_s.
 \label{eq:supply-plant}
\end{align}
The bias reaction effort $A$, loss voltage $v_\ell$ and current equation are \eqref{eq:bias-state}. They define $P_a=i_bA$ positive into the plant and $-Ai_b$ into the bias winding. A finite converter command can, for example, be
\begin{equation}
 u_b=\operatorname{clip}\!\left(
 R_bI_*\alpha+K_b(I_*\alpha-i_b),-V_b,V_b\right),
 \qquad V_b>0,\quad K_b\geq0,\quad 0\leq\alpha\leq1.
 \label{eq:bias-command}
\end{equation}
Here $K_b$ has resistance units and $\operatorname{clip}(q,a,b)=\min\{b,\max\{a,q\}\}$. The dimensionless command $\alpha(t)$ is prescribed by the operation or preparation path. A smooth finite connection can use $\alpha=[1-\cos(\pi(t-t_0)/T)]/2$ on $[t_0,t_0+T]$; disconnection reverses this path. On the specific source-off interval set $u_b=0$ as a separate converter mode. Setting $\alpha=0$ in the feedback expression alone would generally apply a braking voltage instead.

Let an ideal charger effort $U$ feed the DC link through resistance $R_s>0$ and a symmetric current limit $I_{\max}>0$. Its constitutive path is
\begin{equation}
 j=\operatorname{clip}\!\left(\frac{U-V_b}{R_s},-I_{\max},I_{\max}\right),
 \quad v_{\mathrm{lim}}=U-V_b-R_sj,
 \quad P_{\mathrm{line}}=(R_sj)j+v_{\mathrm{lim}}j.
 \label{eq:charger-path}
\end{equation}
Inside the current limit $v_{\mathrm{lim}}=0$; outside it the limiter voltage and current have the same sign. Thus each loss product is nonnegative and $Uj=V_bj+P_{\mathrm{line}}$ by the declared voltage law. At $U=0$ the source work is zero but the attached resistance/limiter can still discharge the bus: source-off and open charger are different topologies.

For a dimensionally explicit sensor signal define $h=a_i i+a_vv$, with $a_i$ in volts per ampere and $a_v$ in volt seconds per metre. Let $C_s>0$, $G_s\geq0$ and $\tau_s>0$. In the powered sensing mode set $\dot z=(h-z)/\tau_s$; in the source-off mode set $\dot z=-G_sz/C_s$. The injected sensor current, signed sensor-supply power and nonnegative logic loss are
\begin{equation}
 j_s=C_s\dot z+G_sz,\qquad P_s=zj_s,\qquad
 P_{\mathrm{logic}}=u_{\mathrm{logic}}j_{\mathrm{logic}},\quad
 j_{\mathrm{logic}}=G_{\mathrm{logic}}u_{\mathrm{logic}},\quad G_{\mathrm{logic}}\geq0.
 \label{eq:sensor-supply}
\end{equation}
The sensor power may be negative during return. In the off mode $j_s=0$; disabling the logic sets $u_{\mathrm{logic}}=0$. The sensor and logic effort laws describe a candidate implementation and require physical identification. In particular, motion and current are never added without their voltage conversion scales.

For DC-link leakage $G_b\geq0$, its state equation is
\begin{equation}
 C_b\dot V_b=j-G_bV_b-
       \frac{u_bi_b+P_s+P_{\mathrm{logic}}}{V_b},\qquad V_b>0.
 \label{eq:dc-link-state}
\end{equation}
The demand contains coil-terminal, sensor and logic powers. Actuator reaction and converter loss already enter the coil equation; adding them again to this DC-link demand would count the same account twice. At $V_b=0$, nonzero demanded power is outside this realization. A zero-demand continuation requires a separately defined converter law, not division by a vanishing voltage.

Define plant heat rates $H_e=(R+R_r)i^2$, $H_m=(c+c_r)v^2$, bias copper heat $H_b=R_bi_b^2$, link leakage heat $H_g=G_bV_b^2$ and sensor heat $H_s=G_sz^2$. All are effort--flow products in their corresponding electrical or mechanical components. A conditional thermal reservoir obeys
\begin{equation}
 \dot E_\theta=H_e+H_m+H_b+H_g+H_s+\ell(P_a)
                +P_{\mathrm{logic}}+P_{\mathrm{line}}-Q_{\mathrm{amb}},
 \qquad Q_{\mathrm{amb}}=\gamma_\theta E_\theta,\quad\gamma_\theta\geq0.
 \label{eq:supply-thermal}
\end{equation}
One constitutive temperature assignment is $\Theta=\Theta_a+E_\theta/C_\theta$ with $\Theta_a,C_\theta>0$. The outward thermal port has power $\Theta\dot S_{\mathrm{out}}=Q_{\mathrm{amb}}$, where $\dot S_{\mathrm{out}}=Q_{\mathrm{amb}}/\Theta$ is the specified entropy flow at that boundary. The temperature law, heat destinations and thermal conductance remain material assumptions to identify. Load power $-c_\ell v^2$ crosses to the external load and is not also included in this thermal store.

There are seven continuous coordinates, with local uniqueness on the declared regular domain. The products involving $i_b$ make the combined model nonlinear; a constant third-order characteristic polynomial no longer describes it globally. Scalar observable order requires its own local elimination and state-image analysis. Finite preparation, connection, operation, disconnection, source-off relaxation and resistive reset have distinct vector fields. Continuous state transport gives zero ideal impulse for these finite changes. A finite reset generally retains an endpoint store, and that remainder is carried into the next interval rather than deleted.

### Separate works, endpoints and unresolved local checks

For an explicit finite interval $[t_0,t_1]$ lying within one mode, write $\mathcal W[p]=\int_{t_0}^{t_1}p(t)\,\dd t$. Every occurrence below denotes a separately evaluated signed port integral. Evaluate the stores independently at both ends:
\begin{equation}
 E_p=\frac{Li^2+mv^2+kx^2}{2},\quad
 E_b=\frac{L_bi_b^2}{2},\quad E_{\mathrm{dc}}=\frac{C_bV_b^2}{2},
 \quad E_s=\frac{C_sz^2}{2},\quad
 E_{\mathrm{all}}=E_p+E_b+E_{\mathrm{dc}}+E_s+E_\theta.
 \label{eq:supply-stores}
\end{equation}
The separate inward power products for the four reactive sub-boundaries are

| Store boundary | Inward port powers, each integrated separately |
|:-----------------------|:-------------------------------------------------------------|
| Plant $E_p$ | $v_si$, $F_sv$, $-H_e$, $-H_m$, $-(c_\ell v)v$, $P_a$ |
| Bias coil $E_b$ | $u_bi_b$, $-H_b$, $-Ai_b$, $-v_\ell i_b$ |
| DC link $E_{\mathrm{dc}}$ | $V_bj$, $-H_g$, $-u_bi_b$, $-zj_s$, $-u_{\mathrm{logic}}j_{\mathrm{logic}}$ |
| Sensor $E_s$ | $zj_s$, $-H_s$ |

: Nested boundaries for the conditional finite supply. Thermal receiving powers are given separately in \eqref{eq:supply-thermal}.

Define each residual as its independent store change minus the sum of those individual works. In particular,
\begin{align}
 r_{\mathrm{dc}}={}&\Delta E_{\mathrm{dc}}-
 \bigl(\mathcal W[V_bj]+\mathcal W[-H_g]+\mathcal W[-u_bi_b]
                  +\mathcal W[-P_s]+\mathcal W[-P_{\mathrm{logic}}]\bigr),\nonumber\\
 r_s={}&\Delta E_s-\mathcal W[P_s]-\mathcal W[-H_s].
 \label{eq:supply-local-residuals}
\end{align}
The bias residual is \eqref{eq:bias-dependent-work}, with $\mathcal W[u_bi_b]$ additionally retained when the converter is on. The thermal residual compares $\Delta E_\theta$ with the separate integrals of each receiving heat and the outward ambient port. The plant residual includes $\mathcal W[P_a]$ only for this declared candidate realization; the listed-port residual \eqref{eq:coupling-residual} remains a separate comparison.

Multiplying each state equation by its conjugate effort proves these conditional identities. Adding only after integration cancels the common internal works in pairs. The boundary containing the plant, supply, sensor, line losses and thermal reservoir then has
\begin{align}
 r_{\mathrm{all}}={}&\Delta E_{\mathrm{all}}-
 \bigl(\mathcal W[Uj]+\mathcal W[v_si]+\mathcal W[F_sv]
       +\mathcal W[-c_\ell v^2]+\mathcal W[-Q_{\mathrm{amb}}]\bigr).
 \label{eq:supply-combined}
\end{align}
This is zero for an exact solution of the full declared model. The controller boundary containing only the bias coil and DC link instead retains charger-terminal work, actuator reaction, converter/copper/leakage losses, sensor supply and logic loss separately. Thus $V_bj$, rather than $Uj$, is its charger port; the source-line loss is outside that smaller boundary. This distinction remains relevant when the source command is zero.

The exact derivation establishes the model's internal consistency without a numerical integration error. It leaves specific physical and uncertainty questions open: whether the coil reaction is realized; whether each DC-link interval and its integrated demand agree; whether thermal endpoints can be independently reconstructed; and whether finite work evaluations resolve each transfer on stable or unstable prefixes. A coil identity or paired transfer cancellation does not resolve DC-link or thermal uncertainty. A combined complete-path result cannot replace those local checks. Retain positive and negative residuals and absolute as well as relative uncertainty on growing prefixes; finite supply ratings, depletion, saturation and unmodeled converter dynamics delimit how far any such prefix represents a physical system. No convergence or hardware result follows from writing an exact conditional identity.

## Four-node reference controllers and nested accounts
\label{sec:compound-driver}

The two-node receiver controls in Appendix \ref{sec:reference} admit explicit trajectories and event certificates. This four-node realization specifies a larger connection, the 28 finite sensor, actuator and supply coordinates, and their local powers. It supplies a separate implementation model for the same reference question.

### Compound states, controls and physical boundaries
\label{sec:compound-states}

A finite compound network has nodes $A,B,C,P$ and four oriented winding branches $A\to C$, $P\to C$, $B\to C$, $P\to C$. Let $\mathsf B$ be its node--branch incidence matrix, positive at each branch origin, $\mathsf C$ its positive diagonal node-capacitance matrix and $j$ its external node-current vector. For two coupled pairs $X=A,B$, take signed nonzero ratios $h_X$, $L_0,R_0>0$ and $|\kappa|<1$:
\begin{align}
 \mathsf C\dot v&=j-\mathsf B i,&
 \mathsf L\dot i&=\mathsf B^Tv-\mathsf R i,\nonumber\\
 \mathsf L_X&=L_0
 \begin{pmatrix}h_X^2&\kappa h_X\\\kappa h_X&1\end{pmatrix},&
 \mathsf R_X&=R_0\diag(h_X^2,1).
 \label{eq:compound-state}
\end{align}
The pair matrices form block diagonals. Four node voltages and four winding currents give eight independent continuous states when all nodes are dynamic. Holding one node at a compatible ideal reference removes one capacitive coordinate and gives seven; several capacitors sharing a node contribute stores without creating additional independent voltages. Generic scalar order is at most the state dimension and still depends on controllability, observation and initialized cancellations.

With $\omega=v/\alpha$, $z=\mathsf Li/\alpha$, $\mathsf J=\alpha^2\mathsf C$, $\mathsf K=\alpha^2\mathsf L^{-1}$ and $\tau=\alpha j$, the mechanical equations are
\begin{equation}
 \mathsf J\dot\omega=\tau-\mathsf B\mathsf Kz,\qquad
 \dot z=\mathsf B^T\omega-\frac{\mathsf R}{\alpha^2}\mathsf Kz.
 \label{eq:compound-mechanical}
\end{equation}
This is an exact finite inertia--elastic-state correspondence, not a rigid ideal gear. Its store is both $v^T\mathsf Cv/2+i^T\mathsf Li/2$ and $\omega^T\mathsf J\omega/2+z^T\mathsf Kz/2$. Each node power $v_Xj_X=\omega_X\tau_X$ and each winding heat $-R_bi_b^2$ is separately integrated. Direct differentiation proves the full conditional residual zero. Shaft and mesh diagnostics alone omit inertia, elastic and resistive accounts; a support constraint can carry force or torque while doing zero work at its held coordinate.

For example, a carrier source behind $R_s$ and two receiver paths, one to ground and one to the carrier, contribute $ui_s$, $-R_si_s^2$, $-G_gv_F^2$ and $-G_n(v_F-v_C)^2$. Four winding losses, a probe $-G_pv_F^2$ and a reset path $-G_rv_F^2$ complete ten separately integrated powers. Retain distinct preparation, operation, receiver-change, relaxation and reset intervals with independently evaluated endpoint stores. Changing finite conductances with all current paths retained leaves the states continuous and has no ideal impulsive work. Rewiring a charged capacitor or opening an energized winding is a different event.

For a physical common reference $r$, let $w=v-\mathbf1r$ and install four compensation currents $-\mathsf C\mathbf1\dot r$. Then
\begin{equation}
 \mathsf C\dot w=j-\mathsf B i-\mathsf C\mathbf1\dot r,\qquad
 \mathsf L\dot i=\mathsf B^Tw-\mathsf Ri.
 \label{eq:compound-reference}
\end{equation}
Since $\mathsf B^T\mathbf1=0$, this reproduces \eqref{eq:compound-state} for $v=w+\mathbf1r$ from compatible initial data. Each receiver capacitor sees a node-source power $w_Xj_X$ and a compensation power $-C_Xw_X\dot r$. The reference conductor's net ideal bias current is zero by node balance, not by assuming these individual powers vanish. A prescribed $r(t)$ is distinct from a state-dependent command $r=\chi(t)v_S$: the latter needs the actual selected node state and $\dot r=\chi\dot v_S+\dot\chi v_S$. Its exact algebraic tracking relation restricts initialization and is not an additional free state.

Finite-bandwidth sensors, inductive current actuators, the command capacitor, reference-driver capacitor and supply rail replace that constraint by dynamical equations. The finite controller in Appendix \ref{sec:finite-controller} gives a 28-state realization with separately declared receiver, actuator, sensor, driver, converter and rail accounts. Its finite capacitances, current limits and conversion losses need not preserve ideal reference tracking or the ideal scalar order. At supply cutoff its remaining stores do not disappear. A resolved local residual survives even if receiver and supply remainders cancel in a combined account.

The capacitor-cell correspondence and finite ramp integrals are established exact model results. The physically unresolved questions concern actual compensation currents, reference tracking, independent supply work, initial-state preparation, nonideal return paths and signed local residuals. A compound measurement adds independently calibrated node and winding channels to the same volt/current/endpoints approach; it cannot borrow the small cell's uncertainty bound. Finite apparatus limits, nonlinear driver events and general electromechanical correspondence remain open. The exact constrained and prepared limits in Appendix \ref{sec:compound-limits} delimit, rather than erase, these questions.

### Ideal reference controller and rail

The receiver \eqref{eq:compound-state} and reference cell \eqref{eq:compound-reference} specify different levels of implementation. An ideal state-dependent controller imposes $r=\chi v_S$ with compatible initial data, and four ideal node-current sources plus four compensation sources drive the receiver. A ninth ideal bidirectional converter supplies the reference driver's command voltage $u=r+R_dC_d\dot r$. If $P_k$ is the separately declared output power of converter $k$, a finite rail with capacitance $C_s$ and controller conductance $G_q$ obeys
\begin{equation}
 C_sV_s\dot V_s=-\sum_{k=1}^{9}P_k-G_qV_s^2,\qquad
 E_{\mathrm{rail}}=\frac12C_sV_s^2,\qquad V_s>0.
 \label{eq:ideal-reference-rail}
\end{equation}
For the receiver outputs, $P_k=w_Xj_X$ or $-C_Xw_X\dot r$; the driver output is $uj_d$. Input and output work agree only for these explicitly lossless converter laws. Tracking is an imposed constitutive relation, not a consequence of the rail balance. Controller heat and each converter transfer are integrated separately; the rail endpoint is evaluated from $V_s$. Source and controller ratings constrain the admissible trajectory before its energy audit.

### Finite sensing, actuation and conversion
\label{sec:finite-controller}

A finite implementation instead has four receiver voltages $w_X$, four winding currents, nine RC sensor voltages $z_a$, eight actuator currents $j_b$, command voltage $u$, reference voltage $r$ and rail voltage $V_s$: 28 independent regular coordinates before any additional ideal constraints. The nine sensed quantities are four absolute node voltages $w_X+r$, four winding currents and driver current. Current channels require a calibrated conversion factor $\beta$ with units $\mathrm{V\,A^{-1}}$; for example $\beta=1/10\ \mathrm{V\,A^{-1}}$ is an illustrative assumption, not a dimensionless current-to-voltage identity. With rail-limited sensor targets $\xi_a$,
\begin{equation}
 I_a=\frac{\xi_a-z_a}{R_a},\qquad
 C_a\dot z_a=I_a,\qquad
 E_a=\frac12C_az_a^2.
 \label{eq:compound-sensor}
\end{equation}
The separately integrated inward powers are $\xi_aI_a$ and $-R_aI_a^2$. The transduction input is nonloading under this model; a physical input impedance requires additional receiver ports. Equivalently, on a smooth target interval one may use $\ell_a=(\xi_a-z_a)/(R_aC_a)$ with $\dot\ell_a=(\dot\xi_a-\ell_a)/(R_aC_a)$ and $z_a=\xi_a-R_aC_a\ell_a$. Compatibility of this changed coordinate is essential; it does not change sensor storage or eliminate its state.

From a selected voltage sensor, set $r_\star=\chi z_S$ and $\dot r_\star=\chi\dot z_S+\dot\chi z_S$. External-current targets use the sensed receiver state; a finite holding servo uses the sensed primary current minus a specified conductance times the sensed held-node voltage. Four other targets are $-C_X\dot r_\star$. Thus finite holding error and finite compensation error are part of the dynamics, not suppressed constraints.

Each of the eight actual source currents passes through its own inductor $L_b$ and resistor $R_b$. A declared local feedback law with time constant $\tau_b$ gives
\begin{align}
 e_{b,\mathrm{raw}}&=w_X+R_bj_b+
                    \frac{L_b}{\tau_b}(j_{b,\star}-j_b),\nonumber\\
 e_b&=\operatorname{clip}(e_{b,\mathrm{raw}},-\gamma_bV_s,\gamma_bV_s),
 &L_b\dot j_b&=e_b-w_X-R_bj_b.
 \label{eq:compound-actuator}
\end{align}
Here $0<\gamma_b\leq1$ is a declared voltage limit. The store is $L_bj_b^2/2$, and its three inward powers are $e_bj_b$, $-w_Xj_b$ and $-R_bj_b^2$. Adding four external and four compensation currents into the receiver yields
$\mathsf C\dot w=j_{\mathrm{ext}}+j_{\mathrm{comp}}-\mathsf Bi$.
Source/load coefficients now command regenerative actuators; they are not silently counted as passive source or load resistors. The separate passive circuit remains the one preceding \eqref{eq:compound-reference}.

The command capacitor and physical driver satisfy
\begin{align}
 C_u\dot u&=J_u-j_d,&
 J_u&=\widehat j_d+\frac{C_u}{\tau_u}(u_\star-u),\nonumber\\
 u_\star&=\operatorname{clip}(r_\star+R_dC_d\dot r_\star,
                              -\gamma_uV_s,\gamma_uV_s),&
 j_d&=(u-r)/R_d,\qquad C_d\dot r=j_d.
 \label{eq:compound-command}
\end{align}
The sensed driver current $\widehat j_d$ is reconstructed using its calibrated $\beta$. The command boundary has store $C_uu^2/2$ and powers $uJ_u,-uj_d$. The driver boundary has store $C_dr^2/2$ and powers $uj_d,-R_dj_d^2$; ideal floating-network bias transfer is zero. The driver capacitor is additional to the receiver's carrier capacitance.

Eighteen converters supply eight actuators, nine sensors and the command capacitor. For each separately declared output power $P_{\mathrm{out},k}$, let $0<\eta_k\leq1$ and
\begin{equation}
 P_{\mathrm{in},k}=
 \begin{cases}
 P_{\mathrm{out},k}/\eta_k,&P_{\mathrm{out},k}\geq0,\\
 \eta_kP_{\mathrm{out},k},&P_{\mathrm{out},k}<0.
 \end{cases}
 \qquad H_k=P_{\mathrm{in},k}-P_{\mathrm{out},k}\geq0.
 \label{eq:converter-efficiency}
\end{equation}
Each converter has separately integrated input, negative output and negative heat powers. It has no store in this constitutive idealization; switching filters or semiconductor thermal dynamics would add states. This efficiency law specifies the transfer before any residual is evaluated.

Writing $q=V_s^2$ avoids division by rail voltage inside the stated positive-voltage range:
\begin{equation}
 \dot q=-\frac2{C_s}\left(\sum_{k=1}^{18}P_{\mathrm{in},k}+G_qq\right),
 \qquad E_{\mathrm{rail}}=\frac12C_sq,\qquad V_s\geq V_c>0.
 \label{eq:compound-finite-rail}
\end{equation}
The inward rail powers are the eighteen $-P_{\mathrm{in},k}$ and $-G_qq$. The combined circuit exports 41 distinct heats: four winding, eight actuator, one driver, nine sensor, eighteen converter and one controller heat. This port count is not its state dimension. Independent receiver, actuator, sensor, command, driver, converter and rail accounts are retained before canceling internal transfers in the combined boundary. The ideal mechanical comparator has its own shaft, accelerating-reference and mobility-loss integrals and independent endpoints. A zero residual in each model does not imply equal port works between the models.

### Preparation, cutoff and fast transfers

Prepare the isolated rail from zero voltage using constant current $j_p=C_sV_0/T_p$ through a resistor $R_p$ for a finite chosen time $T_p$. The source voltage is $u_p=V_0t/T_p+R_pj_p$. Direct integration gives
\begin{equation}
 W_p=\frac12C_sV_0^2+\frac{R_pC_s^2V_0^2}{T_p},\qquad
 W_{R_p}=-\frac{R_pC_s^2V_0^2}{T_p},\qquad
 E_0=0,\quad E_1=\frac12C_sV_0^2.
 \label{eq:rail-preparation}
\end{equation}
The exact preparation residual is zero; preparation is not inferred from a desired energy budget. Receiver, sensor and actuator initial states must be specified separately.

An exact zero-drive cutoff control initializes every other state at zero. Then all converter powers vanish and
\begin{equation}
 q(t)=V_0^2e^{-2G_qt/C_s},\quad
 t_c=\frac{C_s}{G_q}\log\frac{V_0}{V_c},\quad
 W_q(0,t)=-\frac12C_sV_0^2(1-e^{-2G_qt/C_s}).
 \label{eq:rail-cutoff}
\end{equation}
Independent endpoints are $C_sV_0^2/2$ and $C_sV_c^2/2$ at cutoff, so the residual is zero and the remaining store is positive. For $C_s=1\ \mathrm F$ and $V_c=1/100\ \mathrm V$ it is $1/20000\ \mathrm J$. An active-drive cutoff generally retains receiver and actuator stores too. Shutdown, reset and the event's timing uncertainty require their own intervals; termination of the operating equations does not set their endpoints to zero.

Fast same-sign transfers need not have an interior power zero. For example the exact positive pulse $P(t)=P_0e^{-t/\tau}$ has work $P_0\tau(1-e^{-T/\tau})$ on $[0,T]$. A procedure that finds every sign change but does not resolve this scale can miss its work. Opposite actuator and rail errors may cancel in the combined account. Likewise an inaccurate rail endpoint can dominate a residual even when the port-work sum changes little. These are distinct uncertainty mechanisms, not evidence for a new transfer; a resolved physical residual still requires an independent account.

A specified approach to the ideal controller may take sensor and actuator time constants proportional to $\varepsilon^2$, actuator inductances and command capacitance proportional to $\varepsilon$, sensor capacitances proportional to $\varepsilon^2$, actuator resistances proportional to $\varepsilon$, and $\eta=1-c\varepsilon$ with $0\leq c\varepsilon<1$. Receiver coefficients, the RC driver and finite rail remain fixed. These simultaneous choices do not prove uniform tracking or work convergence: clipping, prepared fast states, rail depletion and persistent tracking error require bounds on the complete interval. The linear event enclosure in Appendix \ref{sec:compound-events} is not a certificate for this nonlinear limited driver. Hardware error and global nonlinear event completeness remain open.

# Finite implementations, events and service
\label{app:implementation}

These exact constructions preserve constrained preparations, event laws, thermal boundaries and the separate scope of service, cycle and observation results.

## Constrained and prepared limits of the compound network
\label{sec:compound-limits}

Singular component values change the equation class. A descriptor system $\mathsf E\dot x=\mathsf Ax+b$ at singular $\mathsf E$ requires its algebraic constraints and compatible initial charge/flux before an ODE order is assigned. Setting a capacitance to zero imposes node-current balance; setting source resistance to zero imposes a voltage clamp. Neither operation allows arbitrary initial voltage. A zero signed winding ratio changes topology rather than giving the regular inverse in \eqref{eq:compound-state}.

### Perfect coupling retains a magnetizing state

For one pair at $\kappa=1$, put $a=(h,1)^T$ so $\mathsf L=L_0aa^T$. Compatible flux is $\lambda=a\phi$. With positive winding resistance matrix $\mathsf R$ and winding effort vector $u$, KVL and $a^Ti=\phi/L_0$ imply
\begin{equation}
 \dot\phi=\frac{a^T\mathsf R^{-1}u-\phi/L_0}
                 {a^T\mathsf R^{-1}a},\qquad
 i=\mathsf R^{-1}(u-a\dot\phi),\qquad
 E_\phi=\frac{\phi^2}{2L_0}.
 \label{eq:perfect-coupling-state}
\end{equation}
This still has a dynamic magnetic state. Its source works are the individual $\int u_ji_j\,\dd t$ and its heat works the individual $-\int R_ji_j^2\,\dd t$; endpoint flux determines the store independently. Reversing the coupling sign changes $a$ consistently. Removing resistance, magnetizing inductance and capacitance in a joint limit is a different constrained problem.

An energized voltage clamp illustrates why continuity and event work cannot be guessed. Connect a capacitor initially at $v_-$ to fixed voltage $U$ through $\rho>0$. For $t\geq0$,
\begin{align}
 v(t)&=U+(v_--U)e^{-t/(\rho C)},&
 i(t)&=(U-v_-)\rho^{-1}e^{-t/(\rho C)},\nonumber\\
 W_U(0,T)&=CU(U-v_-)(1-e^{-T/(\rho C)}),&
 W_\rho(0,T)&=-\frac C2(U-v_-)^2(1-e^{-2T/(\rho C)}).
 \label{eq:energized-clamp}
\end{align}
Independently use $E_0=Cv_-^2/2$ and $E_T=Cv(T)^2/2$; their difference minus both works is zero. For a completed layer, the source share is $CU(U-v_-)$ and the heat share $-C(U-v_-)^2/2$, while the endpoint change is $C(U^2-v_-^2)/2$. Taking $\rho\to0$ after retaining these integrals does not erase them. A bounded-voltage inductor retains continuous flux; a discontinuous flux needs its own impulse law. Mechanical rate clamps have the corresponding momentum and kinetic-store constraints. Finite locking friction, impact and magnetic saturation are additional physical laws.

Similarly, \eqref{eq:reference-ramp-work} retains a resistor work proportional to $-1/T$ at fixed $R_d,C_d,\Delta r$. A zero-duration reference shift is not a finite-work limit of that fixed driver. The measured finite-duration predictions remain valid under their stated component and supply limits.

### A specified rigid family and its hidden preparations

For $0<\varepsilon\leq1$ set $L_0=\ell_0/\varepsilon$, $\kappa=1-\varepsilon^2$, $R_0=r_0\varepsilon^2$, and node capacitances $\mathsf C=\varepsilon\mathsf C_0$, with fixed positive $\ell_0,r_0,\mathsf C_0$ and fixed nonzero ratios. For one pair define $p=hi_1$, $q=i_2$, common current $s_c=p+q$ and differential current $d_c=p-q$. The exact independent winding equations and store are
\begin{align}
 L_+\dot s_c&=S-R_0s_c,& S&=u_1/h+u_2,&
 L_+&=\ell_0(2-\varepsilon^2)/\varepsilon,\nonumber\\
 L_-\dot d_c&=D-R_0d_c,& D&=u_1/h-u_2,&
 L_-&=\ell_0\varepsilon,\nonumber\\
 E_{\mathrm{pair}}&=\frac14(L_+s_c^2+L_-d_c^2).
 \label{eq:compound-modal-limit}
\end{align}
Here $d_c$ denotes this appendix's differential current, not a contact damping coefficient. Both modes retain their independently prepared initial values:
\begin{equation}
 y(t)=y(0)e^{-R_0t/L_\pm}
       +\frac1{L_\pm}\int_0^te^{-R_0(t-\xi)/L_\pm}f(\xi)\,\dd\xi,
 \quad (y,f)=(s_c,S)\ \hbox{or}\ (d_c,D).
 \label{eq:compound-modal-solution}
\end{equation}
This exact convolution, not a truncated expansion, determines what survives.

For matched constant winding efforts $u_1/h=u_2=U$ and $s_c(0)=0$,
$s_c=2U(1-e^{-R_0t/L_+})/R_0$ and $d_c=d_c(0)e^{-R_0t/L_-}$. The identity $1-e^{-z}=\int_0^ze^{-u}\dd u\leq z$ gives, uniformly on $[0,T]$,
\begin{equation}
 |s_c(t)|\leq\frac{2|U|T}{L_+},\qquad
 |d_c(t)-d_c(0)|\leq
 |d_c(0)|\frac{R_0T}{L_-}.
 \label{eq:matched-mode-bounds}
\end{equation}
For bounded initial differential current both magnetic stores vanish along this matched family. Bounded voltages also make the capacitive stores vanish. This is a conditional reduction, not a claim about arbitrary preparation or drive.

For an explicit finite preparation, ramp isolated winding currents from zero to $i_0$ linearly over $[0,T_p]$, with source efforts $u=\mathsf Li_0/T_p+\mathsf Ri_0t/T_p$. Each source and heat work is
\begin{equation}
 W_{u,j}=\frac12i_{0,j}(\mathsf Li_0)_j+
             \frac{T_p}{3}R_ji_{0,j}^2,\qquad
 W_{R,j}=-\frac{T_p}{3}R_ji_{0,j}^2.
 \label{eq:compound-preparation}
\end{equation}
Independent magnetic endpoints are zero and $i_0^T\mathsf Li_0/2$. A separate linear voltage ramp from zero to $v_{0,X}$ at each capacitor has signed source work $C_Xv_{0,X}^2/2$ and the same independently evaluated final store. The complete preparation residual is zero under these ideal finite drives. Reconnection with continuous capacitor voltages and winding fluxes and compatible secondary currents has no imposed impulse; real switching needs a measured finite path. On the matched family the extra planet clamp and copper losses tend to zero under \eqref{eq:matched-mode-bounds}, but their finite works remain part of every finite account.

An independently imposed common preparation $s_c(0)=s_*\varepsilon^p$ instead gives exactly
\begin{equation}
 E_+(0)=\frac{\ell_0s_*^2}{4}
              (2-\varepsilon^2)\varepsilon^{2p-1}.
 \label{eq:prepared-common-store}
\end{equation}
It vanishes for $p>1/2$, tends to $\ell_0s_*^2/2$ for $p=1/2$, and grows without bound for $p<1/2$ when $s_*\ne0$. At $p=1/2$ the current tends to zero while a finite store remains; at $p=0$ a fixed common current carries a diverging store in this ideal parameter family. Opposed common preparations in a compound assembly may cancel in selected terminal observations without canceling either store. Their finite preparation paths, component ratings and signed source-return works must be evaluated, not inferred from apparent rigid motion.

A small drive mismatch can survive as well. With $d_c(0)=0$ and constant $D=D_*\varepsilon^q$,
\begin{equation}
 d_c(t)=\frac{D_*\varepsilon^q}{R_0}
                    (1-e^{-R_0t/L_-}),\qquad
 \frac{L_-d_c(t)}{D_*\varepsilon^qt}
 =\frac{1-e^{-z}}z,\quad z=R_0t/L_-.
 \label{eq:drive-mismatch-limit}
\end{equation}
For fixed $t>0$ and $D_*\ne0$, the last ratio tends to one. Consequently the current tends to zero for $q>1$, to $D_*t/\ell_0$ for $q=1$, and grows for $q<1$. Its differential store tends to $D_*^2t^2/(4\ell_0)$ when $q=1/2$, even though the effort mismatch tends to zero. For nonconstant drive, the signed convolution, including cancellation and initialization, replaces this constant-drive conclusion.

### Passive loading and fast-layer conditions

For a held member of ratio $h_H\ne0$ and free member of ratio $h_F$, the ideal rigid voltage relation is $v_F=a v_C$, $a=1-h_F/h_H$. Retain a passive source resistor $R_s$, a receiver conductance $G_g$ to ground and $G_n$ to the carrier. Their matched static solution is
\begin{equation}
 v_C=\frac{u}{1+R_s[G_ga^2+G_n(a-1)^2]},\qquad
 v_F=av_C,\qquad
 i_F=-[G_ga+G_n(a-1)]v_C.
 \label{eq:compound-passive-limit}
\end{equation}
This follows directly from constrained node balance and each receiver's current law. Different receiver connections change both the loading and finite dynamics. Matching a prescribed winding drive does not establish this passive-source limit.

For the differential fast subsystem, let $\mathsf B_-$ be the differential-mode incidence after the held coordinate is eliminated and let $\mathsf G$ describe the retained passive conductances. Its scaled matrix and positive metric are
\begin{equation}
 \mathsf F_f=
 \begin{pmatrix}
 -\mathsf C_0^{-1}\mathsf G&-\mathsf C_0^{-1}\mathsf B_-\\
 (2/\ell_0)\mathsf B_-^T&0
 \end{pmatrix},\qquad
 \mathsf H_f=\diag(\mathsf C_0,(\ell_0/2)\mathsf I).
 \label{eq:compound-fast}
\end{equation}
Direct multiplication gives $\mathsf F_f^T\mathsf H_f+\mathsf H_f\mathsf F_f=\diag(-2\mathsf G,0)$. Strict decay requires the absence of a nonzero invariant undamped subspace; positive semidefinite dissipation alone is insufficient. If this condition makes $\mathsf F_f$ Hurwitz, constants $M,\gamma>0$ give $\|\exp(\mathsf F_ft/\varepsilon)\|\leq M e^{-\gamma t/\varepsilon}$. Variation of constants then bounds forced deviations when the forcing and compatible slow states are bounded. Initial layers remain at $t=0$ unless prepared away. Degenerate geometry, unmatched forcing, precharged fast stores or a changing limiting constraint need separate analysis.

These limits distinguish convergence of node rates, of winding currents, of separately integrated port works and of endpoint stores. None implies the others without its own bounds. A favorable signed-work comparison can coexist with large hidden stores or a different current history. Exact finite initial-state formulas retain those alternatives as physical preparation and measurement questions.

## Exact events and their model-specific scope
\label{sec:compound-events}

On any fixed linear switching interval let $\dot x=\mathsf F(t)x+b(t)$ with affine analytic coefficients. Augmenting by a constant coordinate reduces it to a homogeneous analytic system. An instantaneous power is then a linear or quadratic analytic observable. Lifting the quadratic monomials and adjoining work coordinates also gives a linear analytic system when discussing equalities between integrated works. A zero of an individual power, equality of two absolute powers, and a physical change of circuit law are different events.

To enclose events exactly, expand an observable $f$ about a center $c$ in its convergent Taylor series. Suppose it is analytic on the complex disk $|t-c|\leq\rho$ with $|f|\leq M_f$. For an affine matrix $\mathsf F(t)=\mathsf F(c)+(t-c)\mathsf F_1$, a state norm bound on that disk is $\|x(c)\|\exp(\|\mathsf F(c)\|\rho+\|\mathsf F_1\|\rho^2/2)$; the observable's declared linear or quadratic form gives $M_f$. Cauchy's coefficient bound yields, for $q=|t-c|/\rho<1$,
\begin{align}
 \left|f(t)-\sum_{k=0}^Na_k(t-c)^k\right|
 &\leq \frac{M_fq^{N+1}}{1-q},\nonumber\\
 \left|f'(t)-\sum_{k=1}^Nk a_k(t-c)^{k-1}\right|
 &\leq\frac{M_f}{\rho}
       \frac{q^N[(N+1)-Nq]}{(1-q)^2}.
 \label{eq:event-analytic-bounds}
\end{align}
These are exact convergent-series remainder bounds, not an asserted unbounded-domain polynomial approximation. A value enclosure excluding zero proves no root in its interval. Opposite endpoint signs together with a derivative enclosure excluding zero certify one crossing. Tangencies require a separate multiplicity or factor argument; a sign-change search alone misses them.

For a power product, retain zeros of both effort and flow. For absolute-power comparisons, factor the equality into $P_j-P_k=0$ or $P_j+P_k=0$. Identical factors give persistent ties rather than isolated roots. Overlapping enclosures of different factors do not prove coincident roots; an exact relation $f(t)=c(t)g(t)$ with $c$ finite and nonzero throughout the interval does preserve their zeros and multiplicities. Between a complete set of enclosed events, signs and maximizing branches remain fixed; each signed port work is integrated before any maximum or ratio is formed. Integrals over the root enclosures themselves remain in the partition and add with the root-free pieces. A ratio with zero denominator is undefined, including zero divided by zero. Extra apparent crossings from finite observation error do not supply physical switching times.

For example define terminal and internal diagnostics $T(t)=\max_X|v_Xj_X|$ and $C(t)=\max_b|e_bf_b|$ over explicitly named mechanical core ports. Their ratio compares those lists, not whole-system energy. A finite network's shaft, mesh and pin powers need not exhaust its store/heat account. For pair $X$, denote its primary and secondary mechanical branch torques by $f_X$ and $\widetilde f_X$. The extra mesh couple is $m_X=\widetilde f_X+h_Xf_X$, while the carrier pin torque includes $J_{\mathrm{orb}}\dot\omega_C+(h_A-1)f_A+(h_B-1)f_B$, with orbital inertia $J_{\mathrm{orb}}$. Orbital acceleration, these extra couples and the chosen frame must be retained before comparing the core diagnostics. Summed charging current requires the corresponding reference return when node-power reference invariance is invoked.

Exact reversal histories supply controls independent of root searching. For a single inertia $J=1$ with zero initial velocity, $\tau=1-2t$ on $[0,1]$ gives $\omega=t-t^2$, zero endpoint stores and signed shaft works $+1/32$ and $-1/32$ on its two half intervals. Thus zero total work does not mean zero intermediate transfers.

For the lossless compound receiver, choose $v=u\,a(t)$, where $u$ is a fixed node-voltage vector and the scalar polynomial $a$ vanishes at both endpoints with $\int_0^Ta(t)\dd t=0$. Put $A(t)=\int_0^ta(\xi)\dd\xi$ and initialize zero winding flux. Then
\begin{equation}
 \lambda=\mathsf B^Tu\,A,\qquad
 i=\mathsf L^{-1}\mathsf B^Tu\,A,\qquad
 j=\mathsf Cu\,\dot a+\mathsf B\mathsf L^{-1}\mathsf B^Tu\,A.
 \label{eq:compound-reversal}
\end{equation}
Each node's source power is a fixed linear combination of $a\dot a$ and $aA$; its integral is zero separately since $a$ and $A$ vanish at both endpoints. Every capacitor and winding endpoint store is independently zero. Subinterval works can be nonzero. On normalized $[0,1]$, $a=t(1-t)(1-2t)$ gives $A=t^2(1-t)^2/2$. The distinct choice $a=t(1-t)(3t-1)^2(7t-5)/63$ has an interior double zero at $t=1/3$ and primitive $A=-t^2(t-1)^2(21t^2-18t+5)/126$; the identically zero profile is a third case. A planet node can be left without injection if both $e_P^T\mathsf Cu=0$ and $e_P^T\mathsf B\mathsf L^{-1}\mathsf B^Tu=0$. These are explicit preparation and forcing conditions, not a universal zero-work statement. A physical moving reference additionally requires the compensation, driver and supply ports already derived; zero receiver work does not assign their work zero.

Linear drive-sign reversal with reversed compatible initial data changes states' signs but leaves quadratic powers unchanged. It supplies an exact symmetry, not an independent physical trial. Analytic event enclosures certify only the specified linear laws, coefficients and intervals. The finite-rail clipped controller is nonlinear and piecewise smooth; its saturation branches, fast same-sign transfers, cutoff and all possible tangencies require separate enclosures. Finite pointwise agreement and empirical accuracy estimates cannot establish global root completeness or hardware accuracy. The exact constructions resolve the stated bounded mathematical questions while retaining those broader open ones.

## Clocked branches, finite preparation and service comparisons
\label{sec:clocked-branches}

The following smaller circuit supplies a separate exact construction from the shared-output model. Its primary return $O$ and secondary return $B$ are isolated. A tapped secondary has upper/lower winding paths $A-T,T-B$, and node order $(A,T,X_p,Q_p,X_m,Q_m)$. Four selectors connect $A-X_p,T-X_p,T-X_m,B-X_m$. Unit receiver resistors join $X_p-Q_p,X_m-Q_m$; $1/10\ \mathrm F$ cells join $Q_p-B,Q_m-A$. Every node has $1/50\ \mathrm F$ to $B$. The source resistor is $1/5\ \Omega$ and each copper resistor $1/20\ \Omega$.

For $0<f<1$, $0\leq\kappa<1$, polarity $\sigma=\pm1$, set $N=(1,\sigma(1-f),\sigma f)^T$ and $L=(1\ \mathrm H)[(1-\kappa)\operatorname{diag}(N_j^2)+\kappa NN^T]$. The baseline $f=\kappa=1/2$, $\sigma=1$ is the three-winding matrix in Appendix \ref{sec:finite-bank-probe}. With $B$'s primary column zero and secondary columns $e_A-e_T,e_T$,
\begin{equation}
 L\dot i=B^Tv+e_1U-\operatorname{diag}(1/4,1/20,1/20)i,
 \quad C\dot v=-Bi-G(t)v-K^Ti_c(Kv),
 \label{eq:clocked-network}
\end{equation}
where $C=(1/50)I+(1/10)e_{Q_p}e_{Q_p}^T+(1/10)(e_{Q_m}-e_A)(e_{Q_m}-e_A)^T$ in farads. Each resistor contributes its conductance-weighted incidence outer product to $G$. Clamps on $A,T$ and both cells have threshold $2\ \mathrm V$ and slope $5\ \mathrm S$. The selector conductances range from $1/10000$ to $20\ \mathrm S$. Their prescribed command passes successively through selectors 1,2,4,3 over the four quarters of a one-second sinusoid $U=\sin(2\pi t)\ \mathrm V$.

Use $s(r)=r^2(3-2r)$ over a declared edge width. Simultaneous change interpolates old to new; dead time opens the old path during the first half and closes the new during the second, while overlap reverses that order. Widths $1/50,1/100,1/200\ \mathrm s$ define distinct finite histories, not a proved common zero-width limit. Initial currents $(1/10,1/5,-1/10)\ \mathrm A$, $Q_p=Q_m=3\ \mathrm V$ and other states zero give an energized/clamped comparison. Zero-state startup is a different preparation. All winding sections persist; finite selectors change no inductance matrix and impose no state jump. Gate circuits each retain $1/10000\ \mathrm F$ driven through $20\ \Omega$, with their own command-current powers. As in the bank construction, gate voltage and prescribed selector conductance are separate declared laws; physical actuation cost remains unassigned.

For two driven periods followed by one second with source/gates off and $1/5\ \mathrm S$ node bleeders, integrate source, two receivers, each selector, clamp, copper, source resistor, gate supply, gate resistor and bath on every quarter, edge and reset interval. Retained heat satisfies $\dot H=P_{\rm internal\ heat}-H/(2\ \mathrm s)$. Evaluate magnetic, both cell, parasitic, gate and thermal endpoints independently, retaining all nonzero final stores. A finite resolved transition does not also receive an ideal impulse. Positive leakage/parasitics guarantee regular equations; deleting them can impose new compatibility constraints. Arcs and calibrated semiconductor laws are outside this model.

The parallel/series bank variant uses nodes $(A,T,X_1,Y_1,X_2,Y_2)$, cells $X_1-Y_1,X_2-Y_2$ with capacitances $1/10$ and either $1/10$ or $3/20\ \mathrm F$, and a unit receiver $Y_2-B$. Finite links are $A-X_1,T-X_1,X_1-X_2,Y_1-Y_2,Y_1-X_2$. Even quarters enable charge and both parallel links; odd quarters enable injection and the series link. Retain the same winding, parasitic, clamp, driver and heat laws, with a fifth driver. The initialized unequal preparation $(1,1/2)\ \mathrm V$ does not assign its own preparation work. This graph differs from the loaded binary-probe graph in Appendix \ref{sec:finite-bank-probe}.

### What the fixed clock proves

With inactive clamps and fixed material coefficients the nine electrical coordinates obey $\dot x=A(t)x+b(t)$. Compose plateau exponentials and edge fundamental matrices to get $x(1)=Mx(0)+d$. Existence requires $d\in\operatorname{range}(I-M)$, uniqueness requires invertibility of $I-M$, and attraction requires $\rho(M)<1$. The controls $(M,d)=(I,0)$, $(I,d\ne0)$ and $(2I,d)$ give respectively neutral families, no fixed point and an unstable fixed point. A successful initialized trace alone distinguishes none of these possibilities.

For this positive, grounded graph, homogeneous difference storage satisfies $\dot D=-\delta i^TR\delta i-\delta v^TG(t)\delta v<0$. A common positive metric and uniform positive loss over the compact period give strict contraction, hence a unique attracting clocked linear state. Gate RC coordinates have their own contracting maps. If the electrical loss is periodic, heat has map $H(1)=e^{-1/2}H(0)+h$ with $h$ its independently integrated, exponentially weighted heating, and fixed value $h/(1-e^{-1/2})$. This theorem requires inactive clamps and temperature-independent coefficients throughout the orbit; no returned endpoint proves a calibrated continuous flux limit.

A threshold controller switching at $Q_p=1/100\ \mathrm V$ upward and $1/200\ \mathrm V$ downward instead has saltation $I+(f^+-f^-)n^T/(n^Tf^-)$ at a transverse continuous-state event. Grazing, tied guards and changed event count require another analysis; fixed-clock contraction does not prove full hybrid attraction. A separate soft-saturation law is $\lambda=D_\ell i+\kappa I_s\tanh(N^Ti/I_s)N$, $I_s=1/2\ \mathrm A$, with positive leakage $D_\ell$ and energy
$$
 E_m=\tfrac12i^TD_\ell i+\kappa[I_sq\tanh(q/I_s)-I_s^2\log\cosh(q/I_s)],\quad q=N^Ti,
$$
with the inductance unit understood in $\kappa$. Differentiation gives $\dot E_m=i^T\dot\lambda$. Alternatively $R_w=(1/20\ \Omega)(1+H/(100\ \mathrm J))$ adds thermal feedback with capacity $1\ \mathrm{J/K}$. Neither extension supplies remanence or validates a material law, and their amplitude-$4\ \mathrm V$ comparison requires separately solved histories.

### Service, observation and a finite mechanical counterpart

For a supply-cost comparison freeze zero initial states, source and three-second intervals above, and define service as receiver heat integrated over $[0,3]\ \mathrm s$. An ordinary comparison transformer retains both secondary sections, parasitics at $A,T$, one full-secondary resistor and finite reset bleeders. Select a receiver resistance by an independently declared service-matching condition before comparing costs. For example, order 25 geometric trial resistances from $1$ to $10000\ \Omega$ and select the first descending bracket's service-match root, if it exists. This is a conditional comparison, not a proved root or work ordering. Integrate gross source draw $\int\max(Ui_1,0)dt$, gross return $-\int\min(Ui_1,0)dt$ and every gate supply separately. Their net difference cannot be promoted to an equal-reset efficiency when actual final stores differ. No numerical sign is imported as an exact theorem.

Including a generator makes capacitor return an internal transfer. A separate exact ideal conversion control has $e=k_e\omega\sin\phi$, $\tau_e=k_ei\sin\phi$, $k_e=1/(2\pi)$ in the corresponding SI units, $\omega=2\pi\ \mathrm{s^{-1}}$, and $i=\pm\sin(2\pi t)+\cos(2\pi t)/2\ \mathrm A$ on $[0,2]\ \mathrm s$. For rotor $J=1/100\ \mathrm{kg\,m^2}$, drag $b=1/1000\ \mathrm{N\,m\,s}$ and unit field current with unit field resistance/inductance, electrical delivered work is $\pm1\ \mathrm J$, shaft input $\pm1+\pi^2/125\ \mathrm J$, field input $2\ \mathrm J$, drag and field heat exports $-\pi^2/125,-2\ \mathrm J$. Each endpoint independently has rotor store $\pi^2/50\ \mathrm J$ and field store $1/2\ \mathrm J$. This initialized ideal converter supplies no physical field/armature coenergy law for a generator.

Disconnected unit field preparation on $[0,1]\ \mathrm s$ gives $i=1-e^{-t}$, supply work $e^{-1}\ \mathrm J$, field store $(1-e^{-1})^2/2\ \mathrm J$ and Joule heat $\int_0^1(1-e^{-t})^2dt\ \mathrm J$. A prescribed rotor ramp $\omega=2\pi t$ gives endpoint $\pi^2/50\ \mathrm J$, drag heat $\pi^2/750\ \mathrm J$ and their sum as shaft work. Source-off field reset retains $i_0^2e^{-2T}/2$ and releases heat $i_0^2(1-e^{-2T})/2$ in consistent SI units. Real generator trajectories, actuator costs, reset and material states require their own model and observations.

For the fixed first charging topology, observe primary current and $V_A,V_T,V_{Q_p},V_{Q_m}-V_A$. The nine-state observability matrix has rank nine for the declared rational baseline; this is ideal-trace reconstruction, not a bandwidth or uncertainty bound. Heat preparations separated by $1\ \mathrm J$ remain electrically indistinguishable and differ by $e^{-T/2}\ \mathrm J$ if coefficients are temperature independent. A unit capacitor at $1000\ \mathrm V$ with voltage error $1/1000\ \mathrm V$ has exact endpoint error $2000001/2000000\ \mathrm J$. Small net work cannot suppress this independent endpoint uncertainty. A same-sign power pulse of height $A$ and duration $\varepsilon$ carries $A\varepsilon$ work without an internal zero; root counting alone is insufficient.

At unit mobility scale the mechanical map is $v=\omega$, $z=Li$, $J=C$ and
$$
 K=L^{-1}=\begin{pmatrix}3/2&-1&-1\\-1&6&-2\\-1&-2&6\end{pmatrix}.
$$
Six ground rotors plus two differential flywheels realize $C$; positive modal springs realize $K$. The independent equations are $J\dot\omega=-BKz-G\omega-\tau_{\rm clamp}$ and $\dot z=B^T\omega-RKz+b_{\rm anchor}$. The primary anchor moves at $U$ in the declared scale; dashpot, gate-rotor and thermal accounts follow their actual ports. General scaling is $v=\alpha_v\omega$, $z=Li/\alpha_v$, $J=\alpha_v^2C$, $K=\alpha_v^2L^{-1}$, with corresponding scaled damping and drives. This state/store map proves the linear model correspondence, including prepared states and finite events. The original rigid train has two independent rates and cannot have a state/port bijection to six arbitrary node rates without extra bodies, compliance or actuators. Physical bearings, adjustment work, bandwidth and magnetic calibration remain unresolved.

### A finite clutch retains states through release

A coaxial ball/carrier control has $I_b=2/5$, $I_c=3/5\ \mathrm{kg\,m^2}$ without orbital translation. With carrier held at unit speed and unit viscous clutch, $\omega_b=1-e^{-5t/2}$. On $[0,1]\ \mathrm s$, independent drive work, ball endpoint store and heat are $2(1-e^{-5/2})/5$, $(1-e^{-5/2})^2/5$ and $(1-e^{-5})/5\ \mathrm J$. An undriven carrier instead has $\omega_c=3/5+2e^{-25t/6}/5$, $\omega_b=3/5-3e^{-25t/6}/5$, initial kinetic store $3/10\ \mathrm J$ and heat $3(1-e^{-25/3})/25\ \mathrm J$. These are distinct preparations and boundaries.

A finite extension retains $(\omega_c,\omega_b,q,H,v_g)$ with $T_c=Kq+D(\omega_c-\omega_b)$, $\dot q=\omega_c-\omega_b$, $T_d=2(\Omega_d-\omega_c)$, $I_c\dot\omega_c=T_d-T_c$ and $I_b\dot\omega_b=T_c-\omega_b/10$ in SI units. Gate capacitance is $1/100\ \mathrm F$ with a $10\ \Omega$ supply resistor. Independently stored quantities are the two spins, $Kq^2/2$, $H$ and $v_g^2/200$. External powers are $T_d\Omega_d$, $\dot Kq^2/2$, gate supply, receiver $-\omega_b^2/10$ and bath $-H/2$; drive, clutch and gate losses heat $H$ internally. The stiffness actuator is a separate physical assumption, not a free clock.

Starting at zero, use half-cosine ramps on four one-second intervals: prepare $\Omega_d:0\to1$, $K:0\to1/5$, $D=1/10$, gate command one; lock at $(1,1/5,2)$ with command one; release $K:1/5\to0$, $D:2\to0$ at $\Omega_d=1$, command zero; then reduce $\Omega_d:1\to0$ at $K=0,D=1/2$, command zero. Damping jumps at $1,3\ \mathrm s$ change finite power, not velocities or stores. Retain actual nonzero four-second endpoints. These time-varying constitutive states delimit any scalar reduction; calibrated clutch, actuator, thermal and release laws remain open.

## Coupled thermal states and finite actuator order
\label{sec:coupled-thermal-control}

An additional thermal coordinate can change coefficients and predictions without being an energy anomaly. A declared three-state electrical, mechanical and thermal model is
\begin{equation}
 \begin{aligned}
 L\dot i&=U-R(\theta)i-kv,&m\dot v&=F+s k i-bv,\\
 C_T\dot\theta&=f[R(\theta)i^2+bv^2]-h\theta,
 &R(\theta)&=\tfrac25(1+\alpha\theta)\ \Omega.
 \end{aligned}
 \label{eq:coupled-thermal-control}
\end{equation}
Here $L=13/10\ \mathrm H$, $m=4/5\ \mathrm{kg}$, $C_T=2\ \mathrm{J/K}$, $b=3/10\ \mathrm{N\,s/m}$, $U=[\sin(23t/10)+3/10]\ \mathrm V$, $F=\cos(11t/10)/5\ \mathrm N$ on $[0,2]\ \mathrm s$. Time is in seconds; $k$ has units $\mathrm{N/A}$, $\alpha$ has units $\mathrm{K^{-1}}$, $0\leq f\leq1$ is the retained heat fraction, $h\geq0$ is a thermal conductance, and $s$ specifies backaction. Supply their values, finite initial states and the interval on which $R(\theta)>0$ independently for each prediction. Disabled coordinates and their drives are exactly zero. This nonlinear state count does not imply a constant third-order scalar equation.

The combined store is $Li^2/2+mv^2/2+C_T\theta$, with sensible heat relative to fixed ambient. Substitution identifies five external powers: $Ui$, $Fv$, controller $(s-1)kiv$, unretained heat $-(1-f)(Ri^2+bv^2)$ and bath $-h\theta$. Reciprocal transfer for $s=1$ and retained heating cancel internally. Define each work by its own integral before comparing independently evaluated endpoints. Reversing $k$ at one second retains continuous physical states and requires both event intervals. Wrong-sign backaction is supplied by the controller port; it is not automatically inadmissible. A formal identity neither validates that controller nor resolves quadrature disagreement. The relevant unresolved numerical question is whether independently reconstructed works satisfy unchanged accuracy bounds for the specified trajectory, including each side of a coefficient switch. No numerical result or zero-error certificate is asserted here.

Comparing final current with the no-thermal-feedback, no-reciprocal-transfer and uncoupled cases is a state-interaction diagnostic, not a work residual. Likewise $e^{-t}$ and $(1-a)e^{-t}+a e^{-2t}$ start at the same observed value but differ by $a(e^{-2t}-e^{-t})<0$ for $a,t>0$. Equal present output alone supplies neither hidden preparation nor future response. Mapping first-order relaxation across domains does not identify thermal, kinetic and magnetic stores with one another.

Finite actuator order supplies another exact control. For two unit masses with initial velocities $(u,v)$, actuator A changes the first velocity at rate $av/d$ for duration $d=1/4\ \mathrm s$ while the second is fixed; actuator B changes the second at rate $bu/d$ while the first is fixed. Thus $A(u,v)=(u+av,v)$ and $B(u,v)=(u,v+bu)$. The individual signed works are $auv+a^2v^2/2$ and $buv+b^2u^2/2$ in the corresponding SI normalization, evaluated at each actuator's actual starting state. In the order AB the final state is $(u+av,v+b(u+av))$; BA instead gives $(u+a(v+bu),v+bu)$. Their separately integrated polynomial powers equal their respective kinetic changes. They are finite paths without impulses, distinct from the resistive reset maps in Appendix \ref{sec:charge-reconnection}. Initial-state preparation, a loaded complete-port extension and an instantaneous limit require additional physical laws.

## A finite shared-core construction and three distinct questions
\label{sec:shared-core}

The following construction separates finite service, return of the full state and identification of prepared energy. It is a declared circuit with positive leakage and explicit probes, not an identified apparatus. Its state laws provide a reproducible example of how additional branches change the coefficient problem. A physical implementation would require independently measured material, selector and source laws.

### The connected graph, preparation and signed accounts

Use six isolated channels $j=1,\ldots,6$. Their source returns $O_j$, secondary returns $B_j$, gate returns $D_{jk}$ and receiver return $B_o$ are distinct physical conductors. No chassis or interwinding capacitance connects these returns in this model. Each source $U_j=1\ \mathrm V$ feeds a primary node $V_j$ through $1\ \Omega$. The input primary runs from $V_j$ to $O_j$; upper and lower secondary windings run from $A_j$ to $T_j$ and $T_j$ to $B_j$. Four selectors join $(A_j,X_{pj})$, $(T_j,X_{pj})$, $(T_j,X_{mj})$ and $(B_j,X_{mj})$. Output input windings run from $X_{pj}$ to $Q_{pj}$ and $X_{mj}$ to $Q_{mj}$. A $1\ \mathrm F$ positive cell joins $Q_{pj}$ to $B_j$; another $1\ \mathrm F$ cell joins $Q_{mj}$ to $A_j$, with that polarity retained throughout.

Each of the six nodes $(A,T,X_p,Q_p,X_m,Q_m)$ has a $1\ \mathrm F$ parasitic and $1/10\ \mathrm S$ bleeder to its own $B_j$. Each $V_j$ has $1\ \mathrm F$ to $O_j$. A series $10\ \Omega$ resistor and $1\ \mathrm F$ probe capacitor loads every $V_j$; its capacitor voltage is $Z_j$. The receiver node $V_o$ has a $1\ \Omega$ receiver, $1\ \mathrm F$ parasitic and the same resistor/capacitor probe to $B_o$. Clamps across $A_j-B_j$, $T_j-B_j$, each cell and $V_o-B_o$ obey $i_c(v)=\operatorname{sgn}(v)\max(|v|-5\ \mathrm V,0)/(1\ \Omega)$.

All winding resistances are $1\ \Omega$. For each of the six input cores,
\begin{equation}
 L_j=(1\ \mathrm H)\left(I+\frac{nn^T}{4}\right),\quad n=(1,1/2,1/2)^T.
 \qquad L_o=(1\ \mathrm H)\left(I+\frac{ss^T}{4}\right),\quad s=\mathbf1_{13}.
 \label{eq:shared-inductance}
\end{equation}
The second matrix describes one output core containing all twelve input windings and one receiver winding from $V_o$ to $B_o$. There is no electrical connection between the twelve windings merely because they share this core. Positive leakage and a positive common reluctance realize the declared inductance matrices; manufactured geometry, remanence and saturation ratings are additional information. The tap fraction $1/2$ is not a coupling coefficient.

Let $i$ contain the 31 physical winding currents and $v$ the 50 node/probe voltages. After eliminating the local references, let $B$ have winding incidence columns directed from positive to negative terminal. In particular the receiver-winding current enters the winding at $V_o$, so its contribution to the receiver node equation is $-i_o$. Let $a_e$ be the incidence of every resistor or cell. The capacitance matrix is $(1\ \mathrm F)I$ plus the twelve cell incidence outer products weighted by $1\ \mathrm F$. With $K$ selecting clamp voltages, the complete electrical equations are
\begin{equation}
 L\dot i=B^Tv-R_wi,\qquad
 C\dot v=-Bi-G(z)v+d(U)-K^Ti_c(Kv).
 \label{eq:shared-network}
\end{equation}
Here $G$ includes each bleeder, source resistor, receiver, probe resistor and selector $g_{jk}a_{jk}a_{jk}^T$; $d$ contains $U_j/(1\ \Omega)$ at each $V_j$. The actual source current is $I_j=(U_j-V_j)/(1\ \Omega)$, which includes parasitic and probe current.

Each gate has $C_g=1/1000\ \mathrm F$, $R_g=1\ \Omega$, $C_g\dot z_{jk}=(c_{jk}-z_{jk})/R_g$ and $g_{jk}=1/10\ \mathrm S+(9/10\ \mathrm S)z_{jk}/(1\ \mathrm V)$. Gates initially equal $(1,0,0,0)\ \mathrm V$ in each channel. At $t_e=1/800\ \mathrm s$, commands change to $(0,1,0,0)\ \mathrm V$ until $T=1/200\ \mathrm s$. After the command, $z_1=e^{-1000(t-t_e)}\ \mathrm V$, $z_2=(1-e^{-1000(t-t_e)})\ \mathrm V$, and $z_3=z_4=0$. All selectors retain at least $1/10\ \mathrm S$: this finite edge is not an ideal opening. The command changes driver current without a state jump or impulse.

For an enlarged boundary retain heat $H$, with $\dot H=P_{\rm loss}-H/(2\ \mathrm s)$, where $P_{\rm loss}$ contains every winding, source, selector, bleeder, clamp, probe and gate-resistor loss. Receiver heat is outside. There are 81 electrical, 24 gate and one thermal coordinate. This is not a constant scalar equation of order 106. The invertible $L,C$, explicit bounded gates and Lipschitz clamps give a unique global electrical solution for every finite preparation; heat follows its scalar linear law. Temperature does not alter coefficients here.

Evaluate the endpoint store independently as
\begin{equation}
 E=\frac12i^TLi+\sum_{\text{physical capacitors }e}\frac12C_e(a_e^Tv)^2
       +\frac12C_g\sum_{jk}z_{jk}^2+H.
 \label{eq:shared-store}
\end{equation}
On each side of $t_e$, integrate the six $U_jI_j$, 24 $c_{jk}(c_{jk}-z_{jk})/R_g$, receiver power $-V_o^2/(1\ \Omega)$ and bath power $-H/(2\ \mathrm s)$ separately. Each winding transfer $(b_w^Tv)i_w$ and its opposite node transfer is also defined before internal cancellation. An electrical-only boundary instead exports the individual heats and excludes $H$; these alternatives must not be combined. Probe loading and probe stores occur in both accounts.

### A finite service certificate

Initially every channel has input currents $(-1,1/5,1/10)\ \mathrm A$, output input currents $(1,1)\ \mathrm A$, secondary voltages $(1,1/2,4/5,7/10,1/5,1/10)\ \mathrm V$ and $V_j=2\ \mathrm V$. Take $V_o=1\ \mathrm V$, $i_o=-1\ \mathrm A$, and zero probe voltages and heat. The gates have the preparation above. Independently perturb plant currents and voltages by at most $1/1000$ in their $1\ \mathrm A$, $1\ \mathrm V$ scales, holding probes, gates and heat fixed. Preparation work and reset are not supplied by this endpoint specification.

In the unclamped region the scaled vector obeys $\dot x=A(t)x+b$ with $\|A\|_\infty\leq61/10\ \mathrm{s^{-1}}$, $\|b\|_\infty\leq1\ \mathrm{s^{-1}}$. The looser bounds $K_0=32\ \mathrm{s^{-1}}$, $\beta=2\ \mathrm{s^{-1}}$ give, using $e^{K_0T}\leq(1-K_0T)^{-1}$,
\begin{equation}
 \|x(t)-x_{\rm nominal}(0)\|_\infty
 \leq\rho+\frac{[K_0(2+\rho)+\beta]T}{1-K_0T}
 =\frac{331}{840},\qquad \rho=\frac1{1000}.
 \label{eq:shared-feasibility}
\end{equation}
Every relevant terminal difference stays below $1171/420\ \mathrm V<3\ \mathrm V<5\ \mathrm V$, which closes the unclamped continuation argument. Every source returns at least $509/840\ \mathrm A$; every output input winding carries at least that current; $V_o\geq509/840\ \mathrm V$. Consequently the separately integrated receiver receipt satisfies
\begin{equation}
 W_L=\int_0^{1/200}\frac{V_o^2}{1\ \Omega}\,dt
 \geq\frac{259081}{141120000}\ \mathrm J>\frac1{1000}\ \mathrm J.
 \label{eq:shared-service}
\end{equation}
This is a continuous-time finite-history result. Winding currents stay below $2\ \mathrm A$, component voltages below $3\ \mathrm V$, linkages below $19907/3360\ \mathrm{Wb}$ and common-core flux below $15223/3360\ \mathrm{Wb}$ in the stated model. These are chosen model limits, not material ratings.

Using the tighter matrix majorant gives a state radius $134/1939$ and, by applying each capacitor incidence row to $C^{-1}$ times the node equation, an all-times capacitor-current bound $187351/96950\ \mathrm A<2\ \mathrm A$. The other resistor, gate, source and receiver currents also stay below $2\ \mathrm A$. In particular $A-X_p\geq599/9695\ \mathrm V$ gives a current at least $599/96950\ \mathrm A$ in the changing full-winding selector. The certificate covers its finite commutation interval rather than only its endpoints.

The nominal initial store is $392079/8000\ \mathrm J$. Positive receiver work and source return therefore coexist with prepared stores and gate-supply input. They do not establish a complete-service efficiency. Removing output mutual inductances while preserving self-inductances changes the nominal initial store to $284079/8000\ \mathrm J$; that control is a different coupled system, not a service-matched set of separate transformers. Zero electrical/source data give zero receiver work despite gate activity. Longer windows, staggered commands, other preparations, nonlinear materials and physical commutators remain outside this certificate.

### Complete electrical observations with overlapping error sets

Keep this graph and interval. Each source probe obeys $10\ \mathrm s\,\dot Z_j=V_j-Z_j$; report $(U_j-Z_j)/(1\ \Omega)$ as the source-current channel. It is a filtered current with a known sensor preparation, not the instantaneous source current. Report $Z_o$ and $Z_o/(1\ \Omega)$ at the receiver and all source-voltage and gate-supply records. Only the six reported source-current channels have error, an arbitrary function bounded pointwise by $1/10\ \mathrm A$. Gains, timing, coefficients and initial sensor values are exact for this mathematical experiment. No calorimetry is observed.

Compare the nominal preparation with one that raises $Q_{p1}$ by $1/10\ \mathrm V$ and lowers $Q_{p2}$ by the same amount. The changed $1\ \mathrm F$ cells and parasitics give independently
\begin{equation}
 E_0=\frac{392079}{8000}\ \mathrm J,\qquad
 E_1=\frac{392239}{8000}\ \mathrm J,\qquad E_1-E_0=\frac1{50}\ \mathrm J.
 \label{eq:shared-energy-gap}
\end{equation}
Both include the $3/1000\ \mathrm J$ gate store and zero initial heat. The continuation bound with radius $1/10$ keeps both paths below clamp threshold. Their homogeneous difference satisfies
\begin{equation}
 D=\tfrac12\delta i^TL\delta i+\tfrac12\delta v^TC\delta v,\qquad
 \dot D=-\delta i^TR_w\delta i-\delta v^TG(t)\delta v\leq0,
 \quad D(0)=\frac1{50}\ \mathrm J.
 \label{eq:shared-difference}
\end{equation}
Thus every source-node voltage difference is at most $1/5\ \mathrm V$. The actual passive probe has nonnegative unit-gain impulse response and zero initial difference, so each reported current difference is at most $1/5\ \mathrm A$. Swapping channels 1 and 2 commutes with every synchronous coefficient matrix, including the finite edge. The preparation difference is antisymmetric, whereas receiver and receiver-probe outputs are symmetric. Their histories are therefore exactly equal; so are gate histories.

The midpoint of the two source-current histories is within the allowed $1/10\ \mathrm A$ error of each. With the common receiver and gate records it is one admissible complete observation for both preparations. The energy consistency interval can therefore have width $1/50\ \mathrm J$. On this specified two-preparation problem the optimal worst-case absolute error is exactly $1/100\ \mathrm J$, attained by its midpoint and forced by the triangle inequality. It exceeds a target $1/250\ \mathrm J$.

This proves a finite-error identification obstruction, not equality of every exact source trace. The time-ordered map of \eqref{eq:shared-network}, with identity state transport at the command event, includes all probe dynamics. A fixed-mode rank calculation or static voltage-sum example would not prove this history result. Smaller error, additional cell/flux or heat observations, a longer window and unknown parameters define different experiments; their discrimination remains to be established.

### Insulated machines and a full-state return obstruction

For a separate machine model retain the fixture and replace each ideal source by an armature current $a_j$ delivered through its existing $R_s=1\ \Omega$. The six generators share angle $\phi$ and speed $\omega$, with fixed offsets $\delta_j=(j-1)\pi/3$ and $\chi_j=\phi+\delta_j$. Set $L_a=L_f=1\ \mathrm H$, $M_g=1/10\ \mathrm H$, $R_a=R_f=1\ \Omega$, and $V_f=1\ \mathrm V$. Their positive joint magnetic stores and equations are
\begin{align}
 E_{gj}&=\tfrac12L_aa_j^2+\tfrac12L_ff_j^2+M_g\cos\chi_j\,a_jf_j,\\
 \begin{pmatrix}L_a&M_g\cos\chi_j\\M_g\cos\chi_j&L_f\end{pmatrix}
 \binom{\dot a_j}{\dot f_j}
 &=\binom{M_g\omega\sin\chi_j f_j-(R_a+R_s)a_j-V_j}
 {V_f-R_ff_j+M_g\omega\sin\chi_j a_j}.
 \label{eq:shared-generator}
\end{align}
The outgoing armature sign means $V_{gj}=V_j+R_sa_j$ and electrical input into the generator is $-V_{gj}a_j$. The source-node law replaces the ideal-source term by $a_j$. With $J=1\ \mathrm{kg\,m^2}$, $b=1/10\ \mathrm{N\,m\,s}$, $\tau_{\rm pm}=8\ \mathrm{N\,m}$,
$$
 \dot\phi=\omega,\qquad J\dot\omega=\tau_{\rm pm}-b\omega-\sum_jM_g\sin\chi_j a_jf_j.
$$
Differentiating $E_{gj}$ gives $-V_{gj}a_j+V_ff_j-R_aa_j^2-R_ff_j^2+M_g\omega\sin\chi_j a_jf_j$. Generator/fixture and rotor/generator transfers cancel only after their separate integrals.

The independent timing motor has angle $\theta$, speed $\Omega$, unit inertia, unit inductance and resistance, torque/back-EMF constant one in the corresponding SI units, and bearing coefficient $b_t=1/10\ \mathrm{N\,m\,s}$. Four followers have $x_k=h\cos(\theta-k\pi/2)$, $h=1/100\ \mathrm m$, stiffnesses $(1,2,3,4)\ \mathrm{N/m}$ and damping $d_k=1\ \mathrm{N\,s/m}$. Retain each spring store and write
\begin{align}
 L_t\dot i_t&=u-R_ti_t-k_t\Omega,\quad \dot\theta=\Omega,\\
 J_t\dot\Omega&=k_ti_t-b_t\Omega-\sum_kK_kx_kx'_k-\sum_kd_k(x'_k)^2\Omega.
 \label{eq:shared-timing}
\end{align}
Cam commands $c_k=(1+\cos(\theta-k\pi/2))\ \mathrm V/2$ drive the same finite RC gates. No cam-dependent capacitance is postulated. Two sensing branches, each $1\ \Omega$, $1/100\ \mathrm F$, are driven by $\sin(\phi-\theta)\ \mathrm V$ and $(\omega-\Omega)(1\ \mathrm{V\,s})$. Their capacitor voltages $q_\phi,q_\omega$ set $U_{\rm cmd}=8\ \mathrm V+q_\phi+q_\omega$; the actual motor supply obeys $C_u\dot u=(U_{\rm cmd}-u)/R_u-i_t$, with the same resistance and capacitance. Sensor and controller supply effort/current products are separate external powers. Ideal transducer laws do not establish unmeasured hardware cost.

The complete insulated assembly has 126 state coordinates and $\dot H=\sum P_{\rm internal\ loss}$, with no bath export. Include fixture, generator, rotor, motor, follower, controller, probe, gate and thermal stores. External ports are the prime mover, six field supplies, 24 cam-command supplies, controller and two sensor supplies, and receiver export. Internal source return is not an extra external input. Positive inductance eigenvalues (at least $9/10\ \mathrm H$ in each generator) and locally Lipschitz laws establish unique solutions within the declared finite operating region; no global hardware or saturation claim follows.

Freeze a next-return section $\theta=0\pmod{2\pi}$, $\Omega>0$, one timing revolution, $T\in[1/2,2]\ \mathrm s$, and admitted speeds $\Omega\in[\pi,4\pi]\ \mathrm{s^{-1}}$. A full cycle must return every non-angle physical state and relative phase, including heat. Independently of all electrical works, its caloric law gives
\begin{equation}
 \Delta H\geq b_t\int_0^T\Omega^2dt
 \geq\frac{b_t}{T}\left(\int_0^T\Omega dt\right)^2
 =\frac{4\pi^2b_t}{T}\geq\frac{\pi^2}{5}\ \mathrm J>0.
 \label{eq:insulated-obstruction}
\end{equation}
The full return map has no fixed point and hence no attracting full-state cycle in this domain. Identical nonthermal trajectories with different initial heat retain that difference while both drift upward. This bounded conclusion is resolved; electrical or shaft periodicity with heat drift, or a replacement cooling law $\dot H=P_{\rm loss}-H/\tau$, changes the question.

Where a section return is differentiable, its derivative is $D\mathcal P=[I-fn^T/(n^Tf)]DF_T$ restricted to tangent coordinates, with the heat-integral row retained. It includes event-time variation. Continuous clamp crossings have identity saltation but changed variational Jacobians; grazing and nontransverse returns need separate treatment. There is no cycle here at which stability multipliers could certify attraction. An admitted $10\ \mathrm A$ winding/field bound implies input, output and generator linkage bounds $15$, $85/2$ and $11\ \mathrm{Wb}$ and shared flux bound $65/2\ \mathrm{Wb}$, as model bounds only.

A finite account can instead start with the fixture preparation, $a_j=0$, $f_j=1\ \mathrm A$, $\phi=\theta=0$, $\omega=\Omega=2\pi\ \mathrm{s^{-1}}$, $i_t=8\ \mathrm A$, $u=8\ \mathrm V$ and zero sensor states, and integrate each named port on $[0,1/200]\ \mathrm s$. Its endpoints are obtained from the component stores, not from a work remainder. This defines an exact finite comparison without claiming a cycle or assigning rigorous uncertainty to a numerical trajectory. Physical limits, calibration and complete preparation/reset service remain separate questions.

### Controls that change the graph

For an ideal isolated winding of signed full ratio $\sigma n$, the positive branch sees $\alpha U$ with $\alpha=\sigma n$ or $f\sigma n$; the oppositely oriented branch sees $-\sigma nU$ or $-(1-f)\sigma nU$. The two tap fractions coincide only at $f=1/2$. For a series $R,C$ branch with initial $v_0$, put $d=\alpha U-v_0$, $h=e^{-T/(RC)}$. Direct integration gives $v_C(T)=\alpha U-dh$, source work $C\alpha Ud(1-h)$, exported heat $Cd^2(1-h^2)/2$, and capacitor work equal to both their difference and $C[v_C(T)^2-v_0^2]/2$. Source return requires $\alpha U(\alpha U-v_C)<0$; tap selection alone does not ensure it. At equality all work vanishes; at zero source voltage a prepared cell still heats the resistor. Unit $R,C,U$, both polarities, fractions $1,1/4,3/4$, preparations $0,2,\alpha U$ and $T=1\ \mathrm s$ are exact substitutions, without impulses.

For a common core with positive reluctance $\mathcal R$, no leakage or copper, $v_j=N_j\dot\Phi$, $v_o=N_o\dot\Phi$, $\sum N_ji_j-N_oi_o=\mathcal R\Phi$. Each input work minus output work gives $\mathcal R[\Phi(T)^2-\Phi(0)^2]/2$. The control $\Phi=t$, $N=(1,2)$, $N_o=\mathcal R=1$, $i_1=1+t$, $i_2=0$, $i_o=1$ in consistent SI units on $[0,1]\ \mathrm s$ gives input $3/2\ \mathrm J$, output $1\ \mathrm J$ and endpoint increase $1/2\ \mathrm J$. Incompatible imposed $v_j/N_j$ have no solution in this ideal graph. Finite leakage instead gives $L=\operatorname{diag}(\ell_j)+NN^T/\mathcal R$ and $\ell\dot d+Rd=v_1-v_2$ for the equal-branch current difference. With unit $\ell,R$, opposite voltages $\pm1/2\ \mathrm V$ and zero initial currents, $i=(d/2,-d/2)$, $d=1-e^{-t}$, and common flux is zero. Each source work is $(T-1+e^{-T})/4\ \mathrm J$; copper heat is $[T-2(1-e^{-T})+(1-e^{-2T})/2]/2\ \mathrm J$; final leakage store is $(1-e^{-T})^2/4\ \mathrm J$.

Distinct ideal transformers in additive series give $v_L=\sum r_jU_j$, $i_{pj}=r_ji_L$. Unit ratios, sources $(1,2)\ \mathrm V$, a $1\ \Omega$ receiver and a one-second interval give separate source works $3,6\ \mathrm J$ and receiver work $9\ \mathrm J$, with zero ideal component stores. Opening the receiver leaves $3\ \mathrm V$ and zero work. Parallel ideal secondaries instead require equal voltages; their current sharing needs additional laws. These controls do not replace the shared-core equations.

Two specified unit cells at $1\ \mathrm V$ store $1\ \mathrm J$ whether represented by a compatible parallel $1\ \mathrm V$, $2\ \mathrm F$ terminal or additive series $2\ \mathrm V$, $1/2\ \mathrm F$ terminal. Reconnection still needs finite paths. For isolated resistive equalization with $C_1=1\ \mathrm F$, $C_2=2\ \mathrm F$, $R=1\ \Omega$ and $(v_1,v_2)=(1,0)\ \mathrm V$, the solution is $(1/3+2e^{-3t/2}/3,1/3-e^{-3t/2}/3)\ \mathrm V$. Heat on $[0,1]\ \mathrm s$ is $(1-e^{-3})/3\ \mathrm J$ and stores are $1/2$, $1/6+e^{-3}/3\ \mathrm J$. A single-path zero-resistance limit does not fix a multi-path reset.

For six equal cells $v_j=a+d_j$, $\sum d_j=0$, the terminal sum is $6a$ but $E=3Ca^2+C\sum d_j^2/2$. Unit-cell preparations $(1,1,1,1,1,1)$ and $(2,0,1,1,1,1)\ \mathrm V$ have the same sum and stores $3,4\ \mathrm J$. This static control does not replace the switched-history proof above. Conversely a fixed-clock linear passive graph with uniform positive dissipation has $D(t)\leq e^{-\gamma t}D(0)$ and a unique attracting periodically forced state. Adding channels within those hypotheses does not defeat that theorem; adding a shaft or timing controller changes its assumptions.

# Measurement uncertainty, comparison guide and verification
\label{app:measurement}

These complete uncertainty calculations and comparison obligations support the main measurement conclusions. The configuration guide provides direct entry to every established example.

## Configuration guide
\label{sec:configuration-guide}

| Configuration | Boundary | Distinguishing observation | Location |
|---|---|---|---|
| I | Damped oscillator / contact | Mapped force–velocity work; release store | Appendix \ref{sec:analogy}; Section \ref{sec:contact} |
| II | Hammer–contact–joint | Anvil angle at equal hammer torque | Section \ref{sec:contact-identification} |
| III | Coefficient observation | Independent damping and weak-term response | Appendix \ref{sec:coefficient-identification} |
| IV | Resonator and shunt | Calibrated complex terminal admittance | Appendix \ref{sec:resonator-identification} |
| V | Coil and polarization | Internal branch voltages and diode guard | Appendix \ref{sec:polarization} |
| VI | Primary and absorber | Internal strain at equal terminal reaction | Appendix \ref{sec:absorber-identification} |
| VII | Prepared passive circuit | Hidden energy as capacitance vanishes | Appendix \ref{sec:singular} |
| VIII | Two-cell connection | Separate switch works at equal endpoints | Appendix \ref{sec:connection} |
| IX | Winding and clamp | Clamp work and opening-side states | Appendix \ref{sec:transformer} |
| X | Transducer and supply | Plant, coil, bias and receiving works | Appendix \ref{sec:transducer} |
| XI | Moving reference | Physical driver work | Appendix \ref{sec:reference} |
| XII | Return commutation | Old-return work and capacitor endpoints | Appendix \ref{sec:commutation} |
| XIII | Compound receiver | Supplied reference and receiver response | Appendix \ref{sec:physical-reference} |
| XIV | Rigid limiting family | Hidden prepared flux and release work | Appendix \ref{sec:compound-limits} |
| XV | Attached physical probe | Probe work and calibrated prediction gap | Appendix \ref{sec:physical-attachments} |

: Configuration lookup. The later charge, four-port and shared-core appendices are additional constructions, not renumberings of these cases.

## Measurements that discriminate the retained alternatives
\label{sec:measurements}

The comparisons below give observables for every retained question. Their types distinguish an exact identity to validate, structural nonidentifiability, competing constitutive laws, physical transfer alternatives and acquisition of a missing law. An omitted port or a coordinate relabeling is an accounting control, not a second prepared physical apparatus. A comparison supports one declared law when its calibrated observations agree with that prediction, exclude the competing predictions and retain both endpoint states and actual event sides. Overlapping intervals leave the comparison unresolved. Disagreement with both laws retains the signed work and store differences while the constitutive law or boundary is investigated. A nonzero energy remainder is a separate outcome, quantified below.

### Exact bounds for work and endpoint uncertainty
\label{sec:uncertainty}

Let true effort and flow be $e,f$ and measurements be $e+\delta e,f+\delta f$, with deterministic bounds $|\delta e|\leq\epsilon_e(t)$ and $|\delta f|\leq\epsilon_f(t)$. Expanding their product and applying the triangle inequality gives, without a small-error approximation,
\begin{equation}
 |\widehat W-W|\leq\int_{t_0}^{t_1}
 \left(|e|\epsilon_f+|f|\epsilon_e+\epsilon_e\epsilon_f\right)\dd t
 =:\epsilon_W.
 \label{eq:work-uncertainty}
\end{equation}
Known amplitude envelopes can replace the unknown $|e|,|f|$ on the right. On a smooth interval with $|\dot f|\leq M_f$, a relative clock error $\epsilon_t$ adds at most $M_f\epsilon_t$ to the flow-error bound. At a jump, use separate event-side bounds and a bounded-power integral over the uncertain event-time window; a smooth derivative bound cannot cross an unspecified discontinuity. Hardware integration error requires its own bound.

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

### Release law, destination and continuation

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

### Singular paths, switching and transformer returns

| Switching question and comparison type | Boundary readout and controlled change | Exact conditional predictions |
|:-------------------------------------|:------------------------------------------|:--------------------------------------------|
| Preparation/coscaling; physical preparations | Observe VII's endpoints and resistor work within its voltage rating | $E^+=1/2\ \mathrm{mJ}$, $W_R=-3/2\ \mathrm{mJ}$ versus zero for relaxed preparation; limiting works follow \eqref{eq:singular-work} |
| Prepared switching; physical paths | Hold VIII's prepared voltages and final state; interchange channels | $(W_A,W_B)=(-3/4,-3/16)$ versus $(-3/16,-3/4)\ \mathrm{mJ}$ |
| Partition; settled scalar result, device law open | Compare sequential/overlapping paths within the conductance ceiling | Sequential pair above versus $(-15/32,-15/32)\ \mathrm{mJ}$; equal endpoints |
| Switch/clamp law; finite laws and acquisition | Record winding, switch, clamp and receiver powers and both event-side states | IX clamp: $(v_C^+,i_2^+)=(-1,0)$ in V/A, $W_c=1/1500-\pi^2/2000\ \mathrm J$; short path: $(0,\pi/20)$, $W=-3\pi^2/8000\ \mathrm J$ |
| Joint limits/orientations; physical paths | Change finite $C_p$, duration and sign of $M$ at known preparation | Capacitor fraction $1$ at $\theta=\pi/2$, $0$ at $\theta=\pi$; canonical secondary signs reverse with $M$ |
| Physical ground/probe; finite attachment | XV's probe voltage/current, winding currents and all capacitor voltage differences | Probe work $0$ versus $-\delta_P$; initial current $0$ versus $1/1000\ \mathrm A$; five-state endpoints from \eqref{eq:attachment-generator} |
| Calibrated hardware correspondence; acquisition | Identify parameters and prepared states independently; predict both graphs with the same uncertainty sets | Compare each work and endpoint with its prediction set; waveform disagreement and signed account residual remain distinct |
| Transformer return; complete finite paths | Hold XII's preparation, source and total duration $3h$; change overlap to immediate new return | Old-return work changes by $-\delta_A<0$; all eight differences and endpoint stores follow \eqref{eq:commutation-comparison} |

: Each work is measured on its named branch. Equality of their total or of the terminal waveform does not establish equality of their partitions.

The prepared-network comparison must cover the stated component and preparation families, including charge and linkage observations separately, before a singular physical path is assigned. The two-capacitor proof already settles path dependence within its scalar model; hardware closure concerns the measured voltage-dependent switch laws and added stores. The two finite clamp models neither identify an arc nor establish a full release topology. Arc ignition/restrike and clamp release require actual branch conductance and both event-side states on the relevant finite operating interval. Finite ratio measurements cannot establish an entire continuous singular surface without an analytic bound; \eqref{eq:parasitic} supplies such an exact result only for its stated lossless cell.

For XII, $[i_s-i_1+\mu i_2-G_kv_a]/v_a=g_e$ supplies a direct overlap observation where $v_a$ is bounded away from zero. Combined conductance uncertainty below $1/2\ \mathrm S$ separates its overlap and no-overlap laws. Old-return work additionally has the strict separation $\delta_A$ at equal source duration, with budget $B_A<\delta_A/2$. Its eight-port ledger tests the complete connection; the return-capacitor and isolated tap-loop examples are subcircuit controls. A coordinate change is an accounting control, and a both-returns-open interval still requires an additional physical path. Switch-control supplies remain measured external ports beyond the ideal graph.

\Needspace{12\baselineskip}

### Controlled supply and accelerating reference

| Question and comparison type | Independently instrumented quantities | Exact conditional predictions |
|:---------------------------------|:------------------------------------------|:---------------------------------------------|
| Bias-coil transfer; receiver alternatives | X's measured force/velocity, actuator $u_ai_a$, bias $u_bi_b$, link power and all endpoints | Regenerative $\Delta E_b=3\log2/10000-3/800000\ \mathrm J$ versus dump $-3/800000\ \mathrm J$; actuator copper $27/320000\ \mathrm J$ in both |
| Reference correspondence; bounded identity and supply alternatives | XI/XIII receiver and driver supplies, shaft torque/rate, finite rail | XI receiver $1/5\ \mathrm J$ versus zero; rail input $1/5$ or $1/4\ \mathrm J$. Lossless XIII driver input $3/200000\ \mathrm J$ |
| Dissipative reference; exact event control | Add XIII's $1/10\ \Omega$ winding resistance with the specified commands; retain all power signs | Node work $1/63\ \mathrm J$, winding work $-1/63\ \mathrm J$, driver input $43/2800000\ \mathrm J$ |
| Hidden modal preparation; finite stores | XIV's separate winding preparation, source-off copper works and endpoints; compare relaxed preparation | Initial store $31/16000\ \mathrm J$, final $31/64000\ \mathrm J$, versus zero in the relaxed control |

: Supply costs and state correspondence require different measurements. A receiver balance alone determines neither converter efficiency nor the compound driver.

The transducer's force must be observed independently of its command, and actuator, bias, thermal and DC-link residuals must be evaluated separately. Each unresolved signed remainder is retained through \eqref{eq:measured-residual}. A positive coil change is compared with measured reaction and all supply paths. For the fixed-coupling receiver law, \eqref{eq:bias-efficiency} supplies the conditional sign threshold; a bias-dependent plant needs its own measured gains and resolved interval/subledger accuracy. The compound state map and both XIII receiver event certificates are settled within their declared laws; actual converter costs and other nonlinear event families retain their separate scope. XIV distinguishes retained winding energy from an erased preparation even as the common current tends to zero. A finite $1\ \mathrm V$ reference change with XI's driver predicts the works in \eqref{eq:reference-jump}; shrinking duration at fixed resistance increases required work. Signed positive and negative intervals are retained even when receiver net work is zero.

\Needspace{25\baselineskip}

### Identification and correspondence

For each row, identify the local law or whole-system equation being tested, the actual attachment and the driven and measured ports. Retain that choice through independent component changes, the calibrated time/frequency domain and prediction. A local coefficient assignment requires local information or a proved inverse from the declared channels.

| Question and comparison type | Measured comparison | Exact prediction or alternative |
|:-------------------------------------|:----------------------------------------|:------------------------------------------|
| Damped analogy; identity | I's independent mechanical and electrical preparation, free and reset works, with both body ports | Source works $(23/30,0,23e^{-\pi}/30)\ \mathrm J$ in both devices; compare through the mapped scale |
| Contact/support; structural ambiguity and inverse | Hold II's torque/hammer angle; add anvil response to separate contact and joint using \eqref{eq:contact-inverse} dynamically | Anvil $1/2$ versus $2/3\ \mathrm{rad}$ at the same hammer angle |
| Weak coefficient; model alternatives | Change III to $(\rho,\eta)=(1,2)$ with calibrated coordinates and covariance | $151/50$ versus $301/100$; separation $1/100$ |
| Resonator; shunt identity and device acquisition | Change the known parallel shunt; measure total current and common voltage, then predict other devices | IV gives $1+\ii$ versus $1+2\ii\ \mathrm S$; the transferable motional law needs separate specification |
| Hidden energy; finite-coupling bound | Internal capacitor voltage and resistor current alongside the terminal channel | $E_0\leq CR^2\epsilon_i^2/(2\nu^2)$ for known $\nu>0$; no uniform ceiling without coupling/preparation bounds |
| Polarization; structural null and bounded discrimination | Observe V's branch voltages at $\log2$; then split time constants | $(1/2,-1/2)\ \mathrm V$ versus $(0,0)$; split terminal contrast $1/2-1/\sqrt2\ \mathrm V$ |
| Absorber; resolved structural result, calibration open | Hold VI's force/frequency; measure coupling strain and section area | Reaction zero in both; stress amplitude $1$ versus $1/2\ \mathrm{MPa}$ |

: Comparison types and finite observables for correspondence and identification questions. Omitting preparation or reset readings is an accounting failure, not an alternative trajectory.

For the damped analogy, forces/torques and motions, not homogeneous equation coefficients alone, must be transported through preparation and reset. The contact experiment must vary support and contact independently, first within a declared finite constitutive family; failure of added anvil data to resolve a frequency-dependent support requires a support sensor or a narrower model, not an assertion of full identification. The coefficient experiment must retain temporal correlation and calibration covariance when evaluating the $1/100$ separation. A successful comparison on the declared support does not prove that support globally minimal.

The resonator task remains an acquisition across physical devices, calibrated fixtures and independently changed shunts. The normalized example predicts a discriminant but supplies no substitute traces. Polarization order recovery requires independently prepared branches, a finite time-constant separation domain and actual noise bounds. The absorber's bounded inability to infer stress from terminal reaction is already resolved; calibrated strain, section area and material conversion address the remaining practical extension.

## Signed residuals and bounds from calibrated channels
\label{sec:channel-audit}

The measurement comparisons in Appendix \ref{sec:measurements} use independent work and endpoint uncertainties. The following forms use observed channel amplitudes, retain all cross terms and distinguish bounded observation errors from unknown physical omissions.

### Which residual survives the independent account?
\label{sec:residual-outcomes}

A positive or negative energy residual is reported for the declared boundary and interval before any additional transfer is assigned. For each case retain the initial and final constitutive stores, every separately integrated signed work, event-side states, and the checks on polarity, timing, dimensions and constitutive assumptions. The exact contact deficit \eqref{eq:contact-deficit} and coupling residual \eqref{eq:coupling-residual} are nonzero examples under the stated exact model. An independently demonstrated transfer or store correction changes the account by its own signed contribution; report the remaining residual as well.

For measurement estimates $\widehat E_j,\widehat W_\ell$, suppose calibration and the declared observation model establish $|\widehat E_j-E_j|\leq\epsilon_{E_j}$ and $|\widehat W_\ell-W_\ell|\leq\epsilon_{W_\ell}$. Then
\begin{align}
 \widehat r_E&=\widehat E_1-\widehat E_0-\sum_\ell\widehat W_\ell,\nonumber\\
 |\widehat r_E-r_E|&\leq
 \epsilon_{E_0}+\epsilon_{E_1}+\sum_\ell\epsilon_{W_\ell}
 \equiv\epsilon_r.
 \label{eq:residual-enclosure}
\end{align}
The proof is the triangle inequality; it requires no statistical independence. Correlated error sets can give a tighter enclosure when justified. Include event-time and event-side uncertainty in the corresponding store and work bounds. A covariance matrix alone supplies no deterministic bound. Unquantified omitted physics remains an unquantified model limitation, rather than an adjustable allowance chosen after seeing the residual.

| Exact condition on the estimated residual interval | Outcome for the declared boundary and assumptions |
|:---------------------------------------------------|:-------------------------------------------------|
| $\widehat r_E-\epsilon_r>0$ | Resolved positive residual |
| $\widehat r_E+\epsilon_r<0$ | Resolved negative residual |
| $\widehat r_E-\epsilon_r\leq0\leq\widehat r_E+\epsilon_r$ | Sign unresolved at the stated resolution |

: Signed residual outcomes. Each result retains its interval, preparation, ports and model scope.

If no independently established transfer or store change accounts for a resolved excess, retain it as an open problem with magnitude, sign, conditions and completed checks. A residual interval containing zero gives a bound at that resolution; it is not a missing-destination assignment. Finite source, switching and thermal accounts can fail locally even when a combined interval appears to close. For contiguous intervals with consistent shared endpoint states, the residuals add exactly, so opposite local residuals can cancel. For nested boundaries, cancellation of a declared internal transfer likewise does not certify either subsystem's endpoint reconstruction.

Residual sign patterns are worth investigating, but their interpretation needs an error model. A gain error with a fixed sign can bias every integrated work in a family in the same direction. More generally, a deterministic integration discrepancy need not be symmetric. For an exact algebraic illustration, the equal-subinterval trapezoidal expression for $f(t)=a t^2$, $a>0$, on $[0,T]$ satisfies
\begin{equation}
 \frac{T}{n}\left[\frac{f(0)+f(T)}2+
                   \sum_{j=1}^{n-1}f(jT/n)\right]
       -\int_0^Tf(t)\,\dd t=\frac{aT^3}{6n^2}>0.
 \label{eq:signed-integration-control}
\end{equation}
This identity follows from $\sum_{j=1}^{n-1}j^2=(n-1)n(2n-1)/6$; it is an exact finite-sum control, with no numerical integration performed. A proposed sign test therefore needs a justified null distribution and dependence model. Repeated or shared trajectories are not automatically independent trials. Sign bias alone does not identify a physical transfer, and sign symmetry alone does not resolve a discrepancy. Retain both the sign investigation and each signed residual until its uncertainty or physical account has been established.

### From instrument channels to work and endpoint bounds
\label{sec:instrument-bounds}

Suppose synchronized effort and flow estimates satisfy $|e-\widehat e|\leq\epsilon_e(t)$ and $|f-\widehat f|\leq\epsilon_f(t)$ on a fixed interval. Expand their product before applying the triangle inequality:
\begin{equation}
 |W-\widehat W|\leq
 \int_{t_0}^{t_1}
 \bigl(|\widehat e|\epsilon_f+|\widehat f|\epsilon_e
                  +\epsilon_e\epsilon_f\bigr)\,\dd t,\qquad
 \widehat W=\int_{t_0}^{t_1}\widehat e\,\widehat f\,\dd t.
 \label{eq:channel-work-bound}
\end{equation}
This retains the cross term and requires no independence assumption. Gain, offset, bandwidth and polarity belong in the channel model. A relative timing error bounded by $\delta t$ contributes $M_f\delta t$ to $\epsilon_f$ when $|\dot f|\leq M_f$ on the required smooth extension. Such a bound cannot cross an unresolved discontinuity. Split at events; if regular power is bounded by $M_P$, moving an integration endpoint by at most $\delta t$ adds $M_P\delta t$ to its work bound. Impulsive work and event-side stores require separate bounds.

For an independently calibrated capacitor, $|C-\widehat C|\leq\epsilon_C$, $|v-\widehat v|\leq\epsilon_v$ and $C>0$ imply the exact endpoint bound
\begin{equation}
 \left|\frac12Cv^2-\frac12\widehat C\widehat v^2\right|
 \leq\frac12\epsilon_C\widehat v^2
       +(\widehat C+\epsilon_C)|\widehat v|\epsilon_v
       +\frac12(\widehat C+\epsilon_C)\epsilon_v^2.
 \label{eq:capacitor-error}
\end{equation}
The same form applies to an inductor, translational mass or spring using the corresponding coefficient and state. Apply it independently at both endpoints. For coupled magnetic storage retain the full joint parameter set, including $M$ and its sign. More generally, for $E=x^THx/2$, $\|H-\widehat H\|_2\leq\epsilon_H$ and $\|x-\widehat x\|_2\leq\epsilon_x$, after declaring a dimensionally consistent coordinate scaling,
\begin{equation}
 |E-\widehat E|\leq
 \frac12\epsilon_H\|\widehat x\|_2^2+
 (\|\widehat H\|_2+\epsilon_H)\|\widehat x\|_2\epsilon_x+
 \frac12(\|\widehat H\|_2+\epsilon_H)\epsilon_x^2.
 \label{eq:quadratic-store-error}
\end{equation}
Optimizing over a calibrated correlated set can tighten this enclosure; omitting cross-storage terms cannot.

For the hidden-loop control, \eqref{eq:capacitor-error} bounds each capacitor endpoint by $1432301/200000000000\ \mathrm J$. Equation \eqref{eq:channel-work-bound} bounds each one-second resistor work by $2201/1000000000\ \mathrm J$. Four endpoints and two works give \eqref{eq:hidden-loop-resolution} exactly. The example demonstrates a falsifiable resolution requirement, not observed accuracy.

Recorded-waveform integration adds its own independently bounded acquisition and quadrature error to each work. Exact analytic integration does not eliminate physical calibration or omitted-model uncertainty. A residual bound is complete only for its declared boundary, all named ports, both endpoint states, event sides and observation model. Report an unknown contribution as unknown rather than choosing its size to contain the residual.

## Exact checks and scope of the calculations

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

: Verification separates exact model identities, unevaluated work functionals and named physical omissions.

Every figure is either a schematic or the exact closed form given in the text. All tabulated works and endpoints follow by algebra and integration of those forms. No decimal residual, finite-precision failure or coordinate magnitude has been used as physical evidence. The bounded structural and prescribed-cell conclusions remain bounded; resolving an inherited local question does not replace its practical measurement extension.

\Needspace{16\baselineskip}

## Relation to earlier work

[*Third- and Higher-Order ODEs*][main] supplies the broader distinction between coefficient constructions, state elimination and physical realization. The present results develop its open questions by attaching explicit preparations, event paths, recipient channels and calibrated observations. The complete finite port correspondence in \eqref{eq:analogy}, the distinct contact release laws and the two-channel work partition each identify information absent from a scalar trajectory.

[Wettstein, Grauberger and Matthiesen (2021)][wettstein] relate hammer-mechanism behavior to a changing sequence of contacts and embodiment relations. That modeling context motivates retaining contact and support coordinates through engagement. The exact release destination and repeated constitutive law here require their own measurements. [Bible (2002)][bible] describes the conventional crystal motional branch and shunt capacitance used in \eqref{eq:resonator}; that component description does not establish a transferable coefficient law across arbitrary devices. [Keysight Technologies (n.d.)][keysight] explains impedance methods and fixture compensation. Those measurement distinctions support the calibrated complex-port comparison, while uncertainty and internal-state identification remain specific to the apparatus and model class.

[Kalman (1963)][kalman] supplies the general realization and observability distinction; the present contact inverse and prepared polarization controls specify what additional channels identify in particular models. [Willems (1972)][willems] provides the storage/supply framework for interconnected systems; the separately integrated event paths here identify which physical ports that framework needs. [Schwager and Pöschel (2007)][schwager] distinguish repulsive-contact termination from a continued linear-dashpot collision. The retained material state and receiver comparisons in Section \ref{sec:contact} address the additional destination question. These established principles provide context for the explicit constructions, rather than an assignment of any unmeasured work.

# References {-}

\begingroup\small

1. Nilre, H., and Herlin, B. C. (2026). [*Third- and Higher-Order ODEs: Coefficient synthesis, identification, and physical realization*][main]. Companion manuscript on GitHub.
2. Wettstein, A., Grauberger, P., and Matthiesen, S. (2021). [Modeling dynamic mechanical system behavior using sequence modeling of embodiment function relations: case study on a hammer mechanism][wettstein]. *SN Applied Sciences* **3**, article 128. DOI: 10.1007/s42452-021-04149-8.
3. Bible, S. (2002). [Crystal Oscillator Basics and Crystal Selection for rfPIC and PICmicro Devices][bible]. Microchip Technology, Application Note AN826, DS00826A, pp. 1--14.
4. Keysight Technologies (n.d.). [*Impedance Measurement Handbook: A Guide to Measurement Technology and Techniques*][keysight]. Application note 5950-3000.
5. Kalman, R. E. (1963). [Mathematical Description of Linear Dynamical Systems][kalman]. *Journal of the Society for Industrial and Applied Mathematics, Series A: Control* **1**(2), 152--192. DOI: 10.1137/0301010.
6. Willems, J. C. (1972). [Dissipative Dynamical Systems Part I: General Theory][willems]. *Archive for Rational Mechanics and Analysis* **45**, 321--351. DOI: 10.1007/BF00276493.
7. Schwager, T., and Pöschel, T. (2007). [Coefficient of restitution and linear--dashpot model revisited][schwager]. *Granular Matter* **9**, 465--469. DOI: 10.1007/s10035-007-0065-z.
8. Basu, S., Pollack, R., and Roy, M.-F. (2006). [*Algorithms in Real Algebraic Geometry*][basu]. 2nd edition, Algorithms and Computation in Mathematics **10**. Springer, Berlin, Heidelberg. DOI: 10.1007/3-540-33099-2.

\endgroup

[main]: https://github.com/hobnilre/physics-ode-3rd-deg
[wettstein]: https://doi.org/10.1007/s42452-021-04149-8
[bible]: https://ww1.microchip.com/downloads/en/appnotes/00826a.pdf
[keysight]: https://www.keysight.com/us/en/assets/7018-06840/application-notes/5950-3000.pdf
[kalman]: https://doi.org/10.1137/0301010
[willems]: https://doi.org/10.1007/BF00276493
[schwager]: https://doi.org/10.1007/s10035-007-0065-z

[basu]: https://doi.org/10.1007/3-540-33099-2
