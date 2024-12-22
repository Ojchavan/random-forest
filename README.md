Advanced Stock Market Prediction and Regime-Based Analysis

This project combines advanced technical indicators, market regime detection, and machine learning models to predict stock market movements, with a focus on Apple Inc. (AAPL). 
The model dynamically adjusts its predictions based on market conditions such as volatility and trends.
It also provides backtesting functionality for evaluating predictive performance.
Key Features

1. Advanced Technical Indicators

Momentum Features:

Exponential Moving Average (EMA) and Weighted Moving Average (WMA) for trend detection.

Rate of Change (ROC) and Momentum (MOM) for momentum analysis.

Volume-Weighted Indicators:

Volume Weighted Average Price (VWAP) and Volume Force for incorporating volume trends.

Volatility Features:

Parkinson Volatility to measure high-low price variation.

Average True Range (ATR) and Volatility Ratio for capturing short-term and long-term volatility.

2. Market Regime Detection

Trend Strength: Measures the difference between short-term and long-term moving averages relative to volatility.

Trend Direction:

Identifies strong/weak uptrends or downtrends based on moving averages.

Volatility Regime:

Categorizes the market into low, normal, or high volatility based on historical price standard deviations.

3. Dynamic Target Creation

Volatility-Adjusted Thresholds: Generates binary targets using a dynamic threshold based on rolling volatility.

4. Ensemble Machine Learning Model

Combines:

Random Forest Classifier: Captures non-linear patterns with feature importance.

Gradient Boosting Classifier: Focuses on error correction for better prediction accuracy.

Models are combined using a Voting Classifier to average predictions.

5. Regime-Aware Prediction

Separate models are trained for different market volatility regimes (low, normal, high).

Prediction thresholds are dynamically adjusted based on the regime.

6. Enhanced Backtesting

Evaluates model predictions over time using rolling windows.

Provides precision scores for both global performance and regime-specific performance.


**Backtest**                                                       **Random-forest_backtest**

Technical Indicators:                                                 
(RSI, MACD, Bollinger Bands, etc.)	                        (EMA, WMA, ROC, MOM, VWAP, ParkinsonVol, etc.)

Market Regime Detection	:
None	                                                      Trend and volatility regime detection

Target Creation	:
Static threshold of 1.5% return	                            Dynamic threshold adjusted for volatility

Modeling Approach	:
Single Random Forest Classifier	                            Ensemble model (Random Forest + Gradient Boosting)

Prediction Adjustments :
No regime awareness	                                        Regime-aware predictions with threshold adjustments

Backtesting	:
Standard backtesting	                                      Enhanced backtesting with regime-aware performance

Model Evaluation :
Single precision score	                                    Precision scores by regime (low, normal, high volatility)

Feature Complexity :
Standard features	                                          Advanced features and market regime encoding




Conclusion

This project demonstrates the use of advanced feature engineering, regime detection, and machine learning for stock market prediction. By leveraging market conditions and dynamic thresholds, the model adapts to varying market environments, offering robust predictions and valuable insights for traders and investors.

