# Heart_Failure_Prediction
Predicting the appearance of heart disease using a kNN, weighted kNN, decision tree, and random forest algorithms. 
Normalized and unnormalized data were used for each of these models (8 models in total).

Baseline performance: 47%

<u>Unnormalized Data Results:</u>  
kNN: 86.4%  
Weighted kNN: 85.3%  
Decision Tree: 83.2%  
Random Forest: 83.2%  

<u>Normalized Data Results:</u>  
<b>kNN: 89.1%</b>  
Weighted kNN: 87.5%  
Decision Tree: 83.7%  
Random Forest: 83.7%  

</t>One of the most surprising results from this project was the poor performance of the decision tree and random forest algorithms. The highest accuracy out of this set of algorithms was 84%, achieved by the random forest algorithm on normalized and non-normalized data. Upon further analysis, it can be explained why these algorithms performed poorly. By observing the feature importances chart generated by this algorithm, there were only three variables that appeared to provide a significant information gain (ST_Slope_Up, Oldpeak, and Age). This was also confirmed by the decision tree experiment, where max_tree_depth was a tuned parameter that indicated three levels of leaf nodes resulting in the most accurate results. The poor results of these algorithms surprise me considering many fields of science prefer the use of decision trees for the explanation of an event. While the benefits of readability are evident, the ultimate performance of this data does not correlate as nicely.  

</t>In general, medical diagnoses can be complex a system of equations that attempt to weigh an individual's symptoms. In rare cases, there are anomolies that ultimately hurt the effectiveness of a simple decision tree over time. Therefore, the benefits of comparing large numbers of individuals against each other at once (kNN) outweigh the costs of a more cryptic decision process. Even though decision trees provide the benefit of identifying the most important features, a kNN algorithm would be best suited to use these features in its own experiment, weight them accordingly, and analyze them against a sample to formulate its conclusion.
