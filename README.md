This notebook is based on this great article:

https://techrando.com/2019/08/23/unsupervised-machine-learning-approaches-for-outlier-detection-in-time-series/

and it's meant to confirm an hyphotesis: that the Isolation Forest's results can be easily improved by adding local information to each datapoint.

By using only the gasoline price, the Isolation Forest algorithm find those range of prices with less occurrence and mark them as anomalies. But it does it by ignoring the concept of time series and the information their neigbours provided, hence sudden spikes, for instance, could not be found. Just adding moving average information we can better spot real anomalies.

[Here it's the Jupyter Notebook with the experiment.](https://github.com/ricgu8086/Isolation_forest_for_time_series/blob/master/Isolation_forest_for_time_series.ipynb)
