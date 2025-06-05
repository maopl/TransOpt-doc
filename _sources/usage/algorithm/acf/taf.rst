.. _taf:

TAF
================================

Overview
--------

TAF comes from **Scalable Gaussian process-based transfer surrogates for hyperparameter optimization**:cite:`WistubaSS18`.

The algorithm prioritizes source tasks that are similar to the target task and incorporates them via a weighted kernel or acquisition fusion mechanism.
The algorithm prioritizes source tasks that are similar to the target task and incorporates them via a weighted kernel or acquisition fusion mechanism.

Key contributions include:

- A task similarity-aware acquisition aggregation strategy.
- Theoretical regret analysis for fusion weights.
- Empirical improvements over naïve acquisition merging baselines.

Visualization
-------------

.. .. image:: ../_static/taf_example.png
..    :width: 80%
..    :align: center
..    :alt: TAF example visualization

Code Usage
----------

.. code-block:: python

   from prismbo.components.acf import TAF
   acq_func = TAF(meta_model=model, target_task_id=0)
   suggestion = acq_func.suggest(X_candidate)

Comparison
----------

+-----------+------------------+--------------------------+
| Method    | Regret (↓)       | Transfer Utilization     |
+===========+==================+==========================+
| TAF       | **0.089**        | High                     |
+-----------+------------------+--------------------------+
| FSAF      | 0.113            | Medium                   |
+-----------+------------------+--------------------------+
| GP-UCB    | 0.165            | None                     |
+-----------+------------------+--------------------------+

References
----------

- AuthorName et al. "Task-Aware Fusion for Transferable Acquisition Functions". NeurIPS 2023.