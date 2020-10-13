# Weak-Supervised-Learning-for-Drugs-Lexicon-Detection
Here, we attempt a recent implementation of weakly supervised learning model, as well as pre-trained LSTM model for drugs-related context detection as an attempt to leverage publicly available dataset to detect emerging illegal drugs discussions on the internet. We demonstrated the efficiencies of our method on the Urban Dictionary Dataset, identifying ~1000 terms surrounding drug abuses that did not exists in previous literatures.  
Below here are some steps to reconstruct our pipeline
## Requirements
- Python 3.6
- [Keras](https://keras.io/)
- [Knime 4.1](https://www.knime.com/)
## Knime weak supervision for drug abuses modeling
- Install [Knime](https://www.knime.com/)
- Add Python 
- Run Weakly_Supervised_Model.knwf in Knime. Once the model is loaded, go to Knime/ Preference/ Python. If you have [Conda](https://docs.conda.io/en/latest/) installed, select New Environment.
- Run the model with train.csv as model input, rules.csv as model rules, and add DEA list to model references to obtain the desired results
## LSTM model for relevancy classification
1, Pre-trained python model: lstm.py  
2, Jupiter Notebook for Glove 50-d embedding case: lstm.ipynb  
3, LSTM model weight: lstm.model  
## Results
Cocaine data/ Heroine Data/ General Data/ MJ classified Data
## Sample Results
| basehead     | A crack addict . This is because crack cocaine is a freebase form of cocaine hydro chloride .                                                                                             |   |   |   |
|--------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---|---|---|
| clocking     | To sell crack cocaine                                                                                                                                                                     |   |   |   |
| oxyball      | when one snorts a line of Oxycontin mixed with cocaine . ; ; Oxycontin is a synthetic heroine that also acts upon the opiate receptors in the brain . The name is derived from speed ball |   |   |   |
| slingingrock | Selling crack cocaine
