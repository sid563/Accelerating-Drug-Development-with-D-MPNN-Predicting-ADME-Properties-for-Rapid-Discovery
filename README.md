# Accelerating Drug Development with D-MPNN Predicting ADME Properties for Rapid Discovery

**Introduction:**
ADME, a crucial property in drug discovery, has long been a challenge to predict accurately. Traditional methods rely on experimental determination, which is time-consuming and costly. Recent advances in machine learning offer a game-changing solution. Our project, 'ADME Prediction', harnesses the power of cutting-edge techniques like Graph Convolutional Neural Networks (GCNNs) and Directed Message Passing Neural Networks (DMPNN) to achieve unprecedented accuracy in ADME prediction. By leveraging these innovative methods, we aim to transform the drug discovery process, enabling faster and more efficient development of new treatments. Join us on this exciting journey to explore the potential of machine learning in revolutionizing ADME prediction!<br><br>
**Motivation:**
Accurate ADME prediction is crucial in drug discovery, but traditional methods are time-consuming, resource-intensive, and often inaccurate. Machine learning offers a solution, enabling fast and accurate predictions. Our project harnesses the latest techniques to revolutionize ADME prediction, accelerating drug development and improving drug efficacy and safety.<br><br>
**Scope of the Project:**
This project aims to develop and evaluate novel machine learning models for predicting ADME, leveraging techniques such as:-    
+ Various Regression Algorithms
+ Directed Message Passing Neural Networks (DMPNN)    <br>                                          
The project scope includes:-                                                                           
1. Data collection and preprocessing                                                                  
2. Model development and training                                                                 
3. Performance evaluation and comparison                                                     
4. Identification of optimal models and techniques<br>
By exploring the latest machine learning approaches, this project seeks to achieve unprecedented accuracy in ADME prediction, transforming the drug discovery process.<br><br><br>
**Methodology:**
Our dataset consists of 12,859 unique SMILES representations of chemical compounds with corresponding ADME values (logP), facilitating standardized input for our predictive model. The dataset encompasses a diverse range of chemical compounds, ensuring robustness and generalization capability, and undergoes preprocessing steps to ensure data integrity and suitability for predictive modeling. This comprehensive dataset enables accurate ADME predictions, enhancing our understanding of this crucial property in drug discovery and development.

![image](https://github.com/sid563/Accelerating-Drug-Development-with-D-MPNN-Predicting-ADME-Properties-for-Rapid-Discovery/assets/111000492/6676f481-d6da-42cb-8a28-f6b44f5b7ae7)


![image](https://github.com/sid563/Accelerating-Drug-Development-with-D-MPNN-Predicting-ADME-Properties-for-Rapid-Discovery/assets/111000492/d3bf1fcc-3c7f-4261-a721-45ff56b590be)  <br>
Our model utilizes initial atom and bond features computed through RDKit and initializes node and edge features in the D-MPNN. To enhance performance, we extend the model by treating groups of atoms as hyper-atoms and encoding nodes with feature vectors, which are then processed through a neural network to produce a molecular embedding. This approach generalizes existing atom features to incorporate information about functional groups.
![image](https://github.com/sid563/Accelerating-Drug-Development-with-D-MPNN-Predicting-ADME-Properties-for-Rapid-Discovery/assets/111000492/25adc9d3-5353-4264-a47e-2172f47dac22)
![image](https://github.com/sid563/Accelerating-Drug-Development-with-D-MPNN-Predicting-ADME-Properties-for-Rapid-Discovery/assets/111000492/9ff9a0b3-ae58-4b28-8b8b-9f7eba2a8bdf)

<br>
Directed MPNN (D-MPNN) is a variant of MPNN that exchanges messages along directed edges (bonds) to prevent "tottering" and capture meaningful relationships in molecular graphs. Unlike traditional MPNNs, D-MPNN propagates messages along directed edges, avoiding cyclic paths and aligning with belief propagation in probabilistic graphical models. This approach enhances the network's ability to capture structural characteristics and improve property prediction accuracy.
<br>
Ensemble learning combines multiple Directed Message Passing Neural Networks (D-MPNNs) to improve ADME prediction accuracy and robustness. By training diverse models and aggregating their predictions, ensemble learning mitigates overfitting and captures a wider range of patterns in the data. This approach achieves superior predictive performance and provides valuable insights into prediction uncertainty.
<br>

**Result:**
In this study, we employed various regression algorithms to predict lADME, a crucial property in drug discovery. Our results demonstrate the effectiveness of these algorithms in predicting ADME, with notable variations in performance.
![image](https://github.com/sid563/Accelerating-Drug-Development-with-D-MPNN-Predicting-ADME-Properties-for-Rapid-Discovery/assets/111000492/e23c815d-3335-4abd-9c35-997fb0afecc9)
<br>
![image](https://github.com/sid563/Accelerating-Drug-Development-with-D-MPNN-Predicting-ADME-Properties-for-Rapid-Discovery/assets/111000492/6c80c1ad-27d9-4672-a8d4-d4181caa7ce3)
![image](https://github.com/sid563/Accelerating-Drug-Development-with-D-MPNN-Predicting-ADME-Properties-for-Rapid-Discovery/assets/111000492/070152f7-b5dd-4449-97b9-21bd4bb8e297)

The Polynomial Kernel Ridge algorithm with an alpha value of 0.01 achieved the highest R-squared value of 0.2464, indicating a strong goodness of fit. Additionally, it yielded a Mean Squared Error (MSE) of 1.137, suggesting a high accuracy in predictions. The Polynomial Regression with Elastic Net Regularization (alpha = 0.01121, l1_ratio = 0.1) also performed remarkably well, with an R-squared value of 0.2817 and an MSE of 1.0842.Other algorithms, including Multilinear Regression, Linear Kernel Ridge, Lasso Regression, and Elastic Net Regression, showed relatively lower performance, with R-squared values ranging from 0.1937 to 0.206 and MSE values between 1.1987 and 1.217.
![image](https://github.com/sid563/Accelerating-Drug-Development-with-D-MPNN-Predicting-ADME-Properties-for-Rapid-Discovery/assets/111000492/88917316-8349-4d5f-9c5c-9b11b918d09c)

we evaluated the performance of our proposed ensemble learning approach for predicting ADME values. Leveraging a combination of molecular substructure representation and the Directed Message Passing Neural Network (DMPNN) model architecture, our methodology achieved notable success in accurately predicting ADME values. Upon evaluation our model consistently outperformed previous approaches. Specifically, our model achieved a test loss of 0.2008, a test MAE of 0.3648, a test MSE of 0.0972, a test RMSE of 0.3117, and a test **_R^2 of 0.9607_**, which collectively represent the highest level of accuracy attained thus far in ADME prediction tasks. <br> <br>
**Conclusion:**
These results underscore the effectiveness of our ensemble learning strategy, which combines multiple models trained with different initial weights to improve predictive performance. Moreover, our approach demonstrates the importance of incorporating molecular substructure information into the model's representation of chemical compounds, enabling more accurate predictions of ADME values.














