<div align="center">
  <img src="\hypaq\dvs.png" alt="dvs" width="100"/>
  <br/>
  <strong>DVS - Distributed Viability Score</strong>
</div>

# DVS - Distributed Viability Score
[![PyPI downloads](https://img.shields.io/pypi/dm/your-package-name?label=PyPI%20downloads)](https://pypi.org/project/hypaq/)
[![Stack Overflow](https://img.shields.io/badge/stackoverflow-Ask%20questions-blue)](https://stackoverflow.com/questions/tagged/hypaq)
[![DOI](https://img.shields.io/badge/DOI-10.1109%2FQCE57702.2023.00055-blue)](https://doi.org/10.48550/arXiv.2504.09318)
[![Contribute](https://img.shields.io/badge/Contribute-Good%20First%20Issue-brightgreen)](https://github.com/hypaq/hypaq/issues?q=is%3Aissue+is%3Aopen+label%3A%22good+first+issue%22)

Variational Quantum Algorithms (VQAs) are widely seen as one of the most practical methods for near-term quantum computing, but their scalability remains limited by qubit availability, noise, transpilation overhead, and sampling cost. Distributed quantum computing and circuit cutting aim to extend execution across multi-QPU architectures and quantum networks. However, distribution is not inherently advantageous, as it depends on problem structure, ansatz and mixer locality, partitioning strategy, and communication overhead. This paper proposes a network-sensitive framework for Distributed VQAs (D-VQAs) that combines hypergraph partitioning, ansatz-aware and mixer-aware strategies, and a cost perspective including local execution, communication, synchronization, sampling, and reconstruction. The framework identifies viability regimes in which distribution may provide architectural advantage or be dominated by network overhead.
