Algorithmic Components
=====================
PrismBO is equipped with a collection of state-of-the-art TLBO algorithms, all implemented following object-oriented design principles. The following tutorial pages provide an overview of the different algorithmic components and illustrate how they are initialized and executed within the PrismBO framework.

.. admonition:: Overview
   :class: info

   - :ref:`Transfer Learning for Acquisition Function <components/acf/acf>`: How to refine the acquisition function using data to better balance exploration and exploitation.

..    - :ref:`Transfer Learning for Search Space Design <problem-specification>`: How to use data to reshape the search space, improving search efficiency.
..    - :ref:`Transfer Learning for Initialization Design <initialization-design>`: How to utilize data to warm-start the optimization process with informative initial configurations.
..    - :ref:`Transfer Learning for Surrogate Model <surrogate-model>`: How to enhance the surrogate model by incorporating knowledge from previously learned models or task-specific data.





.. toctree::
   :maxdepth: 2
   :caption: Component Submodules

   acf/acf
..    acf/fsaf
..    acf/taf
..    initialization/initialization
..    model/model
..    space/space