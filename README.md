 FCC-yeild-prediction-with-PINNS-model-and-time-dependency-for-more-aciracy-and-time-dependent-
This project predicts FCC process yield using Catalyst to Oil Ratio, Feed Rate, and Temperature parameters. It explores time dependency and compares Random Forest, ANN, and Physics-Informed Neural Networks (PINNs) to enhance prediction accuracy.
 FCC Yield Prediction Using Machine Learning and PINNs

This project involves predicting the yield in the Fluid Catalytic Cracking (FCC) process using various machine learning models (Random Forest, ANN) and Physics-Informed Neural Networks (PINNs). The dataset includes process parameters such as Catalyst to Oil Ratio, Feed Rate, Feed Temperature, and Catalyst Temperature. We also explore time dependency on yield prediction.

 Problem Statement
The objective of this project is to predict the yield of the FCC process using data-driven machine learning models and PINNs, integrating physical laws and dynamic time-based behavior.

 Methodology
1. Data Collection and Preprocessing
   - Generated 100 random samples for the FCC process parameters within operational ranges.
   - The parameters include:
     - Catalyst to Oil Ratio
     - Feed Rate (BPD)
     - Feed Temperature (°C)
     - Catalyst Temperature (°C)
     - Yield (%)

2. Traditional Machine Learning Models
   - Implemented Random Forest and ANN models to predict yield as baselines.
   
3. Time Dependency Modeling
   - Added time as a parameter to explore the relationship ( Yield(t) = a c.t^n ).
   
4. Physics-Informed Neural Networks (PINNs)
   - PINNs integrate physical constraints (differential equations) and data-driven learning. A custom loss function includes both:
     - Data Loss: Mean Squared Error (MSE) between predicted and actual yield.
     - Physics Loss: Penalizes violations of physical laws.

 Experimental Setup
- Hardware: 16 GB RAM system with GPU support.
- Software:
  - Python
  - Libraries: TensorFlow/Keras, Scikit-learn, Matplotlib, Pandas, NumPy

 Results
- Evaluated models using MSE and R-squared metrics.
- Compared the performance of Random Forest, ANN, and PINN models.
- Visualized the dependency of yield on time and physical parameters.

 How to Run
1. Clone the repository:
   ```bash
   git clone https://github.com/username/FCC_Yield_Prediction.git
