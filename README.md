📈 Dynamic Pricing & Demand Forecasting Engine🚀 
Project Overview -This project addresses a critical challenge in e-commerce: balancing inventory levels with profit margins.
By combining time-series forecasting with econometric price elasticity modeling, this engine provides data-driven recommendations for price adjustments and inventory restocking.
🛠️ Tech StackLanguage: Python (Google Colab)
Forecasting: Meta Prophet
Statistics: Statsmodels (OLS Regression)
Data Manipulation: Pandas,
NumPyVisualization: Matplotlib,Seaborn
📊 Core Components1. Demand ForecastingUsing Prophet, the model analyzes historical sales data to predict demand for the next 30 days. 
It accounts for:Weekly and yearly seasonality.Holiday effects and promotional spikes.Confidence intervals for "best-case" and "worst-case" inventory planning.
2. Price Elasticity of DemandI implemented a Log-Log Linear Regression model to quantify how price changes impact consumer behavior.Calculation: $ln(Quantity) = \beta_0 + \beta_1 \cdot ln(Price)$Insight: Identified which products are "Price Sensitive" (Elastic) vs. "Necessities" (Inelastic), allowing for targeted markdown strategies.
3. Dynamic Pricing AlgorithmA decision-support system that suggests prices based on:Scarcity: Increases prices when predicted demand exceeds current stock.Liquidation: Triggers automated discounts for slow-moving inventory based on calculated elasticity to maximize recovery value.
💡 Business ImpactImproved Accuracy: Achieved a high level of forecast precision compared to moving-average baselines.Margin Optimization: Theoretically increased profit margins by reducing unnecessary discounts on inelastic products.
Automation: Reduced manual pricing overhead by creating a programmatic "suggested price" trigger.
