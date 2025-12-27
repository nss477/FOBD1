This experiment successfully demonstrates the implementation of a scalable machine learning classification workflow using Spark MLlib, 
fulfilling the learning objectives of data preprocessing, model construction, hyperparameter tuning, and performance evaluation on a large, real-world
dataset. The workflow reflects industry-standard practices and highlights the importance of structured analytics pipelines for complex data processing
tasks.
Statistical imputation was applied to handle missing values while preserving dataset integrity. Instead of removing incomplete records, median-based
imputation was used for numerical features, ensuring robustness against outliers and minimizing bias. This approach allowed the model to leverage the
full dataset, which is particularly important for imbalanced classification problems such as fraud detection, where minority-class examples are scarce.
By retaining all observations, the analytical process maintained data completeness and improved the reliability of model learning.

Feature scaling significantly improved model optimization stability. Logistic Regression relies on gradient-based optimization, which is sensitive to
differences in feature magnitude. Standardization ensured that all features contributed equally during training, resulting in more stable convergence
and consistent performance across multiple runs. This highlights the importance of proper feature scaling when applying optimization-based classifiers
in distributed environments.
Hyperparameter tuning using Sparks CrossValidator produced measurable performance improvements. By systematically exploring different regularization 
and elastic net parameters, the tuned model achieved higher evaluation scores compared to the baseline configuration. These improvements demonstrate
the effectiveness of controlled experimentation in enhancing model generalization without introducing overfitting.
Area Under the ROC Curve (AUC) proved to be a more meaningful metric for assessing model discrimination capability. The inclusion of F1-score further
balanced precision and recall for the minority class, providing a more comprehensive assessment of model performance. Overall, the experiment confirms
that thoughtful preprocessing, pipeline design, and metric selection are essential for building robust and scalable machine learning solutions.
