# Dictionary-Based Quantum LDPC Decoder

This repository contains Python code and synthetic datasets used in our research on symbolic, dictionary-based decoding of Quantum LDPC (QLDPC) codes.   
Instead of dense linear algebra, our framework models quantum states, errors, stabilizers, and correction rules with Python dictionaries. This makes error correction efficient, interpretable, and traceable. 
 Features 
- Dictionary-based modeling of quantum errors and stabilizers  
- Rule-based syndrome measurement and correction  
- Simulation of QLDPC codes with synthetic $X$, $Y$, $Z$ errors  
- Metrics for explainability:
  -Explainable Fidelity (XF) 
  - Trust Flow (TF) 
  - Correction Path Entropy (CPE)
- Visualizations: bar charts, line plots, heatmaps, and entropy histograms  
#Contents 
- `decoder.py` → Core methods for symbolic error decoding  
- `simulation.py` → Simulation experiments and metrics  
- `synthetic_qldpc.csv` → Synthetic dataset with injected errors, syndromes, corrections, and explainability scores  
- `plots/` → Figures generated for the paper (XF, TF, heatmaps, entropy histograms)  

git clone https://github.com/Sarwar899030/qldpc_symbolic_decoder.git 
cd qldpc-symbolic-decoder

# Install dependencies
pip install -r requirements.txt

# Run experiments
python simulation.py
