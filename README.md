# Supplementary material: Two-period Contest with Asymmetric Budget Constraints

The long polynomials referred to in the appendices of the paper, together with the
numerical constants and box counts of the computer-assisted steps.

## Layout

| Folder | Contents |
|---|---|
| `supplement/supp_polynomials.pdf` | the typeset supplement: one section per appendix, one subsection per polynomial, with the numerical constants and box counts of each appendix in the section header |
| `supplement/supp_polynomials.tex` | its LaTeX source (`\input` it from a wrapper document with `amsmath`) |
| `supplement/supp_polynomials.txt` | the same polynomials in machine-readable form, one per line, Python/sympy syntax |
| `polynomials/<tag>/<name>.txt` | the same polynomials split into one file each, named after the variable in the paper, for loading a single polynomial |
| `polynomials/INDEX.txt` | list of every polynomial with its variables |

The two folders hold the same 80 polynomials. `supplement/` is for reading (PDF) and for
citing, `polynomials/` is for computing: each file can be read with `sympy.sympify` or any
computer algebra system.

## Which folder covers which appendix

| `polynomials/C4/` | Appendix C.4, Proposition prop:bi_xi1_wi | `P_Delta`, `U_Delta`, `V_Delta`, `W_Delta`, `P_K`, `W_U`, `W_L` |
| `polynomials/C5/` | Appendix C.5, Proposition prop:xj1_single_peaked_bi | `Omega`, `q_rho`, `q_mi`, `q_mj`, `omega_mi`, `omega_mj`, `omega_rho`, `Omega_mi`, `Omega_mj`, `Gamma`, `R`, `Res_mi_Omega_R` |
| `polynomials/C7/` | Appendix C.7, Proposition prop:bi_we_wj | `P_M`, `U_M`, `V_M`, `W_M`, `Xi_mi`, `Xi_mj`, `Xi_rho`, `DetTotal`, `NumTotal`, `Xi_n`, `DetTotal_n`, `NumTotal_n`, `Res_rho_q_Xi_mj1` |
| `polynomials/C9/` | Appendix C.9, Proposition prop:bi_utility | `Pi_poly`, `z5_q`, `z5_Ups`, `z15_Pi_poly` |
| `polynomials/D1/` | Appendix D, Lemma lem:transfer_os_crossing | `K`, `Res_u_K_8h`, `Sturm_0`, `Sturm_1`, `Sturm_2`, `Sturm_3`, `Sturm_4`, `Sturm_5`, `Sturm_6`, `Sturm_7`, `Sturm_8`, `Sturm_9`, `Sturm_10`, `Sturm_11`, `Sturm_12`, `Sturm_13`, `Sturm_14`, `Sturm_15` |
| `polynomials/D2/` | Appendix D, Lemma lem:transfer_single_crossing and Proposition prop:transfer_TI | `H_poly`, `D`, `T_ess`, `P_1`, `Q_0`, `H_0`, `Q_1`, `H_1`, `Q_2`, `H_2` |
| `polynomials/D3/` | Appendix D, Lemma lem:transfer_richer | `Hj_poly`, `Tj_ess`, `Pj`, `qhat`, `Hhat`, `That`, `q_tilde`, `H_tilde`, `Q_2`, `H_2`, `Q_3`, `H_3`, `Q_4`, `H_4`, `Q_5`, `H_5` |

Notation: `m_i = 1/(2 sqrt(y_i))`, `m_j = 1/(2 sqrt(y_j))`, `rho = x_i1/x_j1`, `c = m_j - 1`, `d = m_i - m_j`.
The rescaled variables of the interval searches (`a = 1/m_i`, `b = 1/m_j`, and the chart coordinates
`z, tau, eta`, `t, sigma`, `u, lambda, mu`, `beta, nu, theta`) are defined at the start of the
corresponding section of the supplement.

Each polynomial file gives the polynomial in the form `name(variables) = ...`, expanded, with
integer coefficients, readable by `sympy.sympify` or by any computer algebra system.
