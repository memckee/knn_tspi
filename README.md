# Evaluating Complexity-Invariate Distance in K-Nearest Neighbors Algorithm for Financial Time Series

This project evaluates a modified k-nearest neighbors algorithm (KNN) for forecasting financial market time series. KNN, a supervised learning technique, requires data prepared to facilitate calculating vector distance and making either regression or classification predictions. This notebook uses sub-series normalization to prepare data from daily return data of 126 U.S. equities and ETFs. KNN predictions are then evaluated with regression and classification metrics.

The modifications to KNN used in this project account for time series complexity as suggested by Batista et al (2014). The full KNN implementation is demonstated by Parmezan and Batista (2015), who compared the typical Euclidean distance measure to a complexity-invariate metric. 

After using complexity-invariate distance, the model was evaluated according to six metrics - four regression metrics, two classification metrics. Please the KNN TSPI notebook for details and results.

![Model Evaluation](Images\metric_graph.png)

## References

Batista, Gustavo E. A. P. A., Eamonn J. Keogh, Oben Moses Tataw, and Vinícius M. A. de Souza. “CID: An Efficient Complexity-Invariant Distance for Time Series.” Data Mining and Knowledge Discovery 28, no. 3 (May 2014): 634–69. https://doi.org/10.1007/s10618-013-0312-3.

Hyndman, Rob J., and Anne B. Koehler. “Another Look at Measures of Forecast Accuracy.” International Journal of Forecasting 22, no. 4 (October 1, 2006): 679–88. https://doi.org/10.1016/j.ijforecast.2006.03.001.

Parmezan, Antonio Rafael Sabino, and Gustavo E.A.P.A. Batista. “A Study of the Use of Complexity Measures in the Similarity Search Process Adopted by KNN Algorithm for Time Series Prediction.” In 2015 IEEE 14th International Conference on Machine Learning and Applications (ICMLA), 45–51. Miami, FL, USA: IEEE, 2015. https://doi.org/10.1109/ICMLA.2015.217.