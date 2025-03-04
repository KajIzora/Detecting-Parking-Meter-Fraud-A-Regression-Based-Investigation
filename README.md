# Parking Meter Fraud Detection in NYC: A Statistical Analysis

This project investigates a dataset from New York City’s parking meter collections in the late 1970s, where suspected fraud by the private contractor Brink’s Inc. led to legal action. The city’s data compares monthly revenues from meters emptied by municipal workers vs. private contractors, allowing for a direct, quantitative assessment of discrepancies.

The analysis was conducted by first visualizing trends in collections over time for both public and private entities. Simple line plots offered an initial impression of monthly fluctuations in revenue. Next, correlation and linear regression techniques were applied to examine how private collections related to city collections. A key step involved excluding Brink’s months to establish a “baseline” model for honest contractors. Applying that baseline model to Brink’s collection windows yielded an estimate of the shortfall allegedly stolen.

Underlying all this work is classical linear regression: we modeled the private contractors’ collections as a function of the city’s reported figures. Residual plots helped identify outliers or systematic patterns that might indicate theft. The slope and intercept were then interpreted to understand how much more (or less) private contractors were collecting, relative to the smaller subset of meters tracked by the city. An additional statistical comparison—removing Brink’s data from the regression—made the suspected theft clearer, with an estimated difference of about \$2.35 million.

Tthe evidence suggests significant underreporting in months when Brink’s handled the collections, reinforcing the city’s suspicion of theft. While no single analysis can prove guilt, the linear regression and resulting discrepancies point to a meaningful shortfall that aligns with the legal case pursued by the city.

**R Libraries Used**
- R base packages  
- ggplot2  
