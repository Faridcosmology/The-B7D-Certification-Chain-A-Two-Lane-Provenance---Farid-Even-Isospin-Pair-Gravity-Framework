# The B7D Certification Chain: A Two-Lane Provenance Architecture, a Source-Derived Binary Contract, and the Frozen Phase-II Control Protocol for the Farid Even-Isospin Pair Gravity Framework
\documentclass[11pt,a4paper]{article}
\usepackage[utf8]{inputenc}
\usepackage{amsmath}
\usepackage{amsfonts}
\usepackage{amssymb}
\usepackage{booktabs}
\usepackage{geometry}
\usepackage{hyperref}

\geometry{margin=1in}

\title{\textbf{The B7D Certification Chain: A Two-Lane Provenance Architecture, a Source-Derived Binary Contract, and the Frozen Phase-II Control Protocol for the Farid Even-Isospin Pair Gravity Framework}}
\author{\textbf{Prof. Dr. Md. Faridul Islam Chowdhury}\\
MBBS, MS (Neurosurgery) \\
\small Neurosurgeon | Neuroscientist | Theoretical Cosmologist\\
\small Founder \& Director, Tanfarid Vision Research Institute (TVRI), Bogura, Bangladesh\\
\small Email: \href{mailto:dr_faridul@yahoo.com}{dr_faridul@yahoo.com}}
\date{2026}

\begin{document}

\maketitle

\begin{abstract}
This article presents the complete certification chain of the B7D programme of the Farid Even-Isospin Pair Gravity Framework, spanning the audits D18 through D28. The chain carries the programme from a documented absence of its single immutable input to a fully sealed two-lane production architecture. Ten linked audits are reported, each with hash-sealed artifacts, across two physically distinct lanes. The legacy lane ($e_{\max}=4$, $\hbar\omega = 20$~MeV, SRG $2.0~\text{fm}^{-1}$, NuclearToolkit v0.3.4 / IMSRG-Net-v0, Julia 1.8.5) is the validation class; its Hartree-Fock reconstruction of ${}^{16}\text{O}$ and ${}^{40}\text{Ca}$ has been executed under the retrieved legacy interaction (SHA-256 \texttt{267c85b5...}), yielding $E_{\text{HF}}({}^{16}\text{O}) = -132.95058$~MeV and $E_{\text{HF}}({}^{40}\text{Ca}) = -518.07110$~MeV with exactly closing one-body/two-body decompositions. The new B7D-1 production lane ($e_{\max}=8$, $\text{Nnmax}=14$, $\hbar\omega=16$~MeV, effective two-nucleon-three-nucleon contribution, $k_F = 1.35~\text{fm}^{-1}$, no SRG, NuclearToolkit v0.5.2 @\texttt{dfc01916...}, Julia 1.10.10) has generated its first production interaction (SHA-256 \texttt{050e9165...}), a 77,593,968-byte file containing 3,526,624 two-body records with zero semantic violations and a nonzero 2n3n column. The exact \texttt{.snt.bin} binary contract is derived from the frozen source bodies, not from documentation types or inference, and is verified byte-identical across the two frozen revisions (the D25b portability seal). The D28 Phase-II control freeze is pre-registered: the IMSRG control parameters are fixed at their source-verified values; the reference strategy is pre-registered and non-mixed; the \texttt{magnusamethod} vs \texttt{magnusmethod} spelling is resolved from the pinned source tree by the preflight, not assumed. Three corrections are recorded as first-class events: the D18 premature-ingestion correction, the D21b revision-tree-identity recovery, and the D25c Julia-baseline compat-bound correction. The legacy $R_p^2$ blind replay remains NOT RUN. The physical $F_0/F_2$ IMSRG(2) evolution remains NOT RUN. The $A=22$ renormalized monopole and quadrupole matrix elements remain NOT COMPUTED. The gravity fit remains STRICTLY LOCKED.
\end{abstract}

\textbf{Keywords:} certification chain, anti-circular firewall, two-lane architecture, .snt.bin binary contract, Hartree-Fock blind replay, B7D-1 production lane, phase-II control

\newpage

