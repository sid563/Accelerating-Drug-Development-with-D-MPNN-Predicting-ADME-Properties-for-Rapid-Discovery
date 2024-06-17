# Accelerating-Drug-Development-with-D-MPNN-Predicting-ADME-Properties-for-Rapid-Discovery

**Introduction:**
ADME, a crucial property in drug discovery, has long been a challenge to predict accurately. Traditional methods rely on experimental determination, which is time-consuming and costly. Recent advances in machine learning offer a game-changing solution. Our project, 'ADME Prediction', harnesses the power of cutting-edge techniques like Graph Convolutional Neural Networks (GCNNs) and Directed Message Passing Neural Networks (DMPNN) to achieve unprecedented accuracy in ADME prediction. By leveraging these innovative methods, we aim to transform the drug discovery process, enabling faster and more efficient development of new treatments. Join us on this exciting journey to explore the potential of machine learning in revolutionizing ADME prediction!<br>
**Motivation:**
Accurate lipophilicity prediction is crucial in drug discovery, but traditional methods are time-consuming, resource-intensive, and often inaccurate. Machine learning offers a solution, enabling fast and accurate predictions. Our project harnesses the latest techniques to revolutionize lipophilicity prediction, accelerating drug development and improving drug efficacy and safety.<br>
**Scope of the Project:**
This project aims to develop and evaluate novel machine learning models for predicting lipophilicity, leveraging techniques such as:-    
    Various Regression Algorithms                                                                      Directed Message Passing Neural Networks (DMPNN)                                              The project scope includes:-                                                                           Data collection and preprocessing                                                                  Model development and training                                                                 
    Performance evaluation and comparison                                                     
    Identification of optimal models and techniques                                                By exploring the latest machine learning approaches, this project seeks to achieve unprecedented accuracy in lipophilicity prediction, transforming the drug discovery process.<br>
**Methodology:**
Our dataset consists of 12,859 unique SMILES representations of chemical compounds with corresponding lipophilicity values (logP), facilitating standardized input for our predictive model. The dataset encompasses a diverse range of chemical compounds, ensuring robustness and generalization capability, and undergoes preprocessing steps to ensure data integrity and suitability for predictive modeling. This comprehensive dataset enables accurate lipophilicity predictions, enhancing our understanding of this crucial property in drug discovery and development.
![image](https://github.com/sid563/Accelerating-Drug-Development-with-D-MPNN-Predicting-ADME-Properties-for-Rapid-Discovery/assets/111000492/6f64980f-b44c-49cd-b52e-674a4724bc8a)
![image](https://github.com/sid563/Accelerating-Drug-Development-with-D-MPNN-Predicting-ADME-Properties-for-Rapid-Discovery/assets/111000492/d3bf1fcc-3c7f-4261-a721-45ff56b590be)  <br>
Our model utilizes initial atom and bond features computed through RDKit and initializes node and edge features in the D-MPNN. To enhance performance, we extend the model by treating groups of atoms as hyper-atoms and encoding nodes with feature vectors, which are then processed through a neural network to produce a molecular embedding. This approach generalizes existing atom features to incorporate information about functional groups.
![image](https://github.com/sid563/Accelerating-Drug-Development-with-D-MPNN-Predicting-ADME-Properties-for-Rapid-Discovery/assets/111000492/5ae88ef8-a94f-4ec4-8072-1bd076504d4b)
<br>
![image](https://github.com/sid563/Accelerating-Drug-Development-with-D-MPNN-Predicting-ADME-Properties-for-Rapid-Discovery/assets/111000492/a34e2e39-14d4-4bb9-9820-47ad96012c20)







