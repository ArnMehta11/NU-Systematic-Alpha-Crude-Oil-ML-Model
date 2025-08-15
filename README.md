# NU-Systematic-Alpha-Crude-Oil-ML-Model
Research project for Northeastern Systematic Alpha (NUSA), exploring Machine Learning models to forecast Crude Oil Prices

Currently our research implements an oil price forecasting model based on the VMD-SE-GRU framework proposed in Zhang et al. (2023), you can find the research paper in the repository as well. The approach combines Variational Mode Decomposition (VMD) to break down West Texas Intermediate (WTI) crude oil prices into different frequency components, Sample Entropy (SE) to group similar components for reduced redundancy and faster computation, and a Gated Recurrent Unit (GRU) neural network to predict each grouped signal. 

The model, as proposed uses the past 30 days of prices to forecast future values, reconstructing the final prediction by summing the forecasts of all grouped components. This decomposition aims to improve accuracy over single deep learning models, handles the nonlinear and volatile nature of oil prices, and significantly reduces training time with minimal loss in precision. Performance is currently evaluated using RMSE, MAE, MAPE, and R², with results demonstrating strong predictive capability for both short- and medium-term oil price movements.

Currently the model fetches and sources the data from AlphaVantage, and you can get your free API key here: https://www.alphavantage.co/support/#api-key

Additionally, if you are interested in Systematic Alpha, either as an external sponsor/partner, or a student that aspires to join the club, feel free to reach out, you can find my LinkedIN on my GitHub profile, or can alternatively reach out to us through our site: https://nusystematicalpha.com/