\section{Introduction: A Programme That Refuses to Guess}
The B7D programme is the nuclear-structure certification stage of the Farid Even-Isospin Pair Gravity Framework. Its purpose is to produce --- eventually --- the $A=22$ renormalized pairing monopole and quadrupole matrix elements $M_0$ and $M_2$ from an explicitly certified interaction, through an explicitly certified evolution, under an explicitly certified binary contract, so that no gravitational inference ever rests on an unproven input.

The programme is therefore not primarily a computation programme. It is a \textbf{proof programme} whose computations are its lemmas.

The governing instrument is the \textbf{anti-circular firewall}: a set of procedural rules that forbid claims whose premises are unmet. The firewall has one operational consequence that dominates everything reported here:
\begin{quote}
\textbf{\textit{A missing input is declared missing, the gate is re-locked, and the programme waits.}}
\end{quote}

This article is the record of what that discipline costs, and of what it buys. What it costs is visible in the chain itself: ten audits, three corrections recorded as first-class events, and two execution days separated by a slow-network failure. What it buys is visible in the results: every artifact in this article carries a SHA-256 identity; every validation is reproducible from the frozen source; and the two computations that were finally executed did not merely run --- they ran against contracts that had already been tested against reality.

\section{The Two-Lane Architecture}
The programme operates in two physically distinct lanes that may never be mixed.

\subsection{The Legacy Lane (Validation)}
The purpose of the legacy lane is \textbf{blind replay}: to reproduce, within the programme's own walls, the class of observables against which the comparison literature is defined.

\begin{table}[h!]
\centering
\caption{Legacy Lane Validation Parameters}
\begin{tabular}{ll}
\toprule
\textbf{Parameter} & \textbf{Value} \\
\midrule
$e_{\max}$ & 4 \\
$\hbar\omega$ & 20~MeV \\
SRG resolution scale & $2.0~\text{fm}^{-1}$ \\
Target interaction & \texttt{tbme\_em500n3lo\_srg2.0hw20emax4.snt.bin} \\
Reference nuclei & ${}^{16}\text{O}$, ${}^{40}\text{Ca} $ \\
NuclearToolkit & v0.3.4 / branch \texttt{IMSRG-Net-v0} (commit \texttt{11654a52...}, tree-identical to tag v0.3.4) \\
Julia & 1.8.5 \\
\bottomedrule
\end{tabular}
\end{table}

\subsection{The New B7D-1 Lane (A = 22 Production)}
Its reference strategy is pre-registered and non-mixed: primary $\text{core} = \text{"O16"}$, $\text{ref} = \text{"core"}$, $\text{vspace} = \text{"sd-shell"}$; a separate sensitivity branch with $\text{ref} = \text{"nucl"}$; the $A=22$ valence partitions are nucleus-specific: ${}^{22}\text{Mg}(4p+2n)$, ${}^{22}\text{Na}(3p+3n)$, and ${}^{22}\text{Ne}(2p+4n)$.

\begin{table}[h!]
\centering
\caption{New B7D-1 Lane Production Parameters}
\begin{tabular}{ll}
\toprule
\textbf{Parameter} & \textbf{Value} \\
\midrule
$e_{\max}$ & 8 \\
$\text{Nnmax}$ & 14 \\
$\hbar\omega$ & 16~MeV \\
\texttt{calc\_3N} & true (effective two-body 2n3n contribution) \\
$k_F$ & $1.35~\text{fm}^{-1}$ \\
SRG & false \\
NuclearToolkit & v0.5.2 @ \texttt{dfc01916c7416a90600f84cb06b2aa91a481a983} \\
Julia & 1.10.10 \\
\bottomedrule
\end{tabular}
\end{table}

\subsection{The Central Lock}
The two lanes are physically distinct:
\begin{equation}
\mathbf{\Omega(e4, hw20) \neq \Omega(e8, hw16)}
\end{equation}
No saved Magnus operator, no bare $F_0/F_2$ block, no channel basis, ket mapping, normal-ordering reference, Pandya lookup, or BCH transport crosses between the lanes. The single object the two lanes share --- the \texttt{.snt.bin} binary contract of Section 4 --- is the only object that was verified to be identical across both frozen revisions, and the verification is part of this record (the D25b portability seal).

