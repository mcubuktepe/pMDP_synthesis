# pMDP_synthesis
This repository contains benchmark files for Convex Optimization for Parameter Synthesis in MDPs

## Parameter Synthesis with Convex Optimization using Stormpy and Prophesy

We have implemented convex-optimization-based methods for convex optimization using Stormpy and Prophesy.

## Dependencies


The packages has been tested on a clean Ubuntu 20.04 LTS installation and Python 3.8 with [gurobipy](https://www.gurobi.com/downloads/gurobi-software/), [stormpy](https://moves-rwth.github.io/stormpy/), and [prophesy](https://github.com/mcubuktepe/prophesy) installed.

Specifically, we tested the code with Gurobi 9.1.2, and Stormpy with commit id 0f9aa3af2de7540eb051fcfcab7a5eac1bef495a.


## Reproducibility Instructions

We provide the command in order to reproduce the results in the paper. Note that the directory expected_results/ contains the results for different models using different approaches. The first line of each file also gives the command for running the code.

For example, in the file "expected_results/pMC/brp/brp_16_2_pm_delta_2_0_gamma_1_5_affine_0_1", the command "python3 parameter_synthesis.py load-problem prism/brp/brp_16_2.pm prism/brp/brp.prctl set-threshold 0.1 find-feasible-instantiation --qcqp-incremental --qcqp-mc full below affine"  runs the SCP approach on the benchmark model "brp_16_2.pm" with specification "brp.prctl" and threshold 0.1.
