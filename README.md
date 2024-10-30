Berkeley Haas ML AI Practical Application 3<br>
Yash Bhargava<br>
10/29/2024

Link to <a href="https://github.com/yash-b18/ML-AI-Practical-Application-3/blob/main/prompt_III.ipynb">Notebook</a>


<h2>Comparing Classifiers</h2>
<p><b>Overview:</b> In this practical application, your goal is to compare the performance of the classifiers we encountered in this section, namely K Nearest Neighbor, Logistic Regression, Decision Trees, and Support Vector Machines. We will utilize a dataset related to marketing bank products over the telephone.</p>

<h2>Getting Started</h2>
<p>Our dataset comes from the UCI Machine Learning repository <a href="https://archive.ics.uci.edu/dataset/222/bank+marketing">link</a>. The data is from a Portugese banking institution and is a collection of the results of multiple marketing campaigns. We will make use of the article accompanying the dataset <a href="https://github.com/yash-b18/ML-AI-Practical-Application-3/blob/3248b1ee3e86cff85d6df256b2e99b5bd7264e01/CRISP-DM-BANK.pdf">here</a> for more information on the data and features.</p>

<h2>Process</h2>
<p>In this practical application using the bank marketing campaign dataset, the objective is to predict whether or not a client subscribes for a term deposit.</p>

<p>Through some visualizations, we identified some characteristics about clients who subscribed to a term deposit. For example, majority of term deposit subscribers were between the ages of 30 and 45, had jobs of technician and blue-collar with a university degree, and most likely married or single.</p>

<p>First we analyzed the dataset and performed some data cleaning steps such as converting data from categorical to numerical data where applicable, removing missing data and duplicate data, and removing outliers.
After, a baseline model was created that the classifier should aim to beat. The accuracy of this model came to be 87.18%.</p>

<p>Further, we created Logistic Regression, KNN, SVM, and Decision Tree models and recorded the runtime and accuracy of these models on the training and test dataset. The conclusion of this was that Logistic Regression seemed to be best model as it provided the highest test accuracy with the fastest runtime. SVM had the same results but was much slower.</p>

<h2>Model Improvement</h2>
<p>After our initial models were created, we explored hyperparameter tuning, specifically Logistic Regression, KNN, and Decision Tree models. End result is KNN was the best model with hyperparameter tuning. The parameters used for KNN model was k = 14, weights = uniformed (meaning all features contributed equivalently), and metrics = manhattan.</p>

<p>Logistic Regression came in second place with the next highest test data accuracy, followed by Decision Trees.</p>

<p>We also decided to look at Recursive Feature Elimination with hyperparameter tuning on the logistic regression model, however, that did not impact the test accuracy score.</p>

<h2>Next Steps/Recommendation</h2>
<ol>
    <li>Feature exploration on importance towards a model should be discovered.</li>
    <li>With the right computer, SVM should be explored with hyperparameter tuning.</li>
    <li>Principal Component Analysis (PCA) along with Recursive Feature Elimination (RFE) should be explored for modes like Decision Trees.</li>
    <li>Features that were not used should also be considered as important factors in training a model and also be explored as a possibility for use.</li>
</ol>

<h2>Conclusion</h2>
<p>After hyperparameter tuning Logistic Regression, KNN, and Decision Tree models, KNN had the best test accuracy of 0.872 or 87.2%, and the most optimal k parameter was 14. The weights parameter was uniform meaning that each neighbor contributes to the prediction equally. RFE was explored for Logistic Regression, however, with both hyperparameter tuning and RFE, the model accuracy did not improve. In fact, it stayed the same throughout.</p>
