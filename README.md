# History-Resolved pi_f Anticipatory Self-Healing Conductance Law

TopEquations promoted equation bundle for `eq-history-resolved-pif-anticipatory-self-healing-law`.

**Score:** 91  
**TopEquations rank:** 19  
**Units:** OK  
**Theory:** PASS

## Equation

$$
\dot g_e = \alpha_G(S)\,[1+\xi H_e^{(f)}] \,|J_e|\,e^{i\Theta_e} - \mu_G(S)\,g_e - \lambda_s g_e\sin^2\!\left(\frac{\Theta_e}{2\pi_a}\right) + \chi C_e g_e
$$

## Precursor term

The local flat-adaptive precursor used in the writeup is

$$
H_e^{(f)}=\sum_{\ell\ni e} w_{e\ell}\,\tanh\!\left(\frac{\Sigma_\ell^{(f)}-\Sigma_{\ell,\mathrm{ref}}^{(f)}}{\sigma_\ell+\varepsilon}\right)
$$

This makes `pi_f` an anticipatory loop-health observable rather than a passive readout.

## Lineage

- Builds on LB #1 History-Resolved Phase with Adaptive Ruler.
- Builds on LB #31 Adaptive Topological Self-Healing Conductance Law.
- Builds on LB #8 Flat-Channel Loop Signature (pi_f Health Observable).
- Remains compatible with the local deficit-gated repair viewpoint in LB #14.

## Bundle contents

- `data/benchmark_results.csv` and `data/benchmark_summary.csv`: committed graph-mode ablation tables.
- `data/pif_anticipatory_self_healing_metrics.json`: computed deltas and bundle-consistency checks.
- `data/pif_anticipatory_self_healing_report.md`: short score-facing report.
- `images/benchmark_summary.png`: original mode-level summary plot.
- `images/maze_trace_seed0.png`: representative maze trace.
- `images/pif_anticipatory_self_healing_dashboard.png`: repo-native dashboard.
- `images/pif_anticipatory_self_healing_preview.gif`: repo-native preview animation.
- `notes/derivation_bridge.md`: parent-law bridge.
- `notes/falsifiers.md`: falsification criteria.
- `notes/top_equations_evidence_block.md`: stronger evidence wording.
- `simulations/benchmark_pif_98plus.py`: original benchmark harness snapshot.
- `simulations/generate_pif_anticipatory_self_healing_artifacts.py`: local renderer for the committed bundle.

## Rebuild local preview assets

From the repository root run:

```bash
python simulations/generate_pif_anticipatory_self_healing_artifacts.py
```

That command rebuilds:

- `images/pif_anticipatory_self_healing_dashboard.png`
- `images/pif_anticipatory_self_healing_preview.gif`
- `data/pif_anticipatory_self_healing_metrics.json`
- `data/pif_anticipatory_self_healing_report.md`

## Important note about the original benchmark script

`simulations/benchmark_pif_98plus.py` is preserved as the upstream graph-mode benchmark harness snapshot. It expects the external modules `hafc_sim` and `hafc_sim_pif_active`, which are not committed in this repo. In this repository, the supported reproduction path is the local renderer above, which validates and repackages the committed CSV and image bundle.

## Headline findings

- Maze-mode recovery ratio improves from `0.998467` to `1.008786` with `pi_f` enabled.
- Maze-mode tail loop-mismatch residual falls from `0.033686` to `0.003943`, an `88.30%` relative reduction.
- Classic-mode final conductance ratio rises from `0.986924` to `1.023769` with `pi_f` enabled.
- Classic-mode tail mismatch also rises to `0.004914`, so the present empirical support is stronger in maze mode than in classic mode.
- The committed 10-seed bundle is numerically deterministic across listed seeds in this package.

## Current limits

- The present evidence is graph-mode only.
- Lattice or EGATL ablations with the same `pi_f` channel are still missing.
- A `lambda_s = 0` lattice ablation is not yet included.
- A direct precursor lead-time comparison against Bott or Chern observables is not yet included.

## Links

- [TopEquations leaderboard](https://rdm3dc.github.io/TopEquations/leaderboard.html)
- [TopEquations main repo](https://github.com/RDM3DC/TopEquations)
- [Equation certificate registry](https://rdm3dc.github.io/TopEquations/certificates.html)