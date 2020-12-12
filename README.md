# Hotel_Review_Rate_Classification
The assignment is a classification task for hotel reviews. There are 5 ratings that are the labels to be predicted based on the text in the reviews. There are three Data Sets: Training, Test and Dev. Two models is selected: A Baseline model and 2. A State of the art (SOTA) model. The performance of the two models are compared.

First in the both models, a preprocess step was done by filtering the data using TF-IDF weighting scheme.

Second, I used the decision tree as a baseline model [1]. Decision Tree [2] is a hierarchical decomposition of the (training) data space, in which a predicate for the attribute value is used in order to divide the data space hierarchically. In the context of text data, such predicates are typically conditions on the presence or absence of one or more words in the document.

Third, I used Logistic Regression as the other State of the art (SOTA) model [3,4,5]. The logistic regression classifier uses the weighted combination of the input features and passes them through a sigmoid function. The logistic regression model is often capable of providing highly accurate predictions in text classification especially in high scale Data.

Finally the outputs of the two models are compared using Accuracy metric. I used the Dev data set for the performance comparison (since we have the labels for the data) as follows

The accuracy of the logistic regression is: 0.7351927295518647, however the accuracy of the bassline model is Accuracy: 0.39580068943904734. These results were expected as we mentioned above the logistic regression is often provide high prediction in text classification. The decision Tree is usually leads to overfitting of the data. If we have a situation where there are not always interactions and correlation between the observation like our case, then decision tree will not perform well and regression might be the best.

I have implemented four python scripts using Google Colab editor (widely used in the machine learning community):
1. Two scripts for the Baseline model (one with evaluation and one without)
2. Two scripts for the STOA model (one with evaluation and one without)
All the scripts are uploaded to GitHub repository:
https://github.com/IsmailElSayad/Hotel_Review_Rate_Classification

For any further discussion, I am ready to discuss. Waiting you feedback

1. Blockeel, Hendrik, et al. "Decision trees for hierarchical multilabel classification: A case study in functional genomics." European Conference on Principles of Data Mining and Knowledge Discovery. Springer, Berlin, Heidelberg, 2006.
2. Aggarwal, Charu C., and ChengXiang Zhai. "A survey of text classification algorithms." Mining text data. Springer, Boston, MA, 2012. 163-222.
3. Do, Chuong B., and Andrew Y. Ng. "Transfer learning for text classification." Advances in neural information processing systems 18 (2005): 299-306.
4. Genkin, Alexander, David D. Lewis, and David Madigan. "Large-scale Bayesian logistic regression for text categorization." Technometrics 49.3 (2007): 291-304.
5. Zhu, Ciyou, et al. "Algorithm 778: L-BFGS-B: Fortran subroutines for large-scale bound-constrained optimization." ACM Transactions on Mathematical Software (TOMS) 23.4 (1997): 550-560.
