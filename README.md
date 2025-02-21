# Code_Article_Colaboratory
The code used to process, train and visualize the data from the submitted article.

# Reservoir Characterization with NMR Data and MLP Model  

## 1. Processing of NMR (Nuclear Magnetic Resonance) Data  
- The code processes NMR data for the petrophysical characterization of reservoir rock samples.  
- This may involve normalizing \( T_2 \) by porosity and distribution.  
- These data are essential for estimating petrophysical properties such as permeability.  

## 2. Training the MLP (Multi-Layer Perceptron) Model  
- An MLP (Multi-Layer Perceptron) model is an artificial neural network used to learn patterns in the data and predict permeability.  
- In the context of the article, the MLP is trained with NMR data to predict permeability values, aiming to perform reservoir characterizations based on FZI, RQI, and HFU classifications.  
- The training process may include:  
  - Input data normalization  
  - Splitting into training and test sets  
  - Tuning hyperparameters (number of layers, neurons, learning rate)  
  - Evaluating performance using metrics such as Mean Squared Error (MSE) or the coefficient of determination \( R^2 \).  

## 3. Visualization of Reservoir Characterization Data (FZI, RQI, HFU)  
### **FZI (Flow Zone Indicator)**  
An indicator that classifies flow zones in a reservoir based on the relationship between porosity and permeability. It is calculated as:  

\[
FZI = \frac{RQI}{\phi_e}
\]

where:  
- \( RQI \) is the **Reservoir Quality Index**  
- \( \phi_e \) is the **effective porosity**  

### **RQI (Reservoir Quality Index)**  
Represents the rock’s ability to store and transmit fluids and is given by:  

\[
RQI = 0.0314 \times \sqrt{\frac{k}{\phi}}
\]

where:  
- \( k \) is the **permeability** (mD)  
- \( \phi \) is the **fractional porosity**  

### **HFU (Hydraulic Flow Units)**  
Hydraulic flow units (HFUs) group reservoir zones with similar petrophysical characteristics. HFUs are defined based on the FZI distribution and help segment reservoir regions with different flow behaviors.  

### **Data Visualization**  
The visualization of these data may include:  
- Scatter plots  
- Histograms  
- Heat maps  

These techniques help in better understanding the relationships between variables. Additionally, clustering techniques can be used to identify patterns in HFUs.  
