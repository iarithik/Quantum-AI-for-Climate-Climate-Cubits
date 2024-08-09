# Optimizing Battery Temperature for Electric Vehicles Using Quantum Annealing: Implications for Grid Load Management and Carbon Emission Reduction

## Overview

This project explores the optimization of battery temperature management in lithium-ion (Li-On) batteries for electric vehicles (EVs) using quantum annealing. By focusing on maintaining an optimal State of Charge (SoC) and improving the State of Health (SoH), the project aims to enhance battery life, improve EV performance, facilitate smart charging strategies, and contribute to carbon emission reduction.

## 1. Problem Statement

Optimizing battery temperature is crucial because:

- **Battery Temperature:** Affects the SoH and efficiency of EV batteries, directly impacting their lifespan. [Related article](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC4526891/)
- **State of Charge (SoC):** Keeping SoC within optimal ranges is vital for efficient battery operation and user experience. [Reference article](https://www.sciencedirect.com/science/article/pii/S2352152X23025422)
- **Grid Load Management:** Optimized battery performance can enable more effective smart charging strategies, reducing peak-time grid stress. [Article on smart charging](https://www.sciencedirect.com/science/article/abs/pii/S2210670723003190)
- **Carbon Emissions:** Efficient battery management can lead to better utilization of low-carbon energy sources, aiding in the reduction of carbon emissions. [Article on carbon emissions](https://www.sciencedirect.com/science/article/abs/pii/S0306261921002518)

## 2. Background Research and Literature Review

The literature review focused on several key areas:

- **Quantum Optimization in Climate Science:** Explored potential applications of quantum computing for addressing climate challenges. [Quantum Optimization]([2107.05362 (arxiv.org)](https://arxiv.org/pdf/2107.05362)) by Stuart Hadfield and Michał Stęchły.
- **Smart Charging Strategies:** Analyzed the impact of smart charging on grid load and carbon emissions. [Smart charging strategy for electric vehicles]([Smart charging strategy for electric vehicles based on marginal carbon emission factors and time-of-use price - ScienceDirect](https://www.sciencedirect.com/science/article/abs/pii/S2210670723003190)) (ScienceDirect).
- **Battery State Estimation Methods:** Compared classical, AI, and quantum methods for estimating SoH and SoC. 
	- Classical Model : Implementing the Extended Kalman Filter for SoH and SoC estimation.[Energies | Free Full-Text | Implementing an Extended Kalman Filter for SoC Estimation of a Li-Ion Battery with Hysteresis: A Step-by-Step Guide (mdpi.com)](https://www.mdpi.com/1996-1073/14/13/3733)
	- Quantum Models: quantum algorithm optimized stacking : [Lithium-ion battery state of health estimation method based on variational quantum algorithm optimized stacking strategy - ScienceDirect](https://www.sciencedirect.com/science/article/pii/S2352484724001148#da0005)
	- AI Models: SoH estimation using machine learning and AI models
		- CNN and Random Forest : [2010.10452 (arxiv.org)](https://arxiv.org/pdf/2010.10452)
		- Support Vector Machine:[SOH estimation of lithium-ion batteries based on least squares support vector machine error compensation model | Journal of Power Electronics (springer.com)](https://link.springer.com/article/10.1007/s43236-021-00307-8)
		- Deep Learning :[Open access dataset, code library and benchmarking deep learning approaches for state-of-health estimation of lithium-ion batteries - ScienceDirect](https://www.sciencedirect.com/science/article/abs/pii/S2352152X23032826)
		- LSTM : [Prediction of Li-ion battery state of health based on data-driven algorithm - ScienceDirect](https://www.sciencedirect.com/science/article/pii/S2352484722025215)
 - **QUBO and Quantum Annealing Approach**:
	 - **QUBO and Quantum Annealing:** Investigated QUBO formulation and quantum annealing techniques for optimization. Explore more in [D-Wave's resources](https://www.youtube.com/watch?v=Hw6CKoB3B6I).
	- **QUBO to Quantum Annealing Referenced Books ** [A Practical Guide to Quantum Machine Learning and Quantum Optimization](https://github.com/PacktPublishing/A-Practical-Guide-to-Quantum-Machine-Learning-and-Quantum-Optimization/blob/main/Chapter04/Chapter_04_code.ipynb) and [Quantum bridge analytics I: a tutorial on formulating and using QUBO models](https://link.springer.com/article/10.1007/s10479-022-04634-2).
	- **Quantum Annealing Problem with Constraints and Penalties Reference:** [Solving the resource constrained project scheduling problem with quantum annealing](https://www.nature.com/articles/s41598-024-67168-6).

## 3. Methodology

The methodology for the project includes:

- **Data Preparation:** Converted NASA battery datasets from MATLAB to CSV format, and processed data for SoC calculation.
- **Objective Function Formulation:** Used statistical method to derive the objective function for the QUBO problem, targeting temperature minimization.
- **QUBO Formulation:** Developed the Q matrix for the quantum annealing process.
- **Quantum Annealing:** Currently working on embedding the objective function for D-Wave's quantum annealer.

## 4. Computational Resources

- **Data Processing and ML Training:** Conducted on standard CPUs/GPUs.
- **Quantum Annealing:** Utilized D-Wave's quantum annealer for the optimization problem.

## 5. Results and Potential Impact

While still in progress, the project has the potential to:

1. **Extend Battery Life and Improve EV Performance:** Better temperature management could lead to longer battery life and enhanced EV performance.
2. **Optimize Smart Charging Strategies:** More accurate SoC,SoH estimation can lead to optimized charging, reducing grid load during peak hours.
3. **Reduce Carbon Emissions:** By optimizing the use of low-carbon energy sources during charging, carbon emissions could be significantly lowered.

## 6. Next Steps

- **Compare Classical, AI, and Quantum Methods:** Assess the performance of different methods in optimizing SoH and SoC.
- **Optimize Constraints and Penalties:** Fine-tune the QUBO formulation for better results.
- **Expand Literature Review:** Continue to explore emerging research in battery management and quantum optimization.