\section{The Certification Chain, D18 $\rightarrow$ D27}

\subsection{The Correction Arc (D18, D22/D23, D23b)}
The D18 runtime audit verified that a preceding claim --- that the legacy interaction binary had been ingested --- was false. The file was absent, and no SHA-256 freeze, no parse, no Hartree-Fock reconstruction, and no IMSRG evolution had occurred. D18 locked the corrected state and named the only legitimate exits: provision of the bytes, or retrieval via connector integration.

The exit was taken through the second door. The IMSRGNet repository --- the comparison-class repository of Yoshida et al., Phys. Rev. C 108, 044303 (2023) --- hosts a \texttt{snts} directory of NuclearToolkit interaction files, and the exact legacy file was present.

The file was retrieved, its SHA-256 frozen (\texttt{267c85b5870ca436d2a14960e5cf9d6e7da96d9eb8e057ebeb71405201e83cf}), and parsed field-by-field. Every structural invariant derivable from source was satisfied: 15 proton and 15 neutron orbits with $\max(2n+l) = 4$; single-particle energies reproducing the writer formula $(2n+l+3/2)\hbar\omega/2$ exactly; 34,320 two-body records with $34,320 \times 22$ bytes equal to the remaining file size and end-of-file reached exactly; $\hbar\omega = 20.0$ in both blocks; and an identically zero 2n3n column.

The semantic audit then subjected all 34,320 records to six rules derived from the reader and writer source: exchange canonicalization ($a \le b$, $c \le d$), pair ordering, channel purity by orbit-index parity, angular-momentum range, parity conservation, and identical-orbit antisymmetry.

\textbf{Violations:} none. The identical-orbit block distribution showed the exact even-$J$ ladder for every orbit, which simultaneously established fermion antisymmetry in every stored block, pinned the storage convention, and fixed the unique consistent reading of the source exchange-phase convention. The D18 ABSENT state was not erased. It was superseded by documented retrieval, and both states stand in the ledger.

\subsection{The Revision Arc (D21, D21b, D25c)}
Two audit threads had produced two D21 records. The D21b amendment reconciled them and advanced the state on every open item:
\begin{itemize}
    \item The branch \texttt{IMSRG-Net-v0} resolves to commit \texttt{11654a5224405db1fc3e03862372a9961b32f984}; the tag \texttt{v0.3.4} resolves to \texttt{51ce9fff0f9dac985a1915e34aecde7be1b818cf}. The full source trees of the two commits were compared recursively: \textbf{zero differing files}. The author-stated equivalence ``branch $\equiv$ v0.3.4'' was thereby promoted to a content-verified identity.
