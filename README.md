# Altered-Activation-function-m-arcsin

## Project Overview
This repository presents an exploration of kernel and activation functions, particularly focusing on their role in machine learning algorithms such as Support Vector Machine (SVM) and Multi-Layer Perceptron (MLP). The central theme revolves around the evaluation of "m-arcsinh," a modified version of the inverse hyperbolic sine function, proposed as an effective kernel function for SVM and activation function for MLP. The team reproduces results from a subset of the original paper's classification datasets using scikit-learn and demonstrates competitive performance compared to default kernel and activation functions. The function definition is as follows: <img width="213" alt="Screenshot 2023-12-21 at 16 12 43" src="https://github.com/JohanTrippitelli/Altered-Activation-function-m-arcsin/assets/154525880/9ba89b70-5c26-46b7-ba7f-f2a66ffd8792">


## Introduction
The project investigates the performance of "m-arcsinh" as a kernel function for SVM and an activation function for MLP, comparing it to the established "gold-standard" functions in scikit-learn. The study emphasizes the conditions for redefining a function applicable to both SVM and MLP, highlighting the need to maximize margin width for SVM and improve or maintain classification standards for MLP. The proposed function, "m-arcsinh(x)," achieves this by combining the inverse hyperbolic sine function and a slightly nonlinear function, demonstrating suitability for both SVM and MLP.

## Datasets
The project employs a subset of five datasets selected from the original paper, including "breast cancer wisconsin," "iris," "olivetti faces," "wine," and "digits." These datasets cover binary classification, multi-class classification, and image classification scenarios, providing a diverse set of testing scenarios.

## Results (Compared to the original paper)
The team evaluates the performance of "m-arcsinh" on various datasets, comparing results with the original paper. The evaluation metrics include accuracy score for performance and precision, recall, and f1-score for reliability, with training time in seconds as a measure of computational cost. Despite using different hardware (Google Colab), the trends observed align with the original paper's findings, supporting the effectiveness of "m-arcsinh" as a reliable and efficient function for both SVM and MLP.

## The variation of Gammas for SVM
The project conducts experiments to assess the impact of varying gamma values on the m-arcsinh kernel function's performance for SVM. Results on the Iris and Breast Cancer datasets demonstrate consistent accuracy, precision, recall, and f1-score across different gamma values. The study concludes that the choice of gamma values within the specified range does not significantly impact the model's predictive performance on these datasets.

## Challenges and solutions
Challenges faced include calculating training time, preprocessing datasets, and incorporating the custom activation function for MLP. The team records training time by capturing the duration before and after fitting data. Preprocessing involves using scikit-learn functions for dataset loading and division. Due to limitations in editing scikit-learn source code on Google Colab, a simple neural network using TensorFlow replaces the MLP classifier with the m-arcsinh function.

## Key Takeaways and Future Directions
While "m-arcsinh" may not be the best function in all scenarios, it consistently outperforms default functions in scikit-learn. Its applicability to both SVM and MLP makes it a strong candidate for consideration. The study suggests future investigations focusing on optimizing the high training time for MLP when using "m-arcsinh."

## References
The report includes references to datasets, Google Colab, the original paper on "m-arcsinh," and scikit-learn. The appendix contains additional experimental results for the Olivetti Faces, Wine, and Digits datasets, supporting the findings presented in the main report.
