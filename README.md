---
author:
- Mohammad Abazari
bibliography:
- bibs.bib
title: "Final Exam: Impact and Penetration"
---

# Problem 1 {#problem-1 .unnumbered}

A protective wall is struck by a rigid ogive projectile traveling 1,000
m/s. Provide a safe and economic wall design. Material and projectile
properties provided in [1](#tab02){reference-type="ref"
reference="tab02"}.

::: {#tab02}
   Projectile properties.                                           
  ------------------------ ---------- ----------- -------- -------- ------------------
       Material Type        mass, kg   Length, m   $s$, m   $d$, m   $\mu_\mathrm{m}$
           Steel              0.2        0.05       0.1      0.04          0.2

  : Material and projectile properties.
:::

[\[tab02\]]{#tab02 label="tab02"}

# Solution {#solution .unnumbered}

The objective here is to prevent perforation in an economic way. There
are multiple solutions, due to the variety of methods available.

## Concrete panel {#concrete-panel .unnumbered}

[@forrestal1994empirical; @forrestal1996penetration; @frew2006effect; @frew1998penetration]
proposed the following formula for projectile depth of penetration[^1],
$$\label{eq01}
  \begin{aligned}
  h_{\text {pen }}=&\frac{\left(L+0.5 k^{\prime} d\right)}{2 N}\left(\frac{\rho_p}{\rho_0}\right) \ln \left[1+\frac{N \rho_0 V_1^2}{S f_{\mathrm{c}}}\right]+2 d \\
  =&\frac{2 M}{\pi d^2 \rho_0 N} \ln \left[1+\frac{N \rho_0 V_1^2}{S f_{\mathrm{c}}}\right]+2 d
  \end{aligned}$$ $$\label{eq02}
k^{\prime}=\left(4 \psi^2-\frac{4 \psi}{3}+\frac{1}{3}\right)(4 \psi-1)^{0.5}-4 \psi^2(2 \psi-1) \sin ^{-1}\left[\frac{(4 \psi-1)^{0.5}}{2 \psi}\right]$$
$$\label{eq03}
  N=\frac{8 \psi-1}{24 \psi^2}; \quad V_1^2=\frac{V_0^2-\left({2 d}/({L+0.5 k^{\prime} d})\right)\left({S f_c}/{\rho_p}\right)}{1+N\left({2 d}/({L+0.0 k^{\prime} d})\right)\left({\rho_0}/{\rho_p}\right)} ; \quad S=82.6 \times\left(f_{\mathrm{c}} \times 10^{-6}\right)^{-0.544}$$

[@forrestal2003penetration] modified the above. The proposed formula are
only applicable for ogive-nosed projectiles while neglecting friction
between projectile and target medium. $$\nonumber
  \begin{aligned}
  \psi & =\frac{0.1}{0.04} \rightarrow N=\frac{8(2.5)-1}{24(2.5)^2} \rightarrow=0.1267 \\
  S & =82.6 \times\left(90 \times 10^6 \times 10^{-6}\right)^{-0.544} \rightarrow=7.143 \\
  k^{\prime} & =\left(4(2.5)^2-\frac{4(2.5)}{3}+\frac{1}{3}\right)(4(2.5)-1)^{0.5}-4(2.5)^2(2(2.5)-1) \sin ^{-1}\left[\frac{(4(2.5)-1)^{0.5}}{2(2.5)}\right] \\
  & =1.650 \\
  V_1^2 & =\left[{(1000)^2-\left(\frac{2(0.04)}{0.05+0.5(1.650)(0.04)}\right)\left(\frac{(7.430)\left(90 \times 10^6\right)}{7850}\right)}\right]\\
 &\times \left[{1+(0.1267)\left(\frac{20.04)}{0.05+0.5(1.650)(0.04)}\right)\left(\frac{2500}{7850}\right)}\right]^{-1} \\
  & =886000 \rightarrow V_1=941.6 \mathrm{~m} / \mathrm{s} \\
  h_{\text {pen }} & =\frac{2(0.2)}{\pi(0.04)^2(2500)(0.1267)} \ln \left[1+\frac{(0.1267)(2500)(941.6)^2}{(7.143)\left(90 \times 10^6\right)}\right]+2(0.04) \\
  & =0.1711 \rightarrow \text { or } 17.11 \mathrm{~cm}
  \end{aligned}$$ [@chen2002deep; @li2003dimensionless] extended the
equations presented by
[@forrestal1993penetration; @forrestal1996penetration] to a
dimensionless form applicable to arbitrary-nosed projectiles. According
to [@chen2002deep; @li2003dimensionless] maximum penetration depth in a
thick plate is $$\label{eq04}
  \frac{h_{\mathrm{pen}}}{d}=\frac{2}{\pi} N \ln \left(1+\frac{I_0}{N}\right)$$
$$\label{eq05}
    I_0=\frac{M V_0^2}{N_1 S f_{\mathrm{c}} d^3} ; \quad N=\frac{M}{N_2 \rho_0 d^3} ; \quad S=72.0 \times\left(f_{\mathrm{c}} \times 10^{-6}\right)^{-0.5}$$

where $I_0$ and $N$ are defined as the impact and geometry functions,
$N_1$ and $N_2$ account for projectile nose geometry as well as
friction. For an arbitrary-nosed projectile, $N_1$ and $N_2$ are
obtained through integrating the projectile nose profile function along
the nose length. Explicit expressions of $N_1$ and $N_2$ for ogive,
conical, blunt, truncated ogive, hemispherical, and flat projectile
noses are given [@chen2002deep]. For ogive nosed projectiles we have
$$\nonumber
  \begin{aligned}
  & N_1=1+4 \mu_{\mathrm{m}} \psi^2\left[\left(\frac{\pi}{2}-\phi_0\right)-\frac{\sin 2 \phi_0}{2}\right] \\
  & N_2=N^*+\mu_{\mathrm{m}} \psi^2\left[\left(\frac{\pi}{2}-\phi_0\right)-\frac{1}{3}\left(2 \sin 2 \phi_0+\frac{\sin 4 \phi_0}{4}\right)\right] \\
  & N^*=\frac{1}{3 \psi}-\frac{1}{24 \psi^2}, \quad 0<N^* \leq \frac{1}{2} \\
  & \phi_0=\sin ^{-1}\left(1-\frac{1}{2 \psi}\right), \quad \text { where } \psi \geq \frac{1}{2}
  \end{aligned}$$

Inclusion of sliding friction coefficient makes this formula quite
advantageous. $$\nonumber
  \begin{aligned}
  \phi_0 & =\sin ^{-1}\left(1-\frac{1}{2 \psi}\right) \rightarrow=0.9273 \text { or } 53.13^{\circ} \\
  N^* & =\frac{1}{3(2.5)}-\frac{1}{24(2.5)^2} \rightarrow=0.1267 \\
  N_1 & =1+4(0.2)(2.5)^2\left[\left(\frac{\pi}{2}-(0.9273)\right)-\frac{\sin 2(0.9273)}{2}\right] \rightarrow=1.817 \\
  N_2 & =(0.1267)+0.2(2.5)^2\left[\left(\frac{\pi}{2}-(0.9273)\right)-\frac{1}{3}\left(2 \sin 2(0.9273)+\frac{\sin 4(0.9273)}{4}\right)\right] \\
  & =0.1871\\
    S & =72.0 \times\left(\left(90 \times 10^6\right) \times 10^{-6}\right)^{-0.5} \rightarrow=7.589 \\
    I_0 & =\frac{(0.2)(1000)^2}{(1.8175)(7.589)\left(90 \times 10^6\right)(0.04)^3} \rightarrow=2.5172 \\
    N & =\frac{0.2}{(0.1871)(2500)(0.04)^3} \rightarrow=6.681 \\
    h_{\text {pen }} & =(0.04)\left(\frac{2}{\pi}(6.681) \ln \left(1+\frac{(2.5172)}{(6.681)}\right)\right) \\
    & =0.05440 \text { or } 5.440 \mathrm{~cm}
    \end{aligned}$$ while with no friction $$\nonumber
  \begin{aligned}
  N_1 & =1 \\
  N_2 & =N^* \rightarrow=0.1267 \\
  I_0 & =\frac{(0.2)(1000)^2}{(1)(7.590)\left(90 \times 10^6\right)(0.04)^3} \rightarrow=4.575 \\
  N & =\frac{0.2}{(0.1267)(2500)(0.04)^3} \rightarrow=9.866 \\
  h_{\text {pen }} & =(0.04)\left(\frac{2}{\pi}(9.866) \ln \left(1+\frac{(4.575)}{(9.866)}\right)\right) \\
  & =0.09571 \text { or } 9.571 \mathrm{~cm}
  \end{aligned}$$ [@chen2002deep] states that the formula is valid if
the penetration depth is larger than the projectile diameter and the
projectile nose length while projectile remains rigid without noticeable
deformation and damage.

## Steel panel {#steel-panel .unnumbered}

The formula proposed by [@chen2002deep] has a good agreement with tests
on metal, concrete and soil samples with variable nose shapes and
velocities. From [@li2003dimensionless], $$\nonumber
\begin{aligned}
  \frac{X}{d}=&\frac{2}{\pi} N \ln \left(1+\frac{I}{N}\right)\\
  I=&\frac{\lambda \Phi_{\mathrm{J}}}{A N_1} ; \quad N=\frac{\lambda}{B N_2} ; \quad \lambda=\frac{M}{\rho_0 d^3} ; \quad \Phi_{\mathrm{J}}=\frac{\rho_0 V_{\mathrm{i}}^2}{\sigma_{\mathrm{y}}}
\end{aligned}$$ Based on [@forrestal1988dynamic], [@li2003dimensionless]
suggests the following for an elastic, perfectly plastic material, where
$\gamma$[^2] is the Poisson's ratio: $$\nonumber
A=\frac{2}{3}\left\{1+\ln \left[\frac{{E}}{3(1-{\gamma}) {\sigma_y}}\right]\right\}$$
And for incompressible materials $B=1.5$. Note that parameters
$\phi_0, N^*, N_1, N_2$ just depend on the penetrator and not the target
material. So considering sliding friction, $$\nonumber
  \phi_0  =0.9273 \text { or } 53.130^{\circ} ; \quad N^*=0.1267 ; \quad N_1=1.8175 ; \quad N_2=0.1871;$$
and $$\nonumber
  \begin{aligned}
  A  =&\frac{2}{3}\left\{1+\ln \left[\frac{{200 \times 10^9}}{3(1-{0.30}) {400 \times 10^6}}\right]\right\} \rightarrow=4.315 \\
  \lambda  =&\frac{0.2}{7850(0.04)^3} \rightarrow=0.3981 \\
  \Phi_{\mathrm{J}}  =&\frac{(7850)(1000)^2}{{400 \times 10^6}} \rightarrow=19.62 \\
  I  =&\frac{(0.3981)(19.62)}{(4.315)(1.817)} \rightarrow=0.9962 \\
  N =& \frac{(0.3981)}{(1.5)(0.1871)} \rightarrow=1.418 \\
  X  =&(0.04)\left(\frac{2}{\pi}(1.418) \ln \left(1+\frac{(0.9962)}{(1.418)}\right)\right) \rightarrow=0.01922 \text { or } 1.922 \mathrm{~cm}
  \end{aligned}$$ While without friction
$$\phi_0=0.9273 \text { or } 53.13^{\circ} ; \quad N^*=N_2 \rightarrow=0.1267 ; \quad N_1=1 ; \quad A=4.315 ;$$
$$\lambda=0.3981 ; \quad \Phi_{\mathrm{J}}=19.62$$ then $$\nonumber
\begin{aligned}
I=&\frac{(0.3981)(19.625)}{(4.315)(1)}\rightarrow=1.811\\
N=&\frac{(0.3981)}{(1.5)(0.1267)}\rightarrow=2.095\\
X=&(0.04)\left(\frac{2}{\pi}(2.095)\ln{\left(1+\frac{1.811}{2.095}\right)}\right)\rightarrow=0.03323 ~ \mathrm{or}~ 3.323\,\mathrm{cm}
\end{aligned}$$

## Final design {#final-design .unnumbered}

Results from earlier discussions are presented in
[\[tab03\]](#tab03){reference-type="ref" reference="tab03"}.

Suprisingly UHPC proves more expensive. Design thickness suggestions
were made accounting for 25% increase due to formula deviations and
including a 1.2 safety factor which rises the margin to about 50% in
order to prevent spalling and scabbing as suggested by
[@krauthammer2008modern].

# Problem 2 {#problem-2 .unnumbered}

A 200 kg cased cylindrical charge is set off 45 m away from the concrete
face of a two layered blast wall. Design this wall for the largest
primary fragments, and also calculate wall ballistic thickness. The PETN
charge is encased in a mild steel casing 40 cm long with $d_i/t_c=10$.

## Solution {#solution-1 .unnumbered}

The main assumption is that the fragment is stopped by penetrating the
steel layer thus peforating the concrete layer.

::: {#tab04}
            Item             Value
  ------------------------ ----------
   Charge weight, kg(lbs)   200(441)
      Distance, m(ft)       45(150)
   Casing length, cm(in)     40(16)

  : Given.
:::

The specific weight and Gurney energy constant for PETN are respectively
0.0635 lb/in$^3$ and 9,600 ft/sec based on [@ufc3340022014] while
specific weight of mild steel casing is assumed to be about 490
lb/ft$^3$.

Total weight of cased charge equals the sum total of charge and casing
weights. Thus considering a cylindrical shape $$\nonumber\begin{aligned}
W_\mathrm{Total}=&W_{ACT}+W_c\rightarrow \rho_\mathrm{PETN}V_{ACT}+\rho_cV_c\\
=&l\left(\rho_\mathrm{PETN}\left(\frac{\pi}{4}\right)d_i^2+\rho_c\left(\frac{\pi}{4}\right)\left(d_i+t_c^2-d_i^2\right)\right)\\
=&t_c^2l\left(\frac{\pi}{4}\right)\left(100\rho_\mathrm{PETN}+44\rho_c\right)\\
\rightarrow t_c=&0.115(1.38)\, \mathrm{ft(in)}\rightarrow d_i = 1.15(13.8)\, \mathrm{ft(in)}\\
W_{ACT}=&16(0.0635)\left(\frac{\pi}{4}\right)\left(13.8\right)^2, W_c=290\,\mathrm{lbs}\\
W=&1.2W_{ACT}\rightarrow=181\,\mathrm{lbs}
\end{aligned}$$ Initial velocity of primary fragments resulting from a
higher-order detonation of a cylindrical casing with evenly distributed
explosives is expressed as[@ufc3340022014] $$\nonumber
v_o= \sqrt{2E^\prime\left(\frac{W/W_c}{1+0.5W/W_c}\right)}=9600\sqrt{\frac{181/290}{1+0.5\left(181/290\right)}}\rightarrow=6621\,\mathrm{ft/s}$$
largest fragment weight $w_f$ is calculated by setting $N_f$ equal to 1,
$$\nonumber
\begin{aligned}
N_f=&\frac{8W_ce^{-{w_f}^{1/2}/M_A}}{M^2_A}\rightarrow=1\\
w_f=&\left(M_A\ln\left[\frac{8W_c}{N_fM_A^2}\right]\right)^2, M_A=Bt_c^{5/6}d^{1/3}_i\left(1+\frac{t_c}{d_i}\right)\\
\xrightarrow[\text{\cite{ufc3340022014}}]{\text{From Table 2-7}} B=&0.248\\
M_A=&0.248\left(1.38\right)^{5/6}\left(13.8\right)^{1/3}(1+0.1)\rightarrow=0.8558\\
w_f=&\left(0.8558\ln{\left[\frac{8(290)}{(1)(0.8558)^2}\right]}\right)^2\rightarrow=47.5\,\mathrm{oz}
\end{aligned}$$ [@ufc3340022014] expresses striking velocity as
$$\nonumber
V_s=V_oe^{-12k_VR_f}, k_V=0.5(A/w_f)\rho_aC_D;$$ Assuming
$A/w_f=0.78/w_f^{1/3}$ for a random mild steel fragment (in$^2$/oz),
$\rho_a=0.00071$ oz/in$^3$ and $C_D=1.2$ for primary fragments, thus for
a cylindrical casing $$\nonumber
\begin{aligned}
d=&\sqrt{\left(\frac{4}{\pi}\right)0.78w_f^{2/3}}\rightarrow=3.61\, \mathrm{in}\rightarrow A=10.24\,\mathrm{in}^2\\
k_V=&\frac{1}{2}\left(\frac{10.24}{47.5}\right)(0.00071)(1.2)\rightarrow=9.184\times10^{-5}\\
V_s=&(6621)e^{-12(9.184\times10^{-5})(150)}\rightarrow=5612\,\mathrm{ft/s}\,\text{(Case I)}
\end{aligned}$$ Striking velocity is determinable assuming values like
shape factor $N$ and fragment nose tangent ogive caliber radius $n$ for
an alternate fragment form. Assuming $N=1$ and $n=1.5$, according to
Figure 2-244b in [@ufc3340022014] $$\begin{aligned}
\nonumber
V_f=&1.2d^3, \rho_f = 4.6~\mathrm{oz/in}^3\rightarrow w_f= 5.52d^3\,\mathrm{oz} \rightarrow d=2.05\,\mathrm{in}\rightarrow A=3.30\, \mathrm{in}^2;\\\nonumber
k_V=&\frac{1}{2}\left(\frac{3.30}{47.5}\right)(0.00071)(1.2)\rightarrow=2.960\times10^{-5}\\\nonumber
V_s=&(6621)e^{-12(2.960\times10^{-5})(150)}\rightarrow=6277\,\mathrm{ft/s}\,\text{(Case II)}\end{aligned}$$

Perforating the concrete layer the fragment is embeded penetrating in
the steel layer $$\nonumber\begin{aligned}
X_f=&\left\{\begin{array}{lr}
4.0\times10^{-3}\sqrt{K\,N\,D}d^{1.1}v_s^{0.9},& X_f\leq2d\\
4.0\times10^{-6}K\,N\,Dd^{1.2}v_s^{1.8}+d,& X_f>2d\\
\end{array}\right.\\
K=&\sqrt{12.91}{\sqrt{f_c'}}\rightarrow \frac{12.91}{\sqrt{13053}}=0.1130\\
\end{aligned}$$ Penetration depth is larger than $2d$ for both cases.

### Case I {#case-i .unnumbered}

$$\begin{aligned}
\nonumber
 N=&1, D=47.5/(2.05)^3\rightarrow =5.51\\
X_f=&4.0\times10^{-6}(0.113)(1)(5.51)(2.05)^{1.2}(6277)^{1.8}+2.05\rightarrow=42.45\,\mathrm{in}\nonumber\\
\xrightarrow[\text{for }f'_c]{\text{Correcting}} X'_f=&X_f\sqrt{\frac{4,000}{f_c'}}\rightarrow(42.45)\sqrt{\frac{4000}{13053}}=23.5\,\mathrm{in}\nonumber\end{aligned}$$
An armor piercing fragment woul produce this level of penetration and
having a mild steel casing sanctions another correction based off of
Table 4-16 from [@ufc3340022014]. $$\begin{aligned}
\nonumber
X'_f=&kX_f\rightarrow X_\mathrm{pen}\,\text{or}\, X_f=0.7\times(23.5)\rightarrow=16.5\,\mathrm{in}\\\nonumber
T_{pf}=&1.13X_fd^{1/10}+1.311d\rightarrow=1.13(16.5)(2.05)^{1/10}+1.311(2.05)=22.35\,\mathrm{in}\nonumber\end{aligned}$$
Considering $X_f>2d$ [@ufc3340022014] expresses fragment residual
velocity after perforating a concrete wall $T_c$ thick as
$$\label{eqvvr}
V_r/V_s=\left[1-\frac{T_c}{T_{pf}}\right]^{0.555}, X_f>2d$$ In addition
[@ufc3340022014] provides the follwoing for mild steel plate penetration
that in our case the striking velocity would equal the concrete wall
fragment residual velocity. Note that resulting thickness values are
ballistic limits and design should include certain factors of safety.

$$\label{eqxs}
x=0.21w_f^{0.33}V_s^{1.22}$$ Given that $T_C/T_s=5$ and
$v_{r\,\text{(Concrete)}}=v_{s\text{(Steel)}}$ and that the striking
velocity in the above formula is expressed in kft/sec after substituting
[\[eqvvr\]](#eqvvr){reference-type="ref" reference="eqvvr"} into
[\[eqxs\]](#eqxs){reference-type="ref" reference="eqxs"} with known
parameters the resulting equation is solved for $T_s$, $$\begin{aligned}
\nonumber
V_r=&6277\left[1-\frac{5T_s}{22.35}\right]^{0.555}\rightarrow x=0.21w_f^{0.33}V_s^{1.22}\\\nonumber
 x=&0.21(47.5)^{0.33}\left(6.277\left[1-\frac{5T_s}{22.35}\right]^{0.555}\right)^{1.22}\rightarrow=3.13\,\mathrm{in}\\\nonumber
 \text{ and thus }\rightarrow T_c=&15.65\,\mathrm{in}\end{aligned}$$ The
wall would end up $T_T=T_c+T_s=18.8~\mathrm{in}$ thick.

### Case II {#case-ii .unnumbered}

Following the same previous steps, $$\begin{aligned}
\nonumber
N=&1, D=47.5/(3.61)^3\rightarrow=1.01\\\nonumber
X_f=&4.0\times 10^{-6}(0.113)(1)(1.01)(3.61)^{1.2}(5612)^{1.8}+3.61\rightarrow=15.55\,\mathrm{in}\\\nonumber
X'_f=&X_f\sqrt{\frac{4000}{f'_c}}\rightarrow 15.55\sqrt{\frac{4000}{13053}}=8.61\,\mathrm{in}\\\nonumber
X_\mathrm{Pen}\text{ or } X_f=&0.7(8.61)=6.03\,\mathrm{in}\\\nonumber
T_{pf}=&1.13(6.03)(3.61)^{0.1}+1.311(3.61)\rightarrow=12.48\,\mathrm{in}\\\nonumber
v_r=&5612\left[1-\left(\frac{5T_s}{12.48}\right)\right]^{0.555}\, \text{ for } X_f<2d\\\nonumber
T_s=&0.21(47.5)^{0.33}\left[5.612\left[1-\frac{5T_s}{12.48}\right]^{0.555}\right]^{1.22}\rightarrow=2.02\,\mathrm{in}\rightarrow T_c=10.1\,\mathrm{in}\end{aligned}$$
And in this case the wall will end up at least $T_T=12.12\,\mathrm{in}$
thick.

[^1]: DOP.

[^2]: About 0.30 for most steel grades.