\item $\text{maxnormOmega} = 0.25$ was confirmed verbatim in the frozen constructor \texttt{init_IMSRGobject(HFobj; smax=500.0, dsmax=0.5, maxnormOmega=0.25, tol=1.e-6, eta_criterion=1.e-6, denominatorDelta=0.0)}.
\item \texttt{BetaCM} was resolved at source: ``Lawson's beta for Hcm'', default 0.0 on both revisions, implemented as $H = T_{\text{CM}} + (\beta M \hbar\omega^2 / 2\hbar^2c^2) \cdot R_{\text{CM}}^2$ with zero-point offset $1.5\beta\hbar\omega$.
\end{itemize}
The D25c correction fixed the new-lane Julia baseline: v0.5.2 declares \texttt{julia = "1.10"} in its own compat bounds, so the new lane runs under Julia 1.10.10 LTS, while Julia 1.8.5 remains the legacy baseline.
\subsection{The Contract Arc (D22 $\rightarrow$ D25b)}
Public documentation confirms the scalar types of the \texttt{.snt.bin} format --- two-body indices ($a, b, c, d, J$) as \texttt{Int16}, other integers as \texttt{Int64}, matrix elements as \texttt{Float32} --- but documents neither the field ordering nor the repetition structure. A parser written from the documentation alone would therefore be guessing.
The D22--D24 work derived the contract from the frozen function bodies instead: \texttt{write_spes} (binary mode), \texttt{write_tbme}, and \texttt{readsnt_bin}, with function-level anchors frozen for both revisions.
The contract, in brief: a four-integer header; $lp + ln$ orbit records of five \texttt{Int64} quantum numbers each; a single-particle block; a two-body header; and \texttt{count} two-body records of five \texttt{Int16} indices followed by three \texttt{Float32} matrix elements --- 22 bytes per record --- in the writer's canonicalized order, with exchange phases and pair ordering applied symmetrically by writer and reader, and with the reader composing $V_{2b} = V_{jj} + V_{2n3n} + V_{pp} \cdot \hbar\omega / A$ at ingest. The D25b seal then verified that this contract is byte-identical across the two frozen revisions.
\section{Results}
\subsection{The B7D-1 Production Interaction}
The programme executed its first production computation: Phase I interaction generation of the new lane, from the pinned parameter file under the pinned revision. The run completed and returned.
\begin{table}[h!]
\centering
\caption{B7D-1 Production Interaction Observed Properties}
\begin{tabular}{ll}
\toprule
\textbf{Property} & \textbf{Observed Value} \
\midrule
Orbits & $lp = ln = 45$ (90 total) \
Truncation & $\max(2n+l) = 8$ \
Oscillator & $\hbar\omega = 16.0$ in both blocks \
Single-particle records & 190 \
Two-body records & 3,526,624 \
Byte closure & $3,526,624 \times 22 = 77,585,728$ remaining bytes; EOF exact \
$V_{jj}$ range & $[-6.4907, +4.5434]$ \
$V_{2n3n}$ range & $[-1.9901, +2.1451]$ --- \textbf{nonzero} \
$V_{pp}$ range & $[-4.6273, +4.0000]$ \
Channels & $pn$: 1,763,568; $pp$: 882,307; $nn$: 880,749 \
Semantic violations & \textbf{0 / 3,526,624} \
Identical-orbit $J$ ladder & exact even-$J$ for $2j = 1, 3, \dots, 17$ \
\bottomedrule
\end{tabular}
\end{table}
\textbf{SHA-256 Vector Identity:} \
\texttt{050e9165e6e20c300116f34478e37190a45a1948126049d9e2015c10152c0c48}
The nonzero 2n3n column is the lane's defining content: the effective two-body contribution induced by three-nucleon forces is present in the generated bytes.
\subsection{The Legacy Hartree-Fock Blind Replay}
Under Julia 1.8.5 with NuclearToolkit v0.3.4, using the retrieved interaction, Hartree-Fock reconstruction was executed for both closed-shell reference nuclei.
\begin{table}[h!]
\centering
\caption{Hartree-Fock Reference Reconstruction Matrix}
\begin{tabular}{lllll}
\toprule
\textbf{Nucleus} & $\mathbf{E_{\text{HF}}}$ \textbf{(MeV)} & $\mathbf{E_{\text{1b}}}$ \textbf{(MeV)} & $\mathbf{E_{\text{2b}}}$ \textbf{(MeV)} & $\mathbf{E_{\text{MBPT(3)}}}$ \textbf{(MeV)} \
\midrule
${}^{16}\text{O}$ & \textbf{-132.95058} & +363.70 & -496.65 & -156.2804 \
${}^{40}\text{Ca}$ & \textbf{-518.07110} & +1244.59 & -1762.66 & -554.7142 \
\bottomedrule
\end{tabular}
\end{table}
In both cases, the decomposition $E = E_{1b} + E_{2b}$ closes exactly. These are HF- and HF-MBPT(3)-level energies of a two-body-only EM500 N3LO SRG-2.0 interaction in a four-major-shell space; they are not IMSRG(2) observables. The legacy HF replay is executed. It is not a new-lane result.
\subsection{The Two-Lane Clarification}
The quoted HF energies are legacy-lane results. They were produced under the legacy environment ($v0.3.4$, Julia 1.8.5, $e_{\max}=4$, $\hbar\omega = 20$~MeV, SRG 2.0). They are not new-lane results. The new B7D-1 production interaction has been generated and validated, but no HF calculation has been run on it.
\begin{equation}
\mathbf{\text{Legacy HF Replay} \neq \text{B7D-1 Production HF}}
\end{equation}
\section{The D28 Phase-II Control Freeze}
\subsection{Entry Condition}
Phase I complete ($\checkmark$).
\subsection{The Frozen Control Intent}
The D28 preflight freezes the Phase II IMSRG control parameters:
\begin{gather*}
\beta_{\text{CM}} = 0, \quad s_{\max} = 500, \quad ds_{\max} = 0.5 \
\Vert\Omega\Vert_{\max} = 0.25, \quad \text{tol} = 10^{-6}, \quad \eta_{\text{criterion}} = 10^{-6}, \quad \Delta_{\text{denom}} = 0
\end{gather*}
Primary reference: $\text{core} = \text{"O16"}$, $\text{ref} = \text{"core"}$, $\text{vspace} = \text{"sd-shell"}$. Sensitivity branch: $\text{ref} = \text{"nucl"}$. Magnus policy: \texttt{split}.
\subsection{The Preflight Behavior}
The D28 preflight does not run any HF or IMSRG calculation. It performs a runtime audit:
\begin{table}[h!]
\centering
\caption{Preflight Gating Conditions}
\begin{tabular}{ll}
\toprule
\textbf{Check} & \textbf{Behaviour on Failure} \
\midrule
Wrong lane detection & Hard-fail \
Wrong binary detection & Hard-fail \
Wrong Julia/package environment & Hard-fail \
Ambiguous IMSRG source control & Hard-fail \
Exact spelling of \texttt{magnusamethod} vs \texttt{magnusmethod} & Resolved from pinned source; FAIL if ambiguous \
\bottomedrule
\end{tabular}
\end{table}
The spelling resolution is a particularly good firewall move. Rather than guessing which spelling is correct, the preflight reads the pinned source tree and resolves the spelling before execution.
\subsection{The D28 Artifacts}
\begin{table}[h!]
\centering
\caption{Sealed Phase-II Preflight Artifact Register}
\begin{tabular}{ll}
\toprule
\textbf{Artifact} & \textbf{SHA-256 Hash} \
\midrule
\texttt{B7D1_D28_PHASEII_PREFLIGHT.jl} & \texttt{0839847df98f76548f804d8d3e9b197def7b8d8a79acc78982739b858b81d751} \
\texttt{F02_B7D_0D28_PHASEII_CONTROL_FREEZE_v1.js} & \texttt{8c87065357e6b327a74b8deaadc820fa3a27e80819508c701e674fd5414b5c5f} \
\texttt{RUN_B7D1_D28_WINDOWS.bat} & \texttt{5d514ea79e4760748b49ee8665bf187afc5f8282342667ea47dc1c06534f36d8} \
\bottomedrule
\end{tabular}
\end{table}
\subsection{The Expected Output}
On successful execution, the preflight produces:
\begin{verbatim}
STATUS=PASS_D28_PREFLIGHT
NEXT_GATE=D29_EXPLICIT_NEW_LANE_VSIMSRG_RUNNER
EXECUTED_PHYSICS=NONE
\end{verbatim}
and generates: \texttt{F02_B7D_0D28_PHASEII_PREFLIGHT_REPORT.txt}.
\newpage
\section{The Hash Register}
\begin{table}[h!]
\centering
\caption{Comprehensive Provenance Hash Identity Log}
\begin{tabular}{ll}
\toprule
\textbf{Artifact} & \textbf{SHA-256 Hash Identity} \
\midrule
Legacy interaction (757,376 B) & \texttt{267c85b5870ca436d2a14960e5cf9d6e7da96d9eb8e057ebeb71405201e83cf} \
B7D-1 interaction (77,593,968 B) & \texttt{050e9165e6e20c300116f34478e37190a45a1948126049d9e2015c10152c0c48} \
v0.3.4 source tarball & \texttt{a98b0636ac75198004b21372a9961b32f9845c62ca7d3ec6a8beed53ca9} \
IMSRG-Net-v0 tarball & \texttt{477599c8596025705858dd94be8804e11cdf426dab760d3239184e05aa73dafc} \
v0.5.2 source tarball & \texttt{9e22de09f9315b4fc8770d04cc36c7cd6138a02d184d7f1107ac19a126a08cca} \
B7D-1 pinned parameter file & \texttt{c19c29652b9840baaabdbb8748ea0c07eell0a1c85bb5870409a2f0014e6b729} \
New-lane Manifest & \texttt{5eabcfda61c35d536e0ea706f9addf4f843d2a0e5bfe327bad6faca746a347b8} \
Legacy HF output & \texttt{de9f118b0f7ca495b716ff82effelb26a17e41abc3445cle3866368d470f3d3} \
D24 schema document & \texttt{c76082437e82388aad34c1ff6fa41e3115d3a7418b2c48a5bc6954182780b6a0} \
D26 execution record & \texttt{5aa099db0eb82492151b92bd95f8a4813alcd6cla22419a4e0e666349cf3eff8} \
D27 HF replay record & \texttt{a0a58d2a09c9098ab131655b2be96246bdd382821932fe81453d3b595a4d11c6} \
D28 preflight script & \texttt{0839847df98f76548f804d8d3e9b197def7b8d8a79acc78982739b858b81d751} \
D28 control freeze cert & \texttt{8c87065357e6b327a74b8deaadc820fa3a27e80819508c701e674fd5414b5c5f} \
D28 Windows runner & \texttt{5d514ea79e4760748b49ee8665bf187afc5f8282342667ea47dc1c06534f36d8} \
Master ledger & \texttt{b6df8f43b6ed1de52f3fd5c3436dfdd3e93ac9a20409e09b68d93424b313e4cf} \
\bottomedrule
\end{tabular}
\end{table}
\section{Firewall Status and Open Gates}
Unchanged in substance:
\begin{gather*}
\text{D27 legacy HF replay} = \text{EXECUTED} + \text{HASH-FROZEN} \
\text{B7D-1 interaction} = \text{GENERATED} + \text{DUAL-VALIDATED} \
\text{D28 Phase II control freeze} = \text{PRE-REGISTERED}; \text{RUNTIME PASS AWAITED}
\end{gather*}
\begin{align*}
\text{Legacy } R_p^2 &= \text{NOT RUN} \
F_0/F_2 \text{ IMSRG(2)} &= \text{NOT RUN} \
M_{0,2}^{\text{ren}} (A=22) &= \text{NOT COMPUTED} \
\mathbf{\text{GRAVITY FIT}} &\mathbf{= \text{STRICTLY LOCKED}}
\end{align*}
The remaining gates are procedural and few: the D12 comparison (owner's frozen targets), the D29 new-lane O16-core VS-IMSRG production runner, the D30 legacy $R_n^2$ blind replay, the D31 new-lane $F_0/F_2$ operator evolution, and the D32 $A=22$ renormalized matrix elements.
\section{Conclusion}
A premature claim was caught and corrected. An absent input was declared absent, then legitimately retrieved. A binary contract was derived from source, sealed against two frozen revisions, and tested against 3,560,944 matrix element records in total with zero violations. Two computations were executed under two explicitly separated environments, and both of their outputs are hash-frozen artifacts of this programme. A Phase-II control freeze has been pre-registered, with a runtime preflight that resolves ambiguity from source rather than assuming.
The cost of the firewall was real: ten audits, two reconciled audit threads, three recorded corrections, and one failed execution day. Its purchase is the content of this article: every number above can be regenerated from frozen bytes by any independent party, and every correction above remains visible as a correction. That visibility is not a confession of weakness. It is the operating proof that the instrument works.
The programme now stands where it intended to stand: at the boundary between certification and evolution, holding a sealed interaction in each lane, with the path to the $A=22$ matrix elements open and the gravity fit untouched.
\begin{quote}
\textbf{\textit{``A pre-registered protocol is a commitment to a specific form of execution. When the inputs arrive, the protocol executes without modification.''}}
\end{quote}
\vspace{0.5cm}
\noindent \textbf{Tanfarid Vision Research Institute (TVRI)} \
\textit{Bogura, Bangladesh} \
\
\textit{``The universe does not merely contain entropy. It is organised by it.''} \
\textbf{--- Prof. Dr. Md. Faridul Islam Chowdhury}
\newpage
\section*{References}
\begin{enumerate}
\item Yoshida, S., et al. NuclearToolkit.jl, branch \texttt{IMSRG-Net-v0}, commit \texttt{11654a5224405db1fc3e03862372a9961b32f984}; tag \texttt{v0.3.4}, commit \texttt{51ce9fff0f9dac985a1915e34aecde7be1b818cf} (tree-identical pair). \url{github.com}.
\item Yoshida, S., et al. NuclearToolkit.jl v0.5.2, commit \texttt{dfc01916c7416a90600f84cb06b2aa91a481a983}. \url{github.com}.
\item Yoshida, S., et al. IMSRGNet: Code and data of IMSRG-Net. \url{github.com}. Phys. Rev. C \textbf{108}, 044303 (2023).
\item Stroberg, S. R., Morris, T. D., & He, H. Benchmark of IMSRG(2) and IMSRG(3) for two-particle systems. Phys. Rev. C \textbf{110}, 044316 (2024).
\item Hergert, H., Bogner, S. K., Morris, T. D., Schwenk, A., & Tsukiyama, K. The In-Medium Similarity Renormalization Group: A novel ab initio method for nuclei. Phys. Rep. \textbf{621}, 165 (2016).
\item Chowdhury, M. F. I. \textit{From Absence to Execution: The Complete B7D Certification Chain.} TVRI Monographs (2026).
\item Chowdhury, M. F. I. \textit{The D18 Runtime Ingest Audit.} TVRI Monographs (2026).
\item Chowdhury, M. F. I. \textit{The D21b Revision Reconciliation.} TVRI Monographs (2026).
\item Chowdhury, M. F. I. \textit{The D22--D24 Source-Extraction and Ingest Record.} TVRI Monographs (2026).
\item Chowdhury, M. F. I. \textit{The D25b Schema-Portability Seal.} TVRI Monographs (2026).
\item Chowdhury, M. F. I. \textit{The D26 Execution Record and D25c Correction.} TVRI Monographs (2026).
\item Chowdhury, M. F. I. \textit{The D27 Legacy HF Blind Replay Record.} TVRI Monographs (2026).
\item Chowdhury, M. F. I. \textit{The D28 Phase-II Control Freeze.} TVRI Monographs (2026).
\end{enumerate}
\newpage
\appendix
\section{B7D Status Table}
\begin{table}[h!]
\centering
\caption{System Metric Mapping and Verification Trail}
\begin{tabular}{lll}
\toprule
\textbf{Sub-Stage} & \textbf{Mission} & \textbf{Status} \
\midrule
B7D-0D10 & Pair-block BCH diagnostic & $\checkmark$ PASS \
B7D-0D12 & Independent observable benchmark & $\checkmark$ FROZEN \
B7D-0D13 & Acquisition & schema preflight & $\checkmark$ COMPLETED \
B7D-0D14 & Generic HF solver & $\checkmark$ PASS \
B7D-0D15 & HF normal-ordering bridge & $\checkmark$ PASS \
B7D-0D16 & $A=2$ truncation reconciliation & $\checkmark$ CORRECTED \
B7D-0D17 & Corrected production ledger & $\checkmark$ LOCKED \
B7D-0D18 & Runtime ingest audit & $\checkmark$ LOCKED \
B7D-0D19 & $A=22$ parameter-lane audit & $\checkmark$ PASS \
B7D-0D20 & Source-safe v2 parameter freeze & $\checkmark$ FROZEN, GUARDED \
B7D-0D21b & Revision-tree-identity reconciliation & $\checkmark$ PASS \
B7D-0D22 & Exact source extraction gate & $\checkmark$ READY, NOT EXECUTED \
B7D-0D23 & Production ingest gate & $\checkmark$ READY \
B7D-0D24 & Exact .snt.bin schema & $\checkmark$ PASS \
B7D-0D25b & Schema-portability seal & $\checkmark$ PASS \
B7D-0D25c & Julia-baseline compat correction & $\checkmark$ CORRECTED \
B7D-0D26 & New-lane Phase I generation & $\checkmark$ PASS \
B7D-0D27 & Legacy HF blind replay & $\checkmark$ PASS \
B7D-0D28 & Phase-II control freeze & $\dots$ PRE-REGISTERED \
B7D-0D29 & D12 blind comparison & $\dots$ WAITING D12 TARGETS \
B7D-0D30 & Legacy $R_p^2$ blind replay & $\mathbf{X}$ NOT RUN \
B7D-0D31 & New-lane $F_0/F_2$ evolution & $\mathbf{X}$ NOT RUN \
B7D-0D32 & $A=22$ renormalized $M_0, M_2$ & $\mathbf{X}$ NOT COMPUTED \
\bottomedrule
\end{tabular}
\end{table}
\section{Lane Distinction Summary}
\begin{table}[h!]
\centering
\caption{Parametric Contrast Layout between Validation and Production Classes}
\begin{tabular}{lll}
\toprule
\textbf{Attribute} & \textbf{Legacy Lane} & \textbf{New B7D-1 Lane} \
\midrule
$e_{\max}$ & 4 & 8 \
$\hbar\omega$ & 20~MeV & 16~MeV \
SRG & $2.0~\text{fm}^{-1}$ & false \
$k_F$ & --- & $1.35~\text{fm}^{-1}$ \
NuclearToolkit & v0.3.4 / IMSRG-Net-v0 & v0.5.2 @\texttt{dfc01916...} \
Julia & 1.8.5 & 1.10.10 \
Purpose & Validation & Production \
Interaction SHA-256 & \texttt{267c85b5...} & \texttt{050e9165...} \
HF status & $\checkmark$ EXECUTED & $\mathbf{X}$ NOT RUN \
\bottomedrule
\end{tabular}
\end{table}
\section{D28 Control Parameters}
\begin{table}[h!]
\centering
\caption{Locked Valuation Map for Verification Engine Parameters}
\begin{tabular}{lll}
\toprule
\textbf{Parameter} & \textbf{Frozen Value} & \textbf{Source} \
\midrule
$\beta_{\text{CM}}$ & 0 & Lawson CM beta, source default \
$s_{\max}$ & 500 & \texttt{init_IMSRGobject} default \
$ds_{\max}$ & 0.5 & \texttt{init_IMSRGobject} default \
$\Vert\Omega\Vert_{\max}$ & 0.25 & \texttt{init_IMSRGobject} default \
\texttt{tol} & $10^{-6}$ & \texttt{init_IMSRGobject} default \
\texttt{eta_criterion} & $10^{-6}$ & \texttt{init_IMSRGobject} default \
\texttt{denominatorDelta} & 0.0 & \texttt{init_IMSRGobject} default \
Primary reference & \texttt{core="O16"}, \texttt{ref="core"}, \texttt{vspace="sd-shell"} & Pre-registered \
Sensitivity reference & \texttt{ref="nucl"} & Pre-registered \
Magnus policy & \texttt{split} & Pre-registered \
\bottomedrule
\end{tabular}
\end{table}
\section{Firewall Declaration}
\begin{gather*}
\text{Physical } F_0/F_2 \text{ renormalized matrix elements} = \text{NOT COMPUTED} \
M_{0,22}^{\text{R,ren}} = M_{2,22}^{\text{R,ren}} = \text{NOT COMPUTED} \
\mathbf{\text{Gravity fitting = STRICTLY LOCKED}}
\end{gather*}
\vspace{0.3cm}
\noindent \textbf{Tanfarid Vision Research Institute (TVRI)} \
\textit{Bogura, Bangladesh} \
\
\small{\textit{``A mathematically formulated functional is not a cross-section. A research programme is not a validated theory.''}} \
\textbf{--- Prof. Dr. Md. Faridul Islam Chowdhury}
\end{document}


