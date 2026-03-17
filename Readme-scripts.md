# DVS - Distributed Viability Score
[![PyPI downloads](https://img.shields.io/pypi/dm/your-package-name?label=PyPI%20downloads)](https://pypi.org/project/hypaq/)
[![Stack Overflow](https://img.shields.io/badge/stackoverflow-Ask%20questions-blue)](https://stackoverflow.com/questions/tagged/hypaq)
[![DOI](https://img.shields.io/badge/DOI-10.1109%2FQCE57702.2023.00055-blue)](https://doi.org/10.48550/arXiv.2504.09318)
[![Contribute](https://img.shields.io/badge/Contribute-Good%20First%20Issue-brightgreen)](https://github.com/hypaq/hypaq/issues?q=is%3Aissue+is%3Aopen+label%3A%22good+first+issue%22)

Variational Quantum Algorithms (VQAs) are widely seen as one of the most practical methods for near-term quantum computing, but their scalability remains limited by qubit availability, noise, transpilation overhead, and sampling cost. Distributed quantum computing and circuit cutting aim to extend execution across multi-QPU architectures and quantum networks. However, distribution is not inherently advantageous, as it depends on problem structure, ansatz and mixer locality, partitioning strategy, and communication overhead. This paper proposes a network-sensitive framework for Distributed VQAs (D-VQAs) that combines hypergraph partitioning, ansatz-aware and mixer-aware strategies, and a cost perspective including local execution, communication, synchronization, sampling, and reconstruction. The framework identifies viability regimes in which distribution may provide architectural advantage or be dominated by network overhead.

As a first step in the analysis, we consolidated the many dimesions from benchmark circuits, comparing the qubit connectivity, size, width, density, to visualize the behaivor and first impressions about different structures of QAOQ and VQE algorithms. Two first scripts to run those tasks are presented:

Script: dvs 01 - reading benchmark circuits for dimensions: [Scripts documentation](./dvs 01 - reading benchmark circuits for dimensions.ipynb)
Script: dvs 02 - drawing dimensions from benchmark circuits: [Scripts documentation](./dvs 02 - drawing dimensions from benchmark circuits.ipynb)

From where we created several insights:

<div align="center">
  <img src="boxplot_depth_by_group_20260317_004135.png" alt="dvs" width="1000"/>
  <br/>
  <strong>Boxplot Depth by Group</strong>
</div>                                                            

<div align="center">
  <img src="heatmap_group_metrics_20260317_004135.png" alt="dvs" width="1000"/>
  <br/>
  <strong>Heatmap Group Metrics</strong>
</div>

<div align="center">
  <img src="scatter_depth_vs_qubits_20260317_004135.png" alt="dvs" width="1000"/>
  <br/>
  <strong>Scatter Depth vs qubits</strong>
</div>

<div align="center">
  <img src="stacked_two_qubit_gates_by_group_20260317_004135.png" alt="dvs" width="1000"/>
  <br/>
  <strong>Stacked two qubit gates by group</strong>
</div>  

<div align="center">
  <img src="two_qubit_density_boxplot_20260317_004135.png" alt="dvs" width="1000"/>
  <br/>
  <strong>Two_qubit_Density_Boxplot</strong>
</div>        

<div align="center">
  <img src="two_qubit_density_by_group_20260317_004135.png" alt="dvs" width="1000"/>
  <br/>
  <strong>Two qubit Density by Group</strong>
</div>

The complete dataset with all benchmark quantum curcuits used for this research is published at IEEE DATAPORT, as follows:

<div align="center">
  <img src="img_ieee_dataport.png" alt="dvs" width="1000"/>
  <br/>
  <strong>dataset at IEEE DataPort</strong>
</div>

Waldemir Cambiucci, "A Network-Sensitive Framework for Variational Quantum Optimization on Multi-QPU Architectures", IEEE Dataport, March 15, 2026, doi:10.21227/s9b5-qy94
https://ieee-dataport.org/documents/network-sensitive-framework-variational-quantum-optimization-multi-qpu-architectures
