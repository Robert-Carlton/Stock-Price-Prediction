# Summary
This project aimed to improve stock price prediction and make the results more understandable for investors through an innovative visualization dashboard. Traditional approaches often rely solely on historical price charts or candlestick graphs, but this system integrates predictive modeling with detailed data on the underlying factors driving price changes. The team gathered technical, fundamental, and social sentiment data, along with six PESTEL categories—political, economic, social, technological, environmental, and legal—to create a richer context for each stock.

Using AutoML tools and the PyCaret framework, the researchers trained and evaluated multiple predictive models, including ARIMA, Gradient Boosting, Bayesian Ridge Regression, and others. They also tested ensemble models that combine several algorithms. Surprisingly, the results showed no single “best” model for all stocks, and ensembles did not always outperform individual models. The dashboard allows users to see predicted prices, compare model outputs, explore the PESTEL factors influencing each prediction, and benchmark a stock against similar companies.

# Highlights

:heavy_check_mark: Motivation

  * Stock price movements influence global economies, investment strategies, and individual financial security.
  * The US stock market represents ~60% of global equity value, affecting over 60% of US adults who have investments.

    
:heavy_check_mark: Data Innovation

  * Combined technical (price history), fundamental (economic indicators), social sentiment, and PESTEL data for a comprehensive view.
  * Data sources included free APIs (Yahoo! Finance, FRED) and paid APIs for specialized PESTEL metrics.
  * Scope: 47 unique data elements per stock, 730 days of history, 6 PESTEL categories.

:heavy_check_mark: Modeling Approach

  * Used AutoML and PyCaret to test and tune models including ARIMA, Bayesian Ridge, Gradient Boosting, Random Forest, ElasticNet, AdaBoost, and LightGBM.
  * Applied five iterations of hyper-parameter tuning, blending top three models, and optimizing ensemble weights.
  * Predictions made for 1–7 days ahead.

:heavy_check_mark: Key Findings

  * No single model consistently achieved the lowest RMSE across all stocks—model choice should be stock-specific.
  * Ensemble models were not always superior; for example:
  * AAPL best predicted by Gradient Boosting (RMSE ≈ 4.14).
  * GOOGL best predicted by Bayesian Ridge Regression (RMSE ≈ 0.67).
  * TSLA best predicted by ARIMA (RMSE ≈ 1.02).

:heavy_check_mark: Visualization Dashboard

  * Displays historical and forecasted prices for multiple models.
  * Shows PESTEL factor trends for each stock.
  * Provides comparative metrics for similar companies to contextualize predictions.

:heavy_check_mark: Future Directions
  * Test different input datasets per stock to improve accuracy.
  * Evaluate the impact of individual data categories on predictions.
  * Extend forecast horizons to 30 or 90 days.
