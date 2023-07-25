# Machine-Learning-Techniques-for-State-Estimation-of-Low-Voltage-Tranmission-System

Distribution systems operators’ (DSO) upcoming challenge is to monitor and control low voltage (LV) grids. Real time measurements’ acquisition from LV grids has become possible thanks to the deployment of smart meters (SM) but it is still limited by technical constraints. Thus, a real time state estimator (SE) is needed to ensure the LV grid’s observability. A machine learning model can be trained using the SM historical data and then run in real time using few available measurements to estimate the system’s state. For the purpose of evaluating the performance of a machine learning based SE on a realistic LV grid, an auto-encoder based SE is presented in this paper. An accuracy enhancement using pseudo-measurements is proposed and a method for reconstructing realistic LV grid models is also described. 

The newly developed Deep Auto-Encoder - Particle Swarm Optimization state estimator was able to retrieve missing data from about 64% of unmeasured nodes without pseudo-measurements and up to 96% with pseudo-measurements. This ability was indicated to be within 2% of the error margin for constrained nodes and 1% for unconstrained nodes.

To achieve this high missing state estimation performance, I developed the Auto-Encoder by using a Deep Structure which acquired the capability to learn complex data relations as represented in the case study of 25 nodes each of which contains 3 dimensional fields of state (75 data features in total). The PSO then used the pre-trained Deep Auto-Encoder to finetune and reconstruct the missing states from input available nodal data measurements.

There are multiple benefits resulting from this technique:
1. Fast estimating time (about 1 second for each node) to be potentially applied for real-time state estimation.
2. Flexibility due to the symmetrical structure of the pre-trained Auto-Encoder, which can help the model adapt to various missing data scenarios in different nodes.
3. High level of automation with the application of hyperparameters used to select high-performance model parameters for Auto-Encoder's structure for different nodal networks.

This is my thesis project for the final year of my Master's Degree at the University Paris-Saclay. It paves the way for the publication of the article entitled "PERFORMANCE EVALUATION OF AN AUTOENCODER STATE ESTIMATOR WITH REALISTIC LOW VOLTAGE GRIDS RECONSTRUCTED FROM OPEN DATA" at the CIRED 2023 conference taking place on the 15th of June in Rome, Italy. 

For more information, please take a look at the selected list of papers: https://www.cired2023.org/wp-content/uploads/2023/05/2023_full_papers_selected_list.pdf 

Due to the copyright and confidentiality of the research program and the hosted organization, the detailed implementation of my work was forced to be kept obscured.
Instead, my thesis and the published paper in CIRED 2023 were uploaded for your further viewing.

Many thanks and best wishes!


